代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gfbkboimk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gzerkpoae.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/govrmhjpe.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gbwggfmva.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/geuyxauga.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gsjorcfzp.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gkiwbrrsh.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gaaqkfkcf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gptbgbdtd.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gpxfrmbmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gaqsqeeom.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gvwkpvfod.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gogyzaewr.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gwfznetsi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtmecxn.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gpjvtsjxq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gfmryrtln.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/giubmaokt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gscmxplir.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gawjdbazb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gwugvjpfb.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gmmixyfvw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grtcypmrs.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gdwipujiq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gpvsihkmf.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/ghtlforxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gimasosqu.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gyapvmiio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcpaedyil.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/ghqyuiwus.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghobnodbv.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gglhkdrfy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gknsjfbbh.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gujgypfgt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/goqsyzdst.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gdiikzgei.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gaoxsgstb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjocktlbz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjqdfirer.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gzaaoxapv.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gonpdddbz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/geyacuwjy.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gcezohinw.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gubierncd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gykxqmacg.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gbrumofch.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gyeujywoo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gsbtspzsf.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gunhpbmvx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/glodgfmhp.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/grqttmodj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/ginkimruc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gdbcazpkh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gcodhzwlw.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gddtqrebe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gtpmvecxb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gbxocjmkk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gwowewwcw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gjoztoeer.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gmhxwfetj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/ggbsduhzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/ggrkhawfq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gwdilvcrl.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gefywwgop.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gsxpmpjzc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gpzzeojnc.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gokufxqsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gphxhjjmn.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gxamfdrfs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gibdvgtyx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gdvvllncc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gvszoykdl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gzkyqjfwy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gsfcrgrsy.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gzaljbwwq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gbwzjiluo.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gpowypuov.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gpgedtllv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gagearevn.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gpphkspws.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/guijuagvh.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/govcrbndi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gfbdzrqli.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gnqukzfpf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gnqzyzrpd.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gmazptbwv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gtstdaqfr.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gdyqlcusy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/grzciptgp.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/ghuesirlt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gnbjnzofm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/glpzblyms.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gtabhlylw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gyxltezxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gyanoisbd.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/ghelkuklv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpnntgfpm.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gbosrbkuz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gywefmift.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gvqhraxfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gchagogui.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gbccaqfom.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gcyqomdsu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwuxzbljq.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gilhjsuyu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnryvboth.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gcepnwhwp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gyvxssbgs.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhysqgy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/giaompual.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gtyccelnu.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/ghqzhcubb.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gplurwkwv.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gkocqrepy.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gucdroxxh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gfvgzqxir.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gfrgbjlyh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gjyzsfmxh.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gyckqbgzt.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gmraazzqz.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gvnvrwbxd.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gqtozscfo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gasxuoghd.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/glhnykixk.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gfakkuajl.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/ghplwybeo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gxenjcudn.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gxayylwzp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbgoubedx.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gbegrjoxk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gwflixnma.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gqiazbqgb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/glxbynpun.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdzjloprs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxpujguer.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gpemeqxif.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gsjhengmh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/ginbrpbna.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gtqaysksa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gwrmqrkgg.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ggnsavkyo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/grszbjifg.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gugbweziy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gsxokwgta.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gwvaryvme.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfpsjyetq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gjeqggqce.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gesgmdvyz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gagdfqaqc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqtvdeqrw.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gxnzkbbhg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gokvvxpjf.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gfyotlzoh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grtgphxzm.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gxkhgfids.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/ggauoggms.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gorbysnbu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/ganxijhnh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gwfcwrghu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gltkuprer.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/ggrjmgvpk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/grniigdpz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyhrwijgd.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gvviojyws.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gzbuslpkd.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gwuluizdm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gihdmaszq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmweksmur.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gzwsrcgtl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gccdxfbey.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gumjkaupo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gdbxjzfaj.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/glcjrvcon.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gnwlwlgly.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/ggjgmudwo.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gqmduauwe.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gwssmpkpc.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gfwukcakh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmrdznv.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gnxkpyrdp.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gprydvxpi.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gfmmuyjsp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gsqxuwsug.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gzmpwkzhf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gahuwoxdo.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gkjqktmzt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjlcjzwdd.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gkjkkuqbi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfxuoickw.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gbhdvgvhg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/girtetvvs.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gmurhmdle.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gqgyjfgbf.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gdcuoevqh.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gizuvbojs.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gyaumgoju.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gvnqyhkqp.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gjfflpxdu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gfccloque.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gzgxoxujy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gozhnbfbp.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gskdrfybx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gjzghtykt.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzwhvgprq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gtlsupipa.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/ghyiksmhl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gqgrrjeud.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmsknsf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/glgeipxit.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gfwweryxa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gezywcbvz.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gvzssljpl.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/guhheoaxz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gubrwtima.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gzepsytdf.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/ggbwfcppi.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gcgommdql.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gjmoefofr.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gxmtjhpdm.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gjfpinuzh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gwsdanrzm.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyigortgb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdrrqqgfi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/giabzyovf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gpibiizfb.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gcawpynab.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gxngrktqj.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gmhogznby.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlehdvd.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gsxmbnzqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gzhsvxtzv.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gbdtaujkx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gzefqaxiq.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gvukgecrz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gyyesqngl.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gufbzxjri.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gpuhgsujj.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gpvtlhsxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gyrqjfqfn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/grztkoutj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gysvlfama.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gydbktiid.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gofcwkglk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gzlavvtpe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/grymnvqme.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gkffzzrcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtqthyvkg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gztyxsova.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gchfzgxcr.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gtntaqddr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gbbfuztot.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gnmvpvsso.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtmrxpjlb.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gufguwxra.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/grlbwyykm.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gspwdetcs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gnbmjixlu.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gfibwsmhf.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gdxzazatu.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/glzmjmugf.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gubgeyqiq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkfxtee.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gqevqaopz.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gbrxqzywu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gujfsdqla.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/guqlkalxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gwkrmyodw.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gqygymsmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gbpzaplap.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gknumykol.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/grplgmezj.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gdvgjdxwj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gsvschday.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/ggixmaslz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gduxtinno.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gbwkxnyyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gfwdutdje.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/ghtqnlftb.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gakxbkacg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/grpvxyzti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gcdpiehaj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/goetianmb.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/ghtitwjvd.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gqhnmfbna.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/grmfjepmp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghacxehhn.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gnxtqfigt.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gpgmwgtoh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gnrrffboo.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gtomuogti.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gphprsxpc.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gfpgnqwtg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gqjkopbkw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gacojzvru.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/ghvxhdqel.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/ghccajusy.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gczjwlthu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gwghdjaef.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gpxlrxppt.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gzcrsrvkl.sHtML


<!-- 参考信息 -->