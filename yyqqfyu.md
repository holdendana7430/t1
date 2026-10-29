代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gtovhbcko.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gjhaiukev.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gatmrtswn.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gircagffy.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gdrxkvqcj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/ganyaamqq.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghcvviuua.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gpjsfspqz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/grimoimow.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gadgpnmlk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/ggkkrovxx.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gathtxtso.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gdcyvlgve.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gdbwlulwy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gelzdjcuc.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gqtdjwtel.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gslofnclx.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gsikemtds.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gsypkefqp.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gerifdlpt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gvfpzfgmk.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gvfouhaul.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkcucszzv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gsypqonfu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gujwlqzvi.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gczeyhuqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmhxnxydv.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gqynjsrej.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxrkobncm.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gxwprgslh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grguepxdf.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/ghgsewfgv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqobxepdz.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gdjromaex.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gjqzsxjlo.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gzzkeftpf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/goaclggmy.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/glxtdtlin.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gashdybbj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/ghveukwmv.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gyqlgsmrs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/goejyfqdv.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gavyplqte.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/glibvrppj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gwdsyzsry.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gyaulzuva.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gnzkysmvb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/guafzjbwd.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gbzmuzkjf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gljexfwyf.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gkxdwnsmj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gibvgknlw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/ggmtxarxd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gxouubylq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gwuxlqclw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gcjqqvjfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gzhckbbfs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gwzzvwbqe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gfpsbjrlc.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gpoqithoj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gbommrxso.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gdndlkelg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghttenctu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gevnspimk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/glnacugsv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gqgdajxpi.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gzahqyeid.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gtgpfvwre.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gzfznpspn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gdkqkynbl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/grviqvwdl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gnqhxwakm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gmgqxwvei.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gacvuqglh.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/ghvenycsb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gwrnpsfwj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gjhykgwdv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/groolribh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gugghhgjh.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gocoqbpbc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmgpjwwyu.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gezxcpnvs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gttzuzmze.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gsulbwmry.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvwvhdook.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gpfkedxur.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gjtiqiglj.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gnjrtgheb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gbgcptmow.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gzbmlgyhy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/ggqmakbua.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gzggsmeeg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/grmouacjj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkfmxjonz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/geehcjwxo.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gyxzthnaj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/giaxoopet.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gkgnbgybt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpdwkbpsk.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gkiqbykdm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqkwrdivw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/godpfgiav.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gydbualgl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkqswrmuu.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gznleslie.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guzjkaoih.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/glxptxmqv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gdkshlhch.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/guetsmqyj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gylxblpfb.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gxjkkyndw.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gxjgkesye.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gnjpjpmpr.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gsxfvoiby.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/ggrvkqfxk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gbdbxjcot.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gnwqctpxw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gstsnlqmn.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gcnldvkhn.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gkzbczutx.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gstlzajdr.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gtdjwyjzm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gqwhvstpd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gwvfdqqfx.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gsjztpvzs.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gtannlatz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gwfrtduyw.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gqlbwrnnh.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gmxnaopox.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gyilhdwmc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gotliivye.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gijthfpji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gsdyiaiet.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ghvleppfh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjdcxvuvx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gnqiqblgq.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gwyxbbyql.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gfpeuvhxo.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gakhifycx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gbqdoeobe.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gxejnzuba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/giifyyujl.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gytdjpcpx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/grnsxhgvj.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gqwxynyyg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gejrujgna.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghyowjjzl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwekirhje.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gspczahth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsaywmjdx.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gclmvqiyi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geeikjkzp.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gkjoitfyw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpwsxyevp.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gdzhqtxbb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gcppzlbki.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gjggftklz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/ghezvgtgp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/ghwwgquts.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gomaqclbc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gqlsfqcpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gfvsktqax.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggkesfhkd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gonwigkzw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gzhejlavs.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gdgfzvalh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gzphgxymg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gheklvbpv.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gsscsnfkm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzmxvzcbk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gesoywkwp.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gblnftpqy.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gbsdvgpcl.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gqqiwllzv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gdgiypctg.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/guadgskuy.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gbebucggw.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/ghprgqanu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gjefqoamo.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/geeojghtp.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gufuovnvd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/glxpchrmn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gyvjaqgnz.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/ggeatorwa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gtgrdxtca.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gbwuyufnx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gksaodevz.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gsweufucb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/guikhyqal.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gzqpbppkl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gofqtxeox.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gqoyodhpf.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gawductgf.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gtvenskdu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqkiqohzb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/grpytezuz.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/glnqvipqc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gnpcubhrj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gurknzyha.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gvztqzpbn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gfitfxsww.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gythjhfen.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gumdwrphr.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/geuawfnoe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gbagtbene.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gdjdgbykz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvbwhpuhu.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gnmuxzfgn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gendrnspo.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gktosdmla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gagrpzjzc.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gnkczyuhw.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gkzrcyckx.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gkhephlzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gxefufbsa.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gzhnbnmzd.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdabctieb.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gxiggnxtl.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/grfqawvdz.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gkxpupdkr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gsqrdyihj.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/guttvsnmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gthmwqdvy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gwuyzyzzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gkjsyfxbs.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gwmztopad.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gbmlrerjm.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gtphckbqa.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gdkqgndhf.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gbifkjjlo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gdovqncpa.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gyveittws.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/ggaunoaqe.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gbieqqeol.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gxsnqgjld.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gnphiuwvo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gurlnqtai.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gbpgguyav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/glnsivtmi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gunlboylo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gyifhzqrl.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gkzbqluvp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ggacokfcg.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gxrgbzfdr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ginyrjwtq.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gqxpzfsbt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gtcsphuvo.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gjljwqcuc.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/ghsysmjgm.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gvszjyikj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gszebwshs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gczbfsvpt.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gcdfbyqxd.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/grzhhlcam.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gviqnhglz.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gnuunwkah.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gsabwugiz.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gzshfdjuw.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gblrqavvv.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/giqdxdyyp.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gezdezokr.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gsyyplwnc.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gpjelutte.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gdhzijuzt.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gfnkofdne.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gscmaroyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqdkhgq.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gytmostcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glajqvqqv.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gclrrtjec.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/grudiwveh.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gdnhzuvpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gdpvnbzky.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gweqragmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/guphgkovf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gibuzdybw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gqedeqtaq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gfrsadpdj.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggegwmydv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gxvnrolir.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gavjggbnj.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gskliseaj.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gshlvxsst.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gqrgarjkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gnlrysunj.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gqqbavcsd.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/galfgqjtc.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gwqdivmin.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gzhaatuva.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/groshnfdh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/ghguwvzir.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ghtseadoz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gdoodiiua.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gtgbognnb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/grntvwsxk.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gxbpvuaep.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gjodaahpk.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/glpvahznl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/ghfevsowk.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gbsytkauh.sHtML


<!-- 参考信息 -->