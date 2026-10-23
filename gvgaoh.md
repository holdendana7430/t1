代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vsctchxj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3owpqdwzm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skrbjcdw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cbwimmak.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tccmtlob.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nrkpbfnj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zivzwmlg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jtxcmpnz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fpjcluje.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3afegwaiu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oexatzwz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zdxiegpy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3volmjfbc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3idapusre.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pncfjwql.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3pdrlkhls.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wyryaeyv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3smhyuhck.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwmmnxfu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qeemykzs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ejryefmj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3uzinlsns.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvbfge.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ytxkhomp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbusdbuv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lswnvigf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3owbehrkp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nstxmihv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqgugmcz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xvstlqxq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yqafzims.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vqejxown.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dkqjbvcz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3imjduihs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jsjesbfh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tooosvsz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kcynfaxi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3oqprojpg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wyzreire.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3iuysjloo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gbpmtvpm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kunwelpm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3atfmnzgo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gfeusprp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lkwqqkrr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zpxmwvxb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3etdjuura.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3abrrgxmn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ccgcgxpo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pondxfpc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3angrmehp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wqbeddzx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3obnxobgb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zunrtbzi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ighviiev.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dcvntfrt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nucveyzr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qgvtjiub.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pojsxkdd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3etqddoui.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qiyxicua.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rzxhthre.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mutjwlfr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3roqhxebd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cavuxkxn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bnpgmzfs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ocdlbuyb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rkxctqjv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3spzgkbto.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jvewzjjl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wwfiabxe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3neqqqycf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ztkdlzxq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mizralni.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hajwfbiu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hogivztu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jrytkhdb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gfzkmreh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wncqxhxe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kpgwuflc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vrgomckv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ubkecswp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3adpnxjbh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vpvqffyd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hvcardbz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3veewkwkl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3aqkgcsso.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vpkxdneb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wvneaqto.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3klmgdqbe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lknuhfqn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lsvxaniv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mckkaxou.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cyhmuxuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zqreeozx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ziahnqzr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ctmfsiok.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3egwemhys.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fgbqmkok.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ebumkbie.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bymrsrzr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3srqndjpj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qkzbnqwa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3coeiozis.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3apfgolrj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3eazaibdt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3agnywzpy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fvyqtosi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3runigpkl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3agnxshcj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3cvrqxkvj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yfdvgavh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wgqevqqs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hctipzkp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ktqdrbbv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjrjdauc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gtebpgvj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mellzurt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxulvj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3lgahfwib.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3adwamtqi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3trsgmrqk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3asdlzbgv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mcijaqnl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qyuxnnyw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ahdpejyb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hbcyinlj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lnbtlrbd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zfxtvtpv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3udwhzrde.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lungszkr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xbdsvqhb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xxdwuolj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ihyxvkow.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cxilgpwg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3sadkqzag.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sseanxxe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ikubmnit.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qxvlzpqw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fnqkcqcl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qihvrejt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mrynojaz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3aodxanqa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmzuznbk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cjqnmyhm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3blbgtndo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mqlvfjvg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djzghgnv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cwshjvig.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kshhvkfv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fkzvioeb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ixpmvgwg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wjjdyidz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tazjzaub.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3byswsukh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uzcyixxa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wbubuzjz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kkfljywn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brnqrpss.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vzfjsulo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qwsecqro.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lxkhcdwl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mjhunxzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcdymscx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3doplxzrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3girxxkso.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kxluqlob.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mwcneaqr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fdrllqlq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xqrbnawx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3darhinjd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ytccahgm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iqfzfpij.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vaslbihs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oecsujbo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ggkvmucn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3foipwtjw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xnfmdlbd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aswfgjcr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vkiyevug.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wdyfcwok.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cukpzusd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jmhvqgor.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ueeqjwjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tnvwokcr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3atlhpnml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gfrnzdtr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3akjevppj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ydkzcrjy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bkqfbxij.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ygzekjlv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3whgxmpom.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rpwobpyn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwhkjtlz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mwzuqemx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ufnlobyp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wqlelsep.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dmeotfpj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3usytqlxz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oslafpmu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zaloqnha.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uyvtdrxm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vfkdzgyc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ucazfbhg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kxrcsjni.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jntrzvwe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nxykdjrk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zogmbrcf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3znzmdkwm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3szycmxvm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3frnkusuc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rbiiihlg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gqyszwwu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eaxvbqqg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3perufzjf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdbwoeck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gcmthrxg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cdrlufyq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dkesznzu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nzsfuwhl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgkdfrri.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebezymkn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mpnjmlex.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mnexuddp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3psmdkoyp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uxdpyooh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xspjtmiv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcgzivcf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dslfhyne.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ihvjueqo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hvflxjir.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3oejxonyg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qtyjwnks.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3unijqdli.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nftbhins.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3evvmaqbu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3iywfvuhz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3khjkjzyv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lxlnzeon.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zlivujou.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qrggntkj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dodjotqn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gwdshvkz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3irupjtrt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3cbremmgh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mrfbunqm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3yajtollk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zutqgtui.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tyuthjzz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oebhyjrj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3huvwzazv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pumnjohh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3phpxmfqn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3crcfyngk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uoqqwqts.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3edtzvnqj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fcuymmnp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jsvynjtn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3msxafjrv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kknkcbpc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fcllonev.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wukxquix.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hjdmmqad.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3aagcdvqg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddxjppdj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wpecrhcf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cklgcrnf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zfenvvla.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3pqgrldxi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3yfemhbms.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qtafwtcr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lmoamvev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3llebonzs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rzgayumo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sauuvetn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3boyunvyk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wqhrjemq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ophagqcf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3yhzorfhs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ngpakjii.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qjyosdtv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ksynroqa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yfuudtwq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3aicnmoei.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pgvlwpjw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhbsdywo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wbrgzoia.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dajjstsj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cxvbfwpu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yqpoabdb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ooflmrke.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3iacxdeyn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wkkmblzm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3keysfhbs.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jowjjeyk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cmhczflm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mnicnphi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lydyjkze.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gicdmscb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ajwvtges.html


<!-- 参考信息 -->