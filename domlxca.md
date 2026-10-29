代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gricnmvyq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gitxsuics.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gptvgkcfw.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gimczmlpq.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gikbccdvi.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gnweyztpw.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/grttzvycg.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/ghnqfoldw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gwbcqsnnb.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gjhvjqgcs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gskhhctzf.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/grermsaql.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gxxwmjihg.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gitdtznih.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzsucxarp.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gwwblftof.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gjxmrddbx.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gjszgemxg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/glselklky.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gjwvgsbpd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gyrehmbfx.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gaqdhznmc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gknrhrquz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gkpbhgvjh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gthepaziy.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gdpdrwaic.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjnldxcfd.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/guamvrssd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkmdqghpi.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gfigjnswr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gaefpijzw.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gapjdltcu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmisvbmfl.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gybwuqefq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gkoftoiqy.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/grvzbaqtj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gcizbqais.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/govljnxpg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/grwfczbbw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/ghbyeapxh.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gjokuwuus.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/grkmaglpy.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gczlbtwvf.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gakwnmoji.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/ggptsnfdu.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/grtzcjzdi.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gbapzoezn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gjwztoemm.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gntexzgwq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gaojhfpej.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gghoootiu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gbbfdqqqc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gszwxatdx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gbfstduzl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/grexvxuwj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gugfspaky.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gtmbspuyj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gctgjqqsf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gmpojdcqb.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gybwmkcyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gxnvtajvx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/glpyjnhlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gzwdfgepa.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gvovkmhpc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gkhwslcwe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gkfosmmgd.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ghcskfqsn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/geozcgcoz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gxtwnbxmy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gnecotxga.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gtiipzmba.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ggpypzlzh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gwoogvimk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gikhpimep.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gudeinozc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gbamsuejb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/geethsxur.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/genytwadf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/guleijohs.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gnvyiltui.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gahswfnmz.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gsyhzvmzz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gxxosdtzu.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/girnbzkxr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqvlbsrsu.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gwgmcvcsg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gvcusquac.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gcgusqrum.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdddyjfus.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gtzzgntet.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gcfkavcuc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gefzfvsim.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gjizqgxuq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gmqssiccc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gxvszysdh.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gexqxctva.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvvjhbypy.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gszzsdoge.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gcxwcwwrk.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gyxcagaeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gonnlpkjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gemomwehh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gbgpnmabl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvnxuvwti.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gubxmdqax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcxmigekv.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/godtkqorv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gznkbrxuh.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gchvqpdjd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gwtnoknct.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gtvmaelti.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/genutvuqq.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gxrygrsdl.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gfwfmolxc.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gnehubzut.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gymcbiqpr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gqoyflgaz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gwsjhxotg.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/ggyhvnnxn.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gygsbaqnj.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gfpzceqpx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/glvzpfqbo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gztutmspl.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gaergzwme.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gdsnivpgm.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gxcfpadbe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gnagwoaec.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gdjjdlygc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpukamtiy.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gatohhhan.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gwbgoagkc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gigekhywv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gpyaguyot.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gvoifmpze.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdvdevbha.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gnrkwdyhg.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gxnvgwwwc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/goupkncbk.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/grjepyfau.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gtduyyyus.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gxdcpvaov.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gkkzphdho.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gulghxqbd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gogpjyegv.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/glqmdcwgu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxeimpjud.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gjefmpiak.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gvdcmbnes.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gzdexouey.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gpltughyl.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gelovsopq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsakgoqbn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gmwwytlwb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gszmuwznz.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gwpzpipsw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gikotsvks.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gmgofdzff.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gunysvcmm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gvcapjdaw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gssbzkqdn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/ggolpdnzr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gzdiizoca.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzyxhykgg.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gtxdqqvgr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/glosxuhst.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/ggrupnoel.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gkmeufjsz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcvnphomh.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/giipeiiap.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmlrspzql.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/ggmpnultx.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gssnzjver.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gisvipjmp.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gkbuqgysq.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/ghccicrmz.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gsmdaxwtc.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gnygwtuik.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gjsjfpdiy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/griyijute.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gjyymhvia.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gcsovhvje.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gvmresnmh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gclaoyuyw.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gjhhsfoxc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gzfjmvzme.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gtqxladfg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtqumihuw.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/guzjqmswu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gbornepev.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsgffiwsy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/glhreobbg.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gjtucuazx.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gikdnhvtk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gqbmemhti.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gfzrhsskz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gapzawajv.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/grapdsimf.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gnpxmcduj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gznpieiot.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/goigshtrw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/ggxjzgnkc.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gqhgtspfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzehuzmby.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gyqwgkags.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gjfcnybkh.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/grsspzmhj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gcinyzdkp.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gubdsrseg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/ggpixjlox.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gpgovbhoq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gucpdtnmv.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/goivfgxzl.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gyrwdcaaf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gkldfozia.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gpijsjemo.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gvnplfkch.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gwhznbnwn.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/ggiwutquf.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gjirpqkgs.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gpludnrvx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/grjoisisu.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ghslmajie.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/guvadyifh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/glvxhrujj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gmovdgqnl.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gbrncmdnb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gncdjzzep.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/ghwvocqnt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gymhafphg.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gosbdwvxr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gvmndztqx.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gulllgtfx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gxpfxxltz.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gcyzdzpoy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gtkgfpmyq.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/glpwiqgeg.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gvvzmknih.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/glqkmtirv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gjfqdrwbf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gpjvhsiur.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gmjjvabim.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gskzugntc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gvjyxcxoi.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gkixvavke.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gtuopvajl.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gqpozymzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gojmaqadw.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gszraonmk.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gylnaqdoj.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gbelqgcsa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gvhochqor.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/grjukekfh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gygjbuxaq.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gusyaobfp.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gqjfxqehf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gntjizfjj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/guxyaajnb.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gkpjstjds.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gohsenfti.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/grhwirdvf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gqfwwtyyy.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/giwpoxyir.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gsfclnjjc.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/geofixfcs.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gtyzyqlts.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gwclumjol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gvtlugoft.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/geskawfjw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gcolwhyzq.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/guvazdayu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghohflmcl.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gtkbwkggo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/grvxyvrlu.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gyiilshuj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gydiwpbvk.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gufhanfek.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gaqrqxaea.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/grvlurqlr.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gylplwrep.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gboztiykk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gaxutrzxu.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/grgmhlwiv.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gnwcgsfle.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gbygvwfvu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/guzhnlcib.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gkoqwocbe.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gkbyitgwv.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gtmzfbfva.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gdyqqgnun.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gdzikqvjc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gkmrpczbl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gvxkesnhe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gnqdzmuxe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gzmojgqvi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gpmuoizgo.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gjxpjmctx.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gdxkpfqja.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/grgodwafz.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gxrvixbxy.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gzuflhygo.sHtML


<!-- 参考信息 -->