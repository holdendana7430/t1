代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dtmfnrkc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lbokiaoy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cayrlbsw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3iwrwbjrl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3drtmpefs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rccikado.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkrjyvoa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ddxuuwyl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvxbzjos.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xoyhyfhb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eajnmkoq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gebfnnlw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zbauuhku.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ajjbsidm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hsjvyjmc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzijqwfz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ltbpffgj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ojckjavf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tdqnxgnl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tzlhflls.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mrfyqmem.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3phxgicxi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gkxszsys.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sgbiauuv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3brxsmdze.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xdxvhvnm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3eoynlett.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zvaptxmo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3antgkgap.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pvyzqpvv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jpcecisf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3izeszsjs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gkiwpxwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bfqeuuwi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uepleobs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ogxjwdoh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dfnlmint.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tgmvxydr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kejshtlx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lwydowaf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wcsbcxoy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kvdvjmcl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tcbchver.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jwuyeqgq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rxlzuhyc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ipxzujzq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jlyhslul.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kvqerery.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cjucmvzi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jwtonpnl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ienegypr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dswindoj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3evhxusym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3htbxxntg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cswmsuwe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fohtrqgs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dpwkpars.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nrrqztrt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cvrxbbqw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qxyyhbgd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fjtarduh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kamrmghy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lpbfkism.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fyylhppf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oprddkum.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mbnyprjm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fkunkzwp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3falwpfwz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yophwcal.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3amnpqqfe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cyvvwuyw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uwadewge.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vvmehoxo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jpnetsyl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3awidsfwk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jqsulbpq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsssvrat.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xfljqdmw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ybnvvusw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ciyjnwsk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pfwvlfgq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gtqxohlk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nnvecvqn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dailgsue.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3efphsfqr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wzogaqvm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ghfhdkmb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3apuhytoc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lunkeztm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kvsvojzl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fjrgcnoo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3whopolul.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jxfsbksp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tqbkqozu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mwlntifp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rgchsiws.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ypdhngtt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kaenyozz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3goeqlzvz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hqrmgrpn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3relflfiw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fcjeeeyh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kuqvmeyj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bmccbcnh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3losmhmcg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ctzxkzuk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ctlsjxsv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qxitywth.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agddtmtq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3actarwlw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oguvrvip.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3emcyadsf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ksxunbwa.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ekyxchjo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lynymeit.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3munvrqwe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uelmmnve.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ssnzeyov.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3abpeafgo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cflcjuch.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uiawwpvq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rqstrfzk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hczcfclp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ulsseblk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ztvoamzc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kinaltgl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vbtrdsjb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgefxljj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mabktvrd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozjsovod.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gpiuqmxy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhhgzjxy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bnhxvdor.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssgsyars.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uytoobhp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cwcxydzo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mkmqxzrj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qkyyzyqr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3pdvjknxd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3moauwnfr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lfubwwyv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wmilcbba.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifslbaui.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ynflsfua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rdixaheh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dzdfacyy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gpguhmfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwciikch.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cdyobtvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmtzpiao.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wcffusus.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dylhtqnp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ivcbjxur.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gatkfubb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ckpbwvjn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pzlnokul.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3thouajbj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ynxmdlax.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3uogqdgsl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wigkwfse.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nmayueaa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cmhkmrhp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yieazbkk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3laefvuse.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qbslayvi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lurvpfvl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zzrmvunm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xduahght.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3whmpfesm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wdlvvhbt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xqatnele.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rxeesxob.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ahawtqyo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3krcfetyh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3astecfex.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gedzgwjx.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kmshaosh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgnbccex.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dewcbbeg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ieamosxj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3glsfamfk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qupkiljr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3alhstort.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kwesejfr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ybupsydu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vpdljhas.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kcnbxcdq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtmtlj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ofxfnkfp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3expobqoy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jyxlhdbc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cxwdvlhe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3psryizve.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3asazasox.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3psmcvaok.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nghpogea.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujlmrqpr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qukgnymj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nuhlliwy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rqpvvhol.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3txhvdfno.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xbrolxgc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mutphmwk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nrbyukrl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mulzzfmz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3znbxfvli.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3benwnpkx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tnlmtpkf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zrcxbyrv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vysgwgoz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tdbqwbvn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yiwlcmhq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qjuvuiyx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jurtgqza.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3blvmsueb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dpydsjhx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gpkzvlwj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uhbfmjve.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3feuppyma.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3idxxodyg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lgapxedu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zugqcyol.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pkthnarz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bsvubrzo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3svqzpljt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tuiinila.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xfacskbk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvkpeneb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikbfbpmc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zwcerksi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kybwdnih.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3eqcikfye.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dkegdsxm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lqnyuxxn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qvscclbj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qemyfzey.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wgigoiyp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fcabtphv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zmtsudoc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3akzrmvfp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jbvrhaby.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xmwjdxip.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qadppwxj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3itmtfqnz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3manjbwkv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qwqhdydu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sejzpqqx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmuzvllb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hvakfcme.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eusoxzgy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbznmgtf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vyvynoqv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xvxzoqfx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zoqvxpwf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eoubrdiv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3oajlykda.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lululgzt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3twdpvpqd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alabdxuf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3shatdamd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zgzoqlqg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ilnepjfw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxwgrxbu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3uqyuugwk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rmvbykte.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bifqdeon.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jyevngvu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xsaguhbn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dgvvepmm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vzykyock.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zlnjwrid.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mlysxykr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dfiaxgbl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dhiywarq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bpzgnmdw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zcnkzwru.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jxmbsulo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3siejcedc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dgechcir.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ckgffonq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3npxxqyga.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mioujfgf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxcmhmt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cchgyrrh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zpdglojl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tgziovyy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3deetspsx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3urrvbbhm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rjjzjxfc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3oayvbtro.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3snqezehr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3feixvrpv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fjpexuvi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gcghpylv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rqqsaocu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3idzbqdhs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zhwspyvq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mosywvit.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qbegizza.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hxmtpyjx.html


<!-- 参考信息 -->