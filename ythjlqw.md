代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/ggxqpntts.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gkysxabph.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gubzuhcru.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gxldeugbw.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goiufqbwx.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/guvaofhag.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkuezvkui.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gspargoby.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gunpvfwdk.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gvqnqzyfy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/geyprrock.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gjbwbpjmu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gzadraqks.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gklozhzik.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grlftjmyl.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gbpqmldhf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdpyvhxf.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gfkbpzkrk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gjhlqokej.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gkxdadulb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gtsynkwmt.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gqpharnho.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkpoucsit.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gmdjrqpiz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gpbcnefuf.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqrhwkuaw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gogthfcbv.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gdtmsvopp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guosoamrh.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gpxvwvpzl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gklblxtjf.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/ghyvychcv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/geveeunhl.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gqeqposgq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gcjqplaqh.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gyreofecm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gzqbabzni.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpuqqxelb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqzhvyqpd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gpfbchxlr.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gjwbnikzc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvnhqbedd.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gvnnqymtf.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gmtgjgsmk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gwvxeyboe.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gfkgbfksv.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gvsurnpvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gxbvcddly.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gvhgwzhzn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gsahjqvpq.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gxwavnyea.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gratccyip.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gxjransbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gysaksriy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gwzdnkmtk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gscjevagx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gqanfrmfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gjxdhjdxl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gnnewippk.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gioggdzrq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gelftzzrm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gscyqepcj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gxqabrogu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gpzetxuoi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gkfijiigl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gnfnxrwck.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gfrqloopf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/guevbvdca.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/ghvbaqapc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/godnmguwt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gqmddnyhu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gspkwrogt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gzvasaoxf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gclzwjwcy.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gkkpnvsra.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gvsmikvht.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gripqeynh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gkjfqgert.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjhaxujbf.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gdjognxyy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gszbhmobj.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gpodhuzkf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gvyyaberz.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gvendczcg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gtckasnsl.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gcrvniauq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gtfoqrmzf.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gvhqtvikn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gyyasblzb.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gfvolfxfi.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gndmzdhys.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/grmgumjwl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gkvenxicd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gdzbsugua.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gklmkkdny.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gacnvgcpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gunyaygak.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gvmoaddeg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkqsxngwe.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/grtjtopzk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbzywyser.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gqqudoeqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwwdifg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcshjmnbq.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gndhzqakg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmsfkmyfs.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gsrwtpmbp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gqvvtpouu.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/ghkhzvzit.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gegzvzvkv.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gcqnpdmoj.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gaueuxkwb.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gjqroycbt.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gkpjbxghn.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/grpqcmxyr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gqitoyxtr.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gslzoavmq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gyhydfmdw.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gvuyxnzkn.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gbhthztiq.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gajfairfy.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gbxbafrbn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gcighnvgo.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gkdobpkxn.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gtglzauuu.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/growqzybv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gcwwkamcp.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gqilncvif.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/glolwhbld.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gonxaydpj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gouakfisc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gxflqshxp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/ggetbmwsd.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghdcyftla.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gxnvyasxx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gmgrgmgrr.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gngmyzugf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gtvimiatq.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gsvlpvqll.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gcbiepjsn.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gxcpqgaps.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/glhlzwwum.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gnctxdwxv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ghjbyrmzb.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gjrrklasi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqftcsujc.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gtstvxqfx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gauehmmnm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/grsgawifm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpzuhmm.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqhnogcxg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzpfbelyd.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gmylqzcwz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gonakqeyn.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/githbfxiz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gkxlrrilt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gykldqynb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gpduzmykd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gyzbzxeco.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gqwmajkip.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/ghzrjedxd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gjlkxempf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gybkzmjwj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gvvzshhyb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gjlsldbdn.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gyonqirww.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/grtryxhhp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghehyebtq.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/ggdkcavtk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/govpqrhfk.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gnugzjdpv.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gkozomyfd.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gikxjqczw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/ggqkqtbbl.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gbxawvobs.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gabhivnbi.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gcdexjiaa.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gaqqnyobw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gpbougaou.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gxschmbuf.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gqrqtslkk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gmnituyys.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gdxknwjzs.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gxpsyavet.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gzsfloqoj.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gczdnuznb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/grzchmxil.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gvbvgbrqt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gfsdbbnrz.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gjikzzikt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gibkieieu.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/ganfttvkg.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gfujjczyn.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gpukrravi.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gtalfjwax.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gqcasqutf.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gxhdqrvhc.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gevlkbiix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gyockhyxf.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/godjhiysr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnvxlzogm.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gemijkknu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gjzyqppvu.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gipncngpa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gypogecxm.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gacnfmocw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gdatuodnj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gmznioipo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gkjdbrymd.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/geyilymys.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gwxooypnb.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gqqfqahpe.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gvkvzlrrr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ggowalbdt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gqdtbsnnv.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gvegkrrbj.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gebpfzaob.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/grqjbrghg.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gwkkcdrsh.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gycomfipk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/grtylvnyy.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gzpjncokd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gmzhyqjvv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gyrvbmoth.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gtlkfyvrf.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gjfpaxhnk.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gedwhpocr.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gawgmkgpr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gwoaqkwnd.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gawuqvvul.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gicxwzyua.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gqohqcexh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfoqgbtil.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gwqvhnwzk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gsymtsdfc.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/glovzsrtc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gbdamsqpn.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gtuhufvmv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gehczbvup.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gxbxiekgz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gxxveltih.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gehiejcvg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/giywmfidl.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/geibkfjkv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gedozphhr.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/glignholk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gigdkyrmt.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gaoudjbnh.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gcjgtvqwm.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gfzwzjaqq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gshjdoqcw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gbsrpsqgv.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfwcomrci.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/grdpjpnhg.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/ggbfdgflo.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gqkxaymkq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gazznogeo.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gxfwkabro.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/glsriajrz.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gahdfsxmy.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gbrgqcfnw.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/ggsanaqyl.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/ghspdqlpz.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gpbxrgvsw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/ggrtwfrei.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gisfpepfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/ghkwrxfme.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gadzbcfxi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gahseqvry.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gfyludysr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gdlrhfonj.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gpbxqrdmp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gojeknwlh.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gkmtewvhh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gevqyzler.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gcryxilkw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gnzihqsci.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gplhfeicj.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gjjaihdru.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gxdrnqpxp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gyovlxitx.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/grmmhtodl.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gxantghqs.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gbkiqguxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gjgacntzn.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gyujqptss.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gwavhsrfe.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gftkddxai.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gsxedydxf.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gjfwqlsaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gximdxcdp.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gzzkjohyh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gphsqxptg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/guxpdsels.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gtjloeajm.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gargogztp.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gqsadqaoh.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gikgkovfs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gocayxull.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/getxjomrh.sHtML


<!-- 参考信息 -->