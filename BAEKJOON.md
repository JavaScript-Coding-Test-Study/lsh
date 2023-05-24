## ���ؿ��� JavaScript �ڵ��׽�Ʈ

 - ��� : nodeJS ����ϱ�
 - �ܰ躰�� Ǯ���


 1. ���

  - nodeJS ����� console.log()�� ����ϸ� �ȴ�.

   > console.log("Hello World!");
   // "Hello World!" 


 2. �Է�
 
  - fs.readFileSync()�� ���� �Է°��� �޴´�.
  - ���� ��ġ: '/dev/stdin' ���� ����Ʈ�� ������
    (���� ȯ�濡�� ���� �ÿ��� �ڽ��� �Է� ���� ��ġ)
  - ��� ������ ���� ����� ������ ���·� ����

   > const fs = require('fs');
   // ���� �ý��� ��� ����Ʈ

   > const input = fs.readFileSync('/dev/stdin');
   // ������ �Է°��� readFileSync �Լ��� ���� ������ �Է°��� �޾ƿ´�.
   

 3. �Է°� ����

  - JS�� String.split() �Լ��� Ȱ���� �Է°��� �迭 ���·� �޾ƿ��� ���
  - split() �ż���� �迭�� �����Ͽ� �Է°��� �پ��ϰ� ������ �� �ִ�.

   > const charArray = input.toString().split('');
   // �Է°��� �� �ܾ��̰�,�� ö�ڸ� �迭�� �޴� ���

   > const wordArray = input.toString().split(' ');
   // �Է°��� �� ���� ���� �ܾ��̰�, �� �ܾ �迭�� �޴� ���

   > const numArray = input.toString().split(' ').map(Number)
   // �Է°��� �� ���� ���� �����̰�, �� ���� �迭�� �޴� ���