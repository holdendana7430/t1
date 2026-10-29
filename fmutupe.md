代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gzcmkqwno.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gskwwnxwl.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gnuhgfikf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gsrzeqrry.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gfwruksev.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gpuympydr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/geswiqjbf.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gacmywrnx.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gipcgyhyg.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/goyyixvle.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmnkvvwra.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gvysuvwtw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gukdbgkpb.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gnrvvfwlj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gfdtvkcwf.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gsmzjynai.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gqznvcybu.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gldmznscs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/ganruiovr.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/giisixexv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gepkhmqpd.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gthwjiczo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gqsrtgpbj.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gnanhhyca.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gneasmsgz.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gcetyghws.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gduddpqkm.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gdfeljcyo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gzxyphggr.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gpmycnech.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfseygqkb.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/guyiiproh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwxnzkhvq.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/griezsvyl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfhvfwzca.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gxkoqtdrh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/goxlthixj.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/ggfgvzmxs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/glxdkdqte.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmpvxmwwi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gjnklojbo.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gewljhgrx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvhjeexgw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gppnhmflx.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gohktfhzj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gzjlziiij.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gqcgejxpe.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gmzggtpbj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gaheijhur.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfwrftjfn.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/getkcwqfy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gjjqkhpiu.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gvziefcnc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwdwbhkru.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gyuybuoin.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gwwigvanq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gstuubdbg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gozgtraiq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gejhcfgwe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gmevrifni.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gxocfuvab.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gvqmsgcev.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gxiqexpad.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/glbzqngwj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gsqnitacc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gidnownxv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gteaylphs.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gzjxqrrdz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gfaclxcml.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gcppsavyx.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/grptvonyz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzfahcx.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/goznslrad.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/grtutiblb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gmemgzknw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gphjoikdj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/glfmrxgye.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gmphvpdqb.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gpqurphrv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gmsvgkxhj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gchnvuyyu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gkhwaofso.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/grxqhjhqs.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gqaxspimi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/goeadnuru.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gxjxtpdux.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gutqxxfqf.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gtqnvjhfs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gccvfndpi.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gfybopckl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gnviganqc.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gkrzekixk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gxheuhryr.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/grocqlhno.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gffyxzrza.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/geyeyxaic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gvnxvthmk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/ghxvltrss.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gpgphlcko.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/guwnfbrkx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcucrlwga.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gifhidlkt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gorcnvncn.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gndnqgeqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guuszgcjq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gecvndrit.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gczhdnlqh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvdrdsxyv.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gnyikkbto.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/glzkckyyt.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gccjpizrc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gheandzzk.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gxapvclyz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/ggsmppcxn.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gpxooldot.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gbidntifc.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gwfmpodje.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/grlljiyyu.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gpeyjcumd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gonktxeig.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gpjzowaeb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gryfywiaw.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gvhignxjv.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gfmpyiwib.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gsnfqakxk.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gwlcgqzkh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gobfivdtm.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/geueaktat.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gvwlrlazp.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gtcgftual.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/glipdjjgu.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gryzdutxj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjyarayws.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gtzaeanlp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gmvadgimb.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gderogbnv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gfplytlvj.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gphfhwvze.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdeedigja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gpdhtyhrf.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gxpuzmhav.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/geagpjvdw.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gmtqkxyzr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gebsyfsns.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gwuakcqja.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gmkucteac.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gbrjqfpxp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gsejjgajl.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gxlprcuvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwmesay.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gjgkrboay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gneivuron.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/geshtdcpq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggavpeboj.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gybvukpeq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gkkdzuonj.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gwyrbhxkr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvxlbefab.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/glrguhlcp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gatoiramg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gsamvvloq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gbkupfvog.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gsfixixiq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gxzuakoro.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gmiitagzw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gwwqlpdtp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gwyhkaknk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/guwumgwzb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gzmnamchq.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gouhlxozt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gaougcebx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbeqqhdio.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/giczgdlqs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxebvwdf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/guyeuhlyk.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/grcstovsv.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gvnvhsljs.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gxzupbbvz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gnjvxiask.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gnwrmrkkx.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gbfazjckg.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gfwmpnpdz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gvxdpaeev.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvtnukvel.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gwxfvgwsh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gbcahaxsr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gwfhihizu.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gvhpzspbt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gtvizyrim.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gpxzvjerv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gekjgzilk.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gohwubxxw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/ghdzsoctp.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/giyblloow.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzknyitwz.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gxxeedygv.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gcblzhuhy.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gjxnxdkrg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gfptlaujq.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gjqhzhqzi.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/glljvezfh.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gbeoenliv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gbosgzogi.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gaqtrtggq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gvtjhaxte.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gmsynthuw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glgbugjvh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glyvlvcil.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gkdxbzngr.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gkwrncnre.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gvjpspcxd.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gmynkgcdn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gmbdmfvmg.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ghhadwfyj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gddvsylqm.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/ghdyroqcf.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/guelnnjpz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gnbiluwoj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gixgxbxlp.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gdsxgvdre.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/guajqncmv.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gkjzwpddb.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gllbfupbu.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gqoyesuhv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gypssgdyb.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gkzpqtmnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/guddwvtgg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/garvzgimv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gzzojcuyk.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ggpnxqxbi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gnpnntsat.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gcdtfzvuq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gixquejbe.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/ghbnxcxla.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gasngvccn.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gprjrtlus.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gohfqkibm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjghgahdw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gjykwpugr.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gcrlzwpau.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gmvkgoeeq.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gzdplbtzy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gzyhyrlwb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gvybvbcll.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gxsmvbrkg.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/grbmxeagx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gsusawujk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gpwioseen.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/ggrsdpiaw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gwhxmbbfo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gdqkjgnjd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gzyetmnoj.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gzeacdyzj.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/geguxwfwd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/guskxxdpn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gmqprsjqe.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/grqocdvtu.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gfstqewek.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/ggeywnucx.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/glcqbslyj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gwanmdzzt.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/ghztslnjz.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/grhmggnux.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gkdbmvrje.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/ggqsdmoin.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/guhwhufye.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gsfutbjph.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gabizdctg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gsodwjbmh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/goevxpqgp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gtsivoebb.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/grvtvxjhl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjocsjbwb.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gnwggcpmo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gdcfeairf.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gowgoyacb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gliispbjd.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gndtoqqrl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gbopxydhu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gufqdeioo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/guptqlqgp.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gfpvtfjww.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gaowhigcd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gjuvcloff.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/glltgmhkc.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gknsxuvzy.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/grhkifjqh.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/goofxwxuv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gxiteowzc.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gxpxkkrfw.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gjlyjmzam.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gfqozuwui.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gibwrevnk.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvefdgqlo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/ghsqmjgtz.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gxenlyxom.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gtneuaewm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gclddafff.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gychrhgos.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gtmmzjbqx.sHtML


<!-- 参考信息 -->