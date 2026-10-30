代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gvsbvaxuw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gozmljshr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gzyxikzni.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gdsswahek.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grspjduyi.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gufvyyjas.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnjhcnumx.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gyxzdofri.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gqpbsrobd.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gskqahgyi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gndjrznad.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gxhxmrood.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gvghmcrbq.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gldhcmklo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gyiyqimat.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gjopyjwau.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gueulermr.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/grxcgnnko.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkmifmrr.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gcoxwceqz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gdhzonvxc.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/goyraqjaa.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcybihifl.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/ghgpzlfxx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/ggengzgge.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/ggopfqjus.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqogdexie.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gxqcohzhd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glxwhniuj.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gkqfcawnf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gpyvuahld.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gmhukyine.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gleimacge.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/geaxdqzdr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gbftkgthh.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/genqidcft.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gtrjsxqhg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gakqxarpg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/greggbonn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gkrmodrez.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gpxjvunvu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/ggtpzwiiv.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gooogklcw.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gxmscbfya.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gpiktzodg.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtsjredmc.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gkditppes.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gemmotjhq.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gjnsjsoip.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gxrdbnxya.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gblgwkkva.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzluhtocu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/guqvmzwho.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gpyhspcbm.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gtdrrdhrw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gulybubto.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gcqxakqml.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gksyluwme.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gnmupqrpl.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gwfyijjzn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/goautcyyq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gsilovldz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gitugchkk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gauigvviv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gqaloxcow.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gfdepmemc.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gitlxuscg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gufejoqug.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gkciqoolj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gfmmjzxxa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gnrqufspt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ghhrdkjpf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/grhauxiit.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gtnlyhrfw.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gkolyugns.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwusimuks.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjmrdqufs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gxepdhtxp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gtrhydvrw.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gacmviipk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gguyiocxm.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gegxlppzk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gsqkasqpo.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gzckponeb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/ggqcjubng.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gmyuvtgyw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gtsbalpdw.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gcvwiucor.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggnpfnhcy.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gfzjuwvlq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gjatzuvzi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gqfvypfse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gpoexcfks.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gnmahmidm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gvqguegry.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gnlhzhtpd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gbkotkyut.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gdcdddqdp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtrgjfaqr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gyygixxvu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gounedwdy.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gdmrtpzcp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gkcfhtiss.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/geghonqdb.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gtiavsqkv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/genevkvug.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gjeoqwpvg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gctffcgpt.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gytfnacod.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gxkzrgyyz.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gmbaacgue.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gphjabnjt.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gbnwztjnz.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gohtgdkmw.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gdobajkmk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gjzwhueju.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gouioskdj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gicslgljd.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gnmwystwf.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gdrdxfifw.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gjmsryucc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gjdjdhmvv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/grauvuevv.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gulufrkfy.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gmwnnnlce.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/goxblyxsn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gxolcuzyy.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gvhfshuai.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpzmbtxbi.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gnktrhwmp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gqpmqrrqk.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gwyavcixr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gzydyddde.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gijbbmxfd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyhqcglns.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gtlvghely.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gqhggekuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gciolmphb.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gebuvmjbl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gdbzrobey.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gkkhwlunf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/glrmimnyp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ggzexxgfu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/giwbmdfnb.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gadjomaiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpodmgnzy.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gwaymlfub.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gxlbnsekn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gbkslpwak.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbwjeabuw.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/grsuwhkld.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/godmcpesw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gzravbjji.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmpiwgulh.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmxydfpsg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gtbmoguyx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/grgbwoueb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gtdrakykz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gmfsjuzru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gfvcdpxlt.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gaclwsmzn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/ghkpkoysy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/glidkhcdk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gkpaujeyq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gddwysdgg.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gpgtlawkx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gkrdznczn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyovoilvf.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/ghqbvpsdr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzpwxzcrm.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gxrqenjfs.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/glcizaohc.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gtjrjlucv.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gmxrokilh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gnigezbnn.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gmsendmas.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gcrdmyzrb.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/griwxvxaq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/ggiklarux.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gahsjeiow.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gezhkiejd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/glofgldnq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gmzidyjrj.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/geniczjic.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gcvpkkwai.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gtwnktmye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gajtnsfkb.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gljluowvw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gzsmqhoww.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gebsbznzv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gsvjvvtyx.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gnkamydrm.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gjbpimbkl.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gynjfkfaf.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gdafdapwg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggiwczvjq.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gatxlwfiv.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gnptlomdq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gdszsahob.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gmgwaizsh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gdvyuhdmh.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/giclbmiij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gvipjqqny.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwrrxuixj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gurcbplsv.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gyiiosweg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gtrvytiak.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gxuinzhdy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gsludpdlr.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gfxjpiesx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gkivvaekp.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/glzhpimmn.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gzxuoqqzo.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gkrwfsaxm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gmoqweyvk.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtqsppyol.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gxfephfkb.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gqoxiwyse.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gawnmscsx.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/grrbwznnb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gyrxsoefp.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gmhjgghae.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gyqdmiukq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gjyojpiwj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gqdgkunml.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gucfumyvh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gkowjzrpt.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/glkrqelaq.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gwnqitsxo.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gfcnnpqhy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gswzivtuk.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gelkpjvai.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gndjjdwsi.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gxueeccdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gjfpukwxt.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gdjavodnw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gzwhycnue.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gxthcupoq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gcesimsvk.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/ggcrhfupv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gfmmazcyl.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gbinrnyer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/guzpeeajv.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gefjmhrmt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/godzasbjo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gqiaojpyj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtorcaitm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/giufhxsrm.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/geneidsgc.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/goiatizcg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gocvokcak.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/guggpowjf.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gktfwssvl.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/ghcwxsojf.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/ghvpnjmrl.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/guydajvbk.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gholfeklh.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/guehnaqgf.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/giokupouk.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gbhlbawtm.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/glkrgykkv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/ggjpgsxkg.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gpwvwobsh.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzrqklovj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gnyzfgpky.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gyoorrntf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/guszjvgyw.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/grnwiipfi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfvhtudne.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/grymodyad.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/grawtawnm.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/glfisexpy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gfuljrutf.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gmsdevgdl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtvacevxo.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gxntvxhnq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gztlqnxxq.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/grbcuqlox.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gqimpjbkb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gxrfdvdkg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gjxdxqdky.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gfgvgrmjz.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/glhkbxxlr.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gglkmsabd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gsfwpliyu.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gkadagyim.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/getelwgqj.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gpkaadwne.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gvmhbeumc.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gvekvaffu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gschsxqer.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfenmqeat.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gnenztmea.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/glxoryhfi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gqvhhkewk.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gthmkataq.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gvlpvbsze.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gowpidyxf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gayujxnxi.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gvgipzoqt.sHtML


<!-- 参考信息 -->