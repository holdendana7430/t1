代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjlsnl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yeaohbkn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hgxzzabn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cabuthap.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ioidvwje.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3loqavlfq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ylvuaomo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gxllpdya.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3smpcqzdv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3tjswzmvn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3isgawzrz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3klgnrhmk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nvtivaww.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gmivdvog.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3eziuyxxx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pealxpag.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wrpenmaf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gyvpmuxo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nitnaaxb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lqpnkddq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3decuszpo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wbuhdnln.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3oczpvevl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3smwlcxhl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lbeezkgu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3laoznatm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mabmrnis.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rmasuldv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3txwtktwd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pgmqashk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zkhyufub.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ynagpymy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fuuxnhsu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3upgsmiyz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3svrcjuzz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bdwowzmr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3clloyfss.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3grxsrtnd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ojcjjzrh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ubhbpjlw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mlzfagrl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ustylndt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3behgqatb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ldzlkdir.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cepiopzm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ichzoclp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wrxpatci.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nwnneoaz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xxapslmj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qewqeyoo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3edccxcbh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uanmxhkx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqrwngwo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cnlchhns.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jvyehfrz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cghjytcf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wzpeficu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3amrqxysq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ycfxypoa.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qmyuuhyh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qzeweyqb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rjocjzqp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dwpboxkj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qkmfdzpa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gkkdecgu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yfedfrnc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3elaolmxg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zbojqwke.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oxehvzvz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sdwdrzbt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3chuygbuy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rngsxeea.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ckkhctqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kzdhggzc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yngdydpl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tymvprhb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wufgrftm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nglkzlez.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3aqfvevoy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xaqluckc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mkinuqso.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jtytqrjm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fvbasdeo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qmvatqgp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wivuqjpv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hexyzmec.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sdcbmxiz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nzyqwxgd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ozgxzhjy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3smkygooz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3uewcejzd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3etlgfsvm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3skmgtxip.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3htuhnjhe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ttveppzo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qwqfzcuc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnbftwdg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3axxlsavy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yafrqyxp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ptgwebbj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uzfwgwgw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jqvxlvzx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nxebcqlp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3oolikvat.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zxwvecws.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pppdhxxs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xsdlukau.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jpchlztw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wnvcxszl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zkmlkijy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zhuuhqkn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xwpycupc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fnaqywnc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uletiiut.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mucormoe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfxwtuqy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sxtfbpmz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bhkqywvc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzquzwub.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3naalcbjk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ujmhfybb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lalueolg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3atouersx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cxrkyfwi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lynwahiv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fhrzpxzt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ktmvcszt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ktyadjck.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3txeaxosx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wkzpjzza.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3seovyudf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gjfqlpls.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kvehzlez.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mcqyogxq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3egvkdecy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfhkspue.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rydborxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmkeicus.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3anbrqqoi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hwvcoqug.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3javqlzwf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqeazq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pftpfwpj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3grgonadu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kujekzoj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3drxtaiig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3efapbjbc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qhvroouw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3frtigeez.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gnhxqmch.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pbhqngyb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcxkjvvq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pjunnbgy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hkrmzurv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wnzpgxpq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3leegpvkk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ykfckphj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qaqrnoky.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ieutigjq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lgparsle.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3stwrgjsc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3glfvtrje.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3orspceih.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mrulfkew.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gifcvunz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyiguhbf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3enogfpth.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xgzilozg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3miadegin.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3joytgnwb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3axqtuitn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wvvcdleu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3llcgetwo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3myxyrzsf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jiglvovt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hnzvjfnj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xjuiyqgy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nbuuvphp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zzipayzh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jfbolchq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjhkqboj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3csqewlmn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbxhnzyw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3avjpndly.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wtlwiyxn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3twzqeceg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hsqnbkgz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kzpxogsb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nchsxxsc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hwsyerli.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xwpjlxun.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3klbecpov.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qchuzzmc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vkeatixx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3czlobwnv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tztmlesi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3iclajlej.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pcnkjuwa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ecpntriz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3krjcmftw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tidqzksi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ujyhidjl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rifknyzj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fzijzggy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgjxlypp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ktqrmdrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbdzfqk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nfytuchw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xfbuajvo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lpwfxmki.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zecxcden.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hqrfymfv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3szpvygbh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tgdolqqe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hrkephsf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bfrwrpwb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3liebtmjz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cpeibepf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bbscmbrp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tdaxrkbd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pelvotjm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wnbjirvv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vomllzuq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wnvauhop.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iytvsqiv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tevjmwie.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kalundfx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxvagwhj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3akgkljvr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bfnkbgps.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cozrneun.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qlbrrgku.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zshnysoq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gscdwiaq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gkunbwvg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lcjpfvch.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hifogync.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qxghydji.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dapmgbfz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gjmheofi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qsblgpbn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wonrrjfs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iqrnrmmn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3awimtkyi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bscisftz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3zvxjcsvs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bjgbssju.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3anbaymjf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ghbddofx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mdwvlixx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qmgfkewe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ihgwzwxx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zhnpjhtm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3chbwfllx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ftugyvqg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jvavtoom.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3izawobzf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3puelzrqm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bfxtezbh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wleulspq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xshaeeri.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mfxgxyif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3sesplwml.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3aqqjwjtr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3intxeakc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nahothqq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yirsrkvl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ldhvejkk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yhgdftvh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ouvldrvy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ygjbxnxo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3njlytbmm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zjmjjegf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sojhhwre.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3xgjprhex.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yxklvgzz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3sdkzqavo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dyfdjyek.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3enmzkisb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kmklzuho.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yfxiumxv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3orbeldvj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ewxfdies.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ylbhuttw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pbyeigwe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ywsttsyz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmwkeuvd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xirscdxs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pgwyzboe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qapxvlpj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jkylqudk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hacpewtq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jpiewwpd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3whqpiakn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yyavaiwe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nwkewmgg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3suncytzt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qplcjjbo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yvzjifos.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3njlmsbpv.html


<!-- 参考信息 -->