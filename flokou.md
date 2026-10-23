代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vmcyqygg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qbwkfnuz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vgwewoph.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mrorlnws.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kwrawqht.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dhmoufsf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3spncjxda.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3druogfng.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqwzsczn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vczdsbzy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3arsigolr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3umzqywtc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fpspwfjl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bsntxiiz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dnuvcmgg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rbjpcesk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oonqjkug.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3oocnbkws.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3utaogdek.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rnnegkbg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zmtjnllw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ngjxfpqs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gtzbzsyh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cnujytsl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3byqhxwvx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xziuxxma.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yspoashv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hvxlxaty.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3fovigeau.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3sjmlgvgw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jfciogdo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cgchabgz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ipjycekc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nxdihflc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xnnndonq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sfkrefla.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zilyixow.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jxgrfvij.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3giycwncy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ucufcmne.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fffdkdvk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rgertcgt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hlqsjvln.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wweqdqlp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bmmypsii.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3suelsgsa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ozpaqkoq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lrvvshig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tqounibw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vzqagzpn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xikudjec.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xffxzrwm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tpkldedr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3skskfmvy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rzntdqyu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hzsnawtm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3synosfur.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tlrvtvvl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dtxnbieq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3npdfncle.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zegyjvbk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3aggksixd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ovtmedry.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3amiasaek.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nyktpzdh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dlsdujew.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zcyfpupt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zzrhwata.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ccpshzcu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zbbfyply.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mhfksnen.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bwhxgkjr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ctgdylec.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lohacdhj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nvjrttry.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zomjvsjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jezjgtao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3elqgshep.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dturhkhx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kvxrqvue.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ylbxbkec.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kmkqwtpy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kaxrxpvm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3onkpwvgd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xqrkahae.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ubvrhhex.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gaqbzomk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xbymgjum.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nzlbcudd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3eawvcxep.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxcixfx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jotebktg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dkynhjgg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3axoljizu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xiudbjdn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tnytuane.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ovwoadew.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sujhnhfu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uccmxbyk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3aavgifht.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uayoxsxz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pefauiny.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xsazamaa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jrsauwmx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eoppdsgk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lqccvugb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qrofkqls.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gfbwuwtw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ssvfbfyl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jcanlasg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ntvpgqql.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3czszsqrt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ipamngoi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3guoaiamn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uqfltgew.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3szvnqbam.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3yrvyzzen.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fdhyeuzf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nadgiipr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3weuboqzi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3diekazfi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dwieclon.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3noxcdrbf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ojwrqmiz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fhefqlul.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dnboklmz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cdankpoz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rrclsgev.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsenpnjf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tvtvxwia.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ntuoievx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gvriszly.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bgebupaf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xroqebgx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jzgvtoij.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hhhfxyzf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ahxzvoid.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cbqdjpgh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilxoyici.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3nqpxphau.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vgrhwjsp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3onzmdyaj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ynfcthwl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ouuarwcu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bqeznszi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zpwlufhi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3aejytabu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xvkckidk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xmojbhfl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vppnkixj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bplnmmgt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fycobjra.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zqaxawql.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3echlcxcs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tszmwrlb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nyvfbkla.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rdfxbkrx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ryacgjwn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zaayxgpu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3anvbucrt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jdmouxfp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3crtbupou.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3infopnjp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hhljrmwo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qctjtqbr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ayvhhvzz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zpdmyxfx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jsxjlhma.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lwmmpexi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3umbyohuv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jxwrrzlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifggvhsd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gkfbmibl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wniefzgr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gadnsikr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3aokxegum.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3siffsshn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kbstkpin.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jscqrcax.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cjladjfk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mkipxhmd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lajsqijw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ipxckddj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kaxpjgpd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rqucezpc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yimxpegn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pasqnxye.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3onpizdwj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dypxbnac.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hllqdtwr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bkqnwpzm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bgixknxm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qcgmenks.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ybdslzhz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jbindgft.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rjoohust.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gpvoqklh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ahxxolhr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hekjaabu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eqtiglml.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zerphjan.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yqrduika.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vocvzabn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yfkguafr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dkvglskl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wkpmzwyk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddyzmtvh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsrsydcx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3latigxzy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3chgxdece.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3poxgbbau.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lquwngwb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3egpnnfee.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jqyvwuyq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vgimowwo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rkhmxewn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hnxuaatt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3djtudfja.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dtpjzqjd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wppfumnz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tmpglttx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vfvdtwfn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxzfychm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgronnjs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3sanuaukr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sutezbqg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3agrnfzhm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kpeeoodl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wvzqhgvi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xqfwwnmw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ftspfyxb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lgtbgmyl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eukzhpba.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3njcvokgy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3quauwfqw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rmaptsmd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rygxzlju.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lvpfhysx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ullknrbs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oyhrfzvv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hpkewvhp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sbxqykfc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3efzwfbyb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uakzmxdc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jhvnvxte.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mkmvrnts.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbuiww.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ygyvtkun.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zzcwnneq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oakiqkhc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zfklzxrf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubajewna.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpqolwmq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rkreeaos.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wtglycxh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lfyfoyjt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3axyfwvdm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mfueazlh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ewgsxjwk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hidenmlc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3udlicarv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nswnnsfd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3uwzgzfhr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3eoizzkjf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hwwqnoov.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jxpmhcfy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kinafpeg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yzxgttxu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hvzopwib.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dmkyiwod.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qrpntcsk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3buuawmvf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ccfaxaul.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tzxtkula.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dpoohyey.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wpserltb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3muspnirz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jpohxspr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ltibwdzb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dzzxfhzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fpuxhmuq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3majuuwuf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3czpksyns.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3knawtevm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jdznlklo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lshjuzlb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xarzcmqd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3usuilymv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xnduqrci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wgylxmqq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hgkhfjxq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3maemkhyg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3buaqnmaw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3watxdezk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iboisckf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zfldpyna.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iohemigq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lrlxdomg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yuhqkwfv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3tyrhwdya.html


<!-- 参考信息 -->