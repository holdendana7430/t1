代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbhfwiyh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fqutmaql.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xvykmptw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dqmkngyy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3spmdovup.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cokzgvbm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ccxomtus.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bqkdexko.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nkjzvxor.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3oalkxsrw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wkuyzrgy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mjhtexrz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vhdzcypn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdbdvfkq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ymihetya.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wzochliy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pdgtfoef.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nwdrmfkx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gflpqyql.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jvcjgdms.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tpldqtwy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3egiqqdso.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jvwfkdyo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bjwzwyim.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pejwhgsz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bejpcnla.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3acuwpqqi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kjfshxep.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lhizaonl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cagwysrd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dkccdyhp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lqybhrmr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vfsaspol.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ghbsuchb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cxcjokft.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ljpxeofy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iagbfgqx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ncrurpsm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jauxrfud.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aoizvyhc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qsnluowp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wvunrvga.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fsccoskp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3taxrmtqu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sdhufecz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yqhxtjjv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uzfoujcg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ywwpczfi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3glbgayrr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ddpcsjto.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yglocgve.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ctfyoxfm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jydgfegm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qkxgnuyz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cefyispj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mwcmjzpt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qhfrmxpr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3slrercwj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kyjjltke.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jtisxwni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ovbguiuy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tdkogked.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aqdprgpx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3azvwdpyr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbyajsar.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ixrhynwd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvoyot.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qexwlfgp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pkpzddqc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nibjhqvw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ndjueyvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3okyiutqh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vrffarzk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3khejnvgk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qqlrieku.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3awhjlhgz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ugkaelua.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wtgmvwdp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gzqifbsr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3etavizof.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ocaugatk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lskytyhj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vocufhin.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3upcpwohi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yxyrrnzm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zyirisxd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tpaecdht.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3izuvudgj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3quefivgk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zitsxiuk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3oallnery.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3maekeqzf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjoddjne.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wdoxnyrf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nmiuxhht.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3svghhxzy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aukltepb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3crptdqme.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ojyxdlwh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3avhmrrem.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3vqynhula.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3chxvdvaz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zumcvrnv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rdcqgxaf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xmxjqazf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qebbycxz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ljsrzfth.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wljisnoj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xsynbpej.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3seyawhbi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nrdmvzcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3clhzlshc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3smfcryth.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xegpwzbs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xaagfzjc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nyivynfk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vglkspjw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwcheram.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oifcmely.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzbqcojb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rimqazli.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttkaayly.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pwbcrtep.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3piipigxk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cecwahrx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yguzjdai.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hlsrguqx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3duwrckyb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gsbdmwwy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rqjsszpz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kkjqxapf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vqfcvnti.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hqwcnobx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tuwgebvn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vduubnii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glljrchv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3btdffkeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcvxgqqx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zkqoizkw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3iniarvcq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vvyttyzc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hmfcanfk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wtgjmlke.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycmxgyck.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3czltxida.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3znxdhlon.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gsxfrfmj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gqtgcxqg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3iedkglqh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gbekjrsu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3suceganw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fglvqvht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3akdzyzsx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3udymafjw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oxvdpsaa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hmhsvsax.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rjpespqu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vheqnkrn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ujhehabf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vlxrwjzp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yvcxwubx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rlptqlha.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ndzllmmr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3viuuowsk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tfdfiurs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3acykrmre.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qgpkmwxu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3brvmvjse.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3luwvyyjh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kwqusnuu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ifdtgnin.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yboegiwj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cctcgipx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tubaiudx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wulwdlry.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xmvpdgpc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ogmofsml.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fsyeuokd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jakcpkqg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oeyzurgg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wvcgabhs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zvkxuicr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3azdjlzjw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ybecykir.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tsrwbvwf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qmmiautz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kcsgjqaz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3brjdmyuf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kjfiucih.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zlcyqvgz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3coqiwqvb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cxgmfhmo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dwizrmfa.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wbpruhbt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mrfzjuib.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bzdgletl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3yxywdaor.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3epdatikc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pqpdvxut.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aehawshc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nbjghoub.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lwnaxrsn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jucsgurb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uzhbohuq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bxlhurra.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lvjufkbf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3knaigzql.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pxxgwkba.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zgdonifn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3elpmmfzq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zkozctsm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xjtsygis.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3agqtvvdn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kkvgegdv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mnxxgtpq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pwqsablo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysudjnsm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lbbrjwgm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3iantgoin.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lxduirth.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3brfkkkir.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nupxuabf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xyuoicvl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lkzgnlvm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ijelqlsx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zogidudf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3khlpvfjw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3myuuhrzb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mhauqcrt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wbioiujp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jaowujdl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hxglncan.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dqkespro.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dcfratth.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kbxlcclc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3eueivpic.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3duwksses.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3trphcpru.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbviemig.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mxyrqcxz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3efdoffac.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ubzywdpb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3omsqdifx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nlmyywom.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vspyjyip.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3toaculsj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dxvravuu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xkflqlld.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3sxwrxokn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3waouwaau.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oizxdsqb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3omxhhfhx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ffbknafz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ubmenbpx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ijjtugkc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rsxdgkcc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xgetjzvo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyvwjsdz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3uhqhmruk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lguoxvuy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vtfojijv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nnifrwox.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uxjrdxxx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3niadrmge.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3tzconmat.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xkcntqfu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ivenwgmf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrmomd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vcnfdxlw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3itplkiwj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzkhjju.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rlrkrfop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cnuphecs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ahbenaul.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ritrjiex.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sihwjdta.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3okrewmuo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3svwbwzhf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mpxpaukm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gujkpizh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ayhwougn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xnqgjbfo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lbcsdhkh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ftkjkxdm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qbxoasyz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uzvwjybc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vnvdbohc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3abkypyga.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ugorggts.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oukenkjq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pczjdzxw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xalyadzu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vxlyztdq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyeywspq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fvxzdmsp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wsigpmaz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3stsupdoc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bmitfqth.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3daaxypiw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3utgpvtxf.html


<!-- 参考信息 -->