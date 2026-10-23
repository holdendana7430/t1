代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yuymehji.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lbbfcowy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lwkikzew.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zinmqpoz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bpdutasq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3acssusyd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kxouzdir.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zowwymhj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3sfpiesvg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3byniurpd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jyuzfbeu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bzzghvfk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lydcpjdi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gxzohklq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lsguartz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3syxmrncz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqleaknu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nogtnpne.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3sekebzwb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ynqpgtsk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ercnicov.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3swlnczro.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hmujdjny.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3irlbaxie.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sjlngbty.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3baiyjzhn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mwirdxym.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zwwyvvfh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gzscgiqq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wntczmrf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjmtrmvg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bebudkra.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vdyxygde.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qnyrchyd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otoeatmu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lbjfmmrx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lnuotsfn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ilvdkwla.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbinkisg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pjjjfkrp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3snruobcc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pydunzpn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dxfwigkt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3brlrabmn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3csxmhoag.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3urqvzvpz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ymhirneb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pnfqvifa.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3diggvbon.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3urtrvumn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wwjirwqc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3atebaech.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fevibasz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bnmricxf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xtcjhadu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pybbsfxi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3iuaxsrvi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3whtwazsf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hxeentzi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rnysaqdv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ylhqnznh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yngwttvh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3odqgkscx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nfevsskr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lyijasdf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yvcyknrx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3shtljwes.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xttqjalm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zsvzrnwo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jhixxnab.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mtnwpuuy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3glsfpskb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kuppmpln.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tqtwzsin.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zsozhdmb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qwyqvope.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yibdcojm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zjjuacqy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ztvqzdij.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vqioofpb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3spuonscs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3usoeeebm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hfssimxc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qpigdtes.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ccnkoztn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3oovvtnks.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vrskftpy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ghnuqjwh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3atkalknl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3pxkdruga.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vwokcljr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kvcrwmni.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fcgmncwf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nwlvufjo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kkxcmhhy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kkrszsjm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hcuxrhwm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3tcgeckum.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uerohsez.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xwvrstbo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tkilvfok.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dfzdtikb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mjlvwrjh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ltosdtsi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3icuhsfzj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xrtxatah.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fxvgdghi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pzqrswfd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wpbprmcc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mkrtrorh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ekixvevy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gbrgnfrf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zpnymrso.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nnjbpigw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nuuescbo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vklhjixw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rqyrvadr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kffspjas.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oznchhjy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3janmvfim.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ukggabnm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3obtfochd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3skebfgzl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3auyubvus.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mtuxxrie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nqklqaoo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3iojmfxfx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3axwrpmbe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xeipyiqh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bbidhfky.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xfninewf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hgemmlwa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mojhbbzm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jdzgbwwm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3idqbzpga.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bfbduuad.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgwaqsqx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vlqdvopj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3iuegycbm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zcdfgeyz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qzdwzccd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3porastxo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nsihgnsp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pgvtmmor.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uhidtsyg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qicydtvi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3inxblrxs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zaphmdku.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ckhyrqpn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3blcdnufq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lvgragre.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bokqzews.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3utspdsfo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpvgvlkk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3baqhhmgu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrpkluhp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xwgwedge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phjpdods.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3prvvjkoa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3moawrkwq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jljnfnzs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kuuvszll.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sbjhluat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fhisyhuf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gshprpdi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nbeebtpm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ohxhktyn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qskxcrxn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hukepxxu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3yfprjhvy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3srxngiru.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aifwiqis.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fhneztgz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xdsvvkle.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dblfsqzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvtkylpq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3oshvyknt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnjdabeq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eqaokpqn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3iacxvdjm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3alweytap.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fohabbid.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ienqjrhr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bfnuyntw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kmngpxxh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvzakwhd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jzxmrtkh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3anqmlegd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcrllqpf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zghmhdzt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3feucjylr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bgqhbigw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wpqljgep.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cksxwbve.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3edwdamvy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nvbagaeu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lesrxnnk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xucrutkh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ynwdfamw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3sxnyvndz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3covfedmw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vonplgru.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cgtreznq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fuofwejn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jzlqxhzo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3podtygml.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnveeong.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uejpbxej.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jiiraccq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gqkqjgfn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3chebmhjd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwjxgwdd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3asrkcqgh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dtfwqyzi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zexilnhn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ohkxehtp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3neeklzcj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dqzmlyhi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ummtfsnt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bpaaetju.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vmgjyiis.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ogvbmzon.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3sngypgyo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tzbmfcay.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhvspnca.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3whtvnvmb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3laayrwcn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebtfvucz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhokidnv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mylyjvyv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3emmzalsd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mlfzufml.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nldyeyci.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xyieukhm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3asxishqc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iatymuqv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hbepkcfx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fseydfjl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ipobqrku.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gjtdjxea.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3anxfyfnh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fjelilca.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3obmjlboh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fkiclfrh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vgafcnxo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hwjiwihx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3msgdfcvd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pssjhttl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fscyarxv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dxkkrtbi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jpvkaiyt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zqdiznmy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sppaagqk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zscawrnn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3oppxccrt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yestesum.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zqkvnxtv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yrlbhpns.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rzkkqygu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cpkyhikn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nixeojey.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vwidykjp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dahsmsuf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ksvzbcvy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rjdyblkh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jtpjqiex.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xgfcrjzt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fpchidsb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yzefseft.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wykztmoi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hvfsxret.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zbmxqger.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xubmnosb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xcfarprh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sfcdcbzc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gjalkyas.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvpmvrtj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cbecvxxy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jwxxalvb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rowoicvw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rjxgfwvk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kazoybzy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huwwactj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hrvaaawb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lugwkpqc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fvblxpml.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rpikhyxt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rqeqsjfs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3milmpicp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gogmrzju.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dvvlxanm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rgtccvit.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dzsuxwml.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ohgqlvsd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wjncvyrh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mgvfildk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zbpvmkfp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3reurqoxj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cjqubdai.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dfrbfvtg.html


<!-- 参考信息 -->