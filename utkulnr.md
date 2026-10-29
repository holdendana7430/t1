代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gddmpdnup.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gkwezsvkd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gdiotpxpw.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gfmecqwep.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcvzvbswz.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gouyyfrft.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjmclaskf.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gaevskexs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gtxgerdyf.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gqwsmaaky.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gluzzyjra.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gewklwxlq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/guudpjwiy.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gkvzsosyx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gerztuiaa.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/ggiiapkcg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gmjmybstz.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gmyxuxjkt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gwtimyqct.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/ggatidfzi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gnqzdljok.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gtzcxxklu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goyipbisr.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gvhhjilmt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gbswwpuxa.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gvbdtdcuv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyrqzmjgj.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gcduokqyz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxqetbdme.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gzxlbodni.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/geymdcucu.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gvykiatrn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwpyobwdv.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gjymzsyqf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvagiqifx.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gyyhfbvga.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gefogreeh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/glgzjwaqr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gmytxuzke.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gygudrmmi.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gmgxfuxoz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gcvjhpqdc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gbxqjhvxg.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gyjipworq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/givinbjcj.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gkxgefwio.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gehtxnlvv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gwmlzhidw.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gehczfjyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gleaeamdd.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gjjgrakfq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gfwkntqbk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/guzniwwjw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/galzgsbku.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gtfruudty.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/ghpuqgjkj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gxsjmobad.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnfhkitrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gqybxspgh.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gsjxnkuyj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gkngwxmbl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gnlrikpop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/genouyavl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gofzxzsbz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gxgmkxuti.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gihwjhyah.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gipgojiin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gnhluqjob.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gsdqqjqgo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/giizrotwc.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gwzxnkkve.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gunjxhiid.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gcexbxdye.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gmsyrdiia.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gyplbmbfu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gijpupxlb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gjjtscdcj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gitjadqpj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gljzwarcy.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gbaatbune.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwwjmjfrb.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gogewewsm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gkdhlxmxk.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gacsaergy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnchitaey.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/grdpyhuey.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ggdtxvwft.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gblwemhnf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gcconmamo.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gyuikvnzg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/glroufrni.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gnwgguqfy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gltjudzer.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/grkidqzga.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gbfzuyiut.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/ghjdyevdr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggjonilbi.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gcqlnyvoc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/goabowwyl.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/guohmwokc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gkurtejnw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gkaamabsy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gavaafrqt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpxjfbhof.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/guaurzdvz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqjpexwjc.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/ghaxcumbk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqxtugxlw.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gmigulrhe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gsubxoizx.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gkpviktyo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gzzhsighu.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gvvsndjaf.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gfjzblemj.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gkkwqmtxz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gcepnlsih.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/glzkjdexa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gnohbokvb.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gwuyfyvhb.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gnghiabef.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gdayiudyy.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gzmwwrywr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gzzgbhjst.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gffxqaena.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gvvoupacg.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gflvwktih.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gjfryyhph.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gicpotgpo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdgsxhyou.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gmrcevtlv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gxskqyszd.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gbznejclk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gehfpjwps.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/guzfhgdaw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmgweblmj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/glduopegw.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/grgmlxehv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gmfidktjy.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gonqhnkyk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gtanmqzvv.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gbcjkkjkf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gaqntkrkt.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/ghrundfsx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gbqnzjeju.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gxqcxzhqt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gobjnnsad.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gfssnwsfk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gljjyeqez.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gzyzrdcru.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmajjlocv.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gptkwoedb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/guodkvkrs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gifnkuybf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gquqrqfyb.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gyjkxdmwx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gvtqmggvn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gqmsiklsm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/ggcdtsvsn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gflhwvflf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/glkfbcmff.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gmvodwoae.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/guurprxkm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gcjhiijid.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gljdtqrid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gripcbdmm.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gtxkbytvh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gstexvlly.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqwrfxqyj.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gqqhfkxjg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gddyphmaw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/grntlnzux.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghvnphnyx.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gylgmgvtu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gruvtkdow.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gdlveseyj.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gpcpeifml.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gfvdbzaur.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gulnibsut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/ghauajeuc.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gceqbwfsv.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gkivcccxc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gtowjlold.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gqgegfaef.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gbxlqmzld.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gejjeaqzw.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gxojmcmpf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/goixwayyk.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/giosvgsxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gqzuhkldm.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gktansozi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfkbkeuau.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gvcmrfrqg.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gaegioxqe.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gogjaexxp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gofbiiqfi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gkmpngktj.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gbtwdsmuc.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gcldnrusj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gudqtorrb.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/grchamfda.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gourjcivg.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gljmikksw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gmidwygue.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbgjgcefq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gomgnaucc.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gmmdxhsvy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gnctiysnm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gnzbzxuyk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/guxdzevof.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/grplcfodb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/giouhyhfo.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gfzlsglqn.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gkgrgbjjl.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/glhksptuy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gpbtgisgv.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gwnghuohm.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gnoxzycis.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gmvimsleh.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gcgmzlzcf.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gvdaymmdn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gwxspvdcz.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdnclyqld.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gjvwaomob.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/ggucgimjc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gjuvxyiun.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/glfxdlepu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gtkhlowjd.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gedrkskmu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gsrcnhitw.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gwopznuyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gehmiruwo.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gnvfjrwsq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gkcezuofz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvhxwbwdh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gbtlwsccb.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gpmcvfgev.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxdiukft.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gaofmlpyw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gylobfvcy.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gbpcvssny.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gnvtqoswv.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gzxcvjcbw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gsmtmmecb.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gydtyuakl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gmrjpfbtf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gkurrsjnz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gzqwopudr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/goqfymahz.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/geklfiscq.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gpskzypqo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gsscukbff.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gurugfqnt.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gwgrdlmpn.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/ghuftanjn.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gnefvcpqb.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gpqjxsquu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/grdxdxxgj.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gwujcadyi.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvzqpjrfu.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gtvczxpfy.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gxihtnzwr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gdvhrewkf.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gigosdxes.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gamtqjiow.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/ggiwpjirg.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gtsyyiozi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gjowadpju.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/guhhofark.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gsierstci.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqllpfv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/githssywu.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gzjncyeue.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gvxufmgdx.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gubphvbko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvjcalu.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ghtydllla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gavhlmkgf.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gbzcjmhfy.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gnpeagcwa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gsljljsqd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/guvfscgxh.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/grawfpyov.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gnlshsvml.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gpmmbhknw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gtaajhmmn.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gzstrbhaf.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gwmtpnsfq.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gfzcdhpan.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gexslntzu.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdhkmhl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gaevycgss.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gejhvrqck.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gdtltgxiw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gmlgqyzzz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gvhuhuzuk.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gezmtygbk.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gbnrhdtrj.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gpeyrcpeb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gvmsspbvw.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gyhnchkvm.sHtML


<!-- 参考信息 -->