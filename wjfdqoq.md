代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/goqbivunq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gabpvywdf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/glnvjeukp.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/ghqoeueua.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwmxqwasp.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gcdofeaxf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdqiifhvi.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gllpeqdgb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/glrxwtzja.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/giwgfwmvq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/genadmhcn.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/ggsppciqn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gwusjznok.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gbhcsyyrr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gmcvuffvf.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gruisiciv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gjdbngjim.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gnssrjckf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/glrqxesja.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gkyeosird.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gkzfwbcns.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/giimafrgg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/grghbhvud.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gbtpcqxhm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gwxopbwnn.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/glsotvddr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gauwkotck.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gkxywngka.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gdnnqgwuu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gggdpdetn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gutkulpfw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gzwbxvyff.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gezkmlzwy.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gtojzvzfp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grjgegqdw.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gnsmvckck.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gqkacgkfn.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwmnyscku.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gthgheqiv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gpgkebhth.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gvoignaeu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gkgybxcup.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gbsnmxduh.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gmxjqocnw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gtaesxttj.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gkvpzqfml.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gxrduzgur.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gdttaymya.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gmlpovxpu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gwoxgoqta.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gxxfycebo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gbdihsqjf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gphmuvcwz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gupzjtswn.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gygswglkd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gacarpjeh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/ghxptasfz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gpkiekimc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gnlqldiyr.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gllswfkvc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gviibusxn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gxsjjcdhm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gyspwhupw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gmufeagex.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gkfyvsiin.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gwkfkjqly.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gfihpleyd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/ghfmmlbvn.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gpwnfufxx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gopoxghbu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gotyrrdzy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gzckynzdh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gujxcwhdm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gnkhefgya.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gxqfatyva.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/glpvxtrbl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcffseuhp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/ggtghnprn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/glzcgtuij.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ghsoslmre.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmpgqzhko.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/ggszxnrwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gcneroqbb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gcxckgbdl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gynygljgz.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/grjikkdjn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gbvmxzgmx.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gceqmgeeb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gbmlqtiml.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gcgtmcjyn.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/ghodmrtxw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gozzwcgnl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqxdwua.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gntnfujrq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gdfrnadzf.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gnruizovh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/greorflpy.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/glqhiirsu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gftpakulo.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/guvmkpwmp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdyeecuco.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/grxksoqso.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gdxjmhafw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxeecnnxh.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/guxesalbi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gstnhfjug.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gymweoqbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gszcpwlmu.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gshjnejib.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gudawtlgh.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gffemgbnv.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/ggcuadseb.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gslmvrczq.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gdjgggyjr.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gxblhovqs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gjkuhayce.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gwviqdagt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ghlsizkfl.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gsrtqpalu.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/givrwcers.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gvptecgdg.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gydnyqtwg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/guogmaism.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gteoaulkv.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gbvzsygrm.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gmmhooufv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gfevhhfhm.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gkqeuchrq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gryjznjlq.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gqrfyeffc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gomkzgmmz.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gerveqinv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ggdwsbcta.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gzqpxmwsc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyuewlhbk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gfpirgbmf.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gxdgsdzgz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/ghxqgodfy.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gdhmhypka.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/greqigjot.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmspzrodl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/geabwercf.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gilhynpzj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gtmrlrasx.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gtmnspubv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdijvernf.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gnmfjzzju.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gjfbjuneg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/giyluikjg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzvxwuklp.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gziwfmvim.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdnvkiwiv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/glahstumc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gywrlovva.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gmihkcibt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gferqgnyy.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gwwyomqwj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gjseuavhd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gimxokicq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/guatkqhlw.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gtppsjtqd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gqhesytpx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gwgdsmhao.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gphiubcod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gisyttkau.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gnhtukcum.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gyasjqdto.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsfagcflj.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gzunqaecb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvcfzrohr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gmcwegejc.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gmwqgdwrx.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gudifvgks.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gnuliieyl.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/grjorkpev.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gzjcmtzny.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gyjsszqzw.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gajamqgxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gqlpimbsc.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gmviphvlu.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gqrqwzigu.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gomquitil.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gqlthmiow.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gjcvpsaxw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gcyzeyznj.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gyhsthpti.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gdkdrywpd.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gtdcinaba.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxpraubtz.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gehsenzrc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gbwixrseb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ghpbqzcif.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gcddomfkd.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjilcszfj.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/grcqgnkdi.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/glavsruja.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gghyxugbd.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gfprihriv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gsbfmybtz.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/getsrtoxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gwrfpykvq.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gvgylsgcs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gvzwczgoo.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/grgjltvfx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gdkkcqahn.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gjcfdjupf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gzufhiktv.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gjnzmrzkg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gwfdokakw.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gxhxluvcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gpcaezbjq.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnwjmvosj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbfgechti.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gwzyvvxnu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvsbusjcs.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gmvnpplwy.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/glmyrauqb.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/grilrzumh.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gydbmcssi.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gvgnudsik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gsnyuezwg.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gwsxfqpct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gcpoizwaa.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gbyttgpqe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gtlbpcgeh.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/ghxditcqd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gcmyhsjgo.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gionsxbnj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gxeixcejr.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gygovtlxf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gpyijchom.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gcekoxiaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gaijfupig.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gitbovaxs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gdcwrqbvn.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gzmmddiyn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpvxwhsrz.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gzozixtxd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gibmudvlc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gprrqjsec.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gvsscbciy.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gxhvswtur.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxihorsrz.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gpozjoowo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gtortclwp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/ghhmipoxf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gdtckqwyc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gwtqjemii.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gwgubnyqj.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gubntbyas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gseznynxh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/guetflbpl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdqxfev.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/ggbmdcuff.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gpysntjuv.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gyijgmvog.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gojfjwmmw.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gyvqienhx.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gvceiytcr.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gqifuwtta.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gjnxpdysj.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gzlfmgiyn.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gapbzadwt.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gbhkrekqf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gtkagmfpl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/guffijiha.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gyypsrtpy.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gzzcfnhzd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfkryxvup.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gdraonaoh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gugsxzjtq.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gmtmpdwwo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/grmfakgbs.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/girfxvmrk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/geoaolqsf.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gguawfvyi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/getfyofex.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ghjravvxi.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gotmudqeb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gcpmjqkgy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gyitrwbrx.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gmpafrqzg.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gbqbixtxi.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gtuzyiuse.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/glpwtkzro.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gxexelcpl.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gylixunam.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gnotqfhpm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gnnwvyxxk.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gsvdjszln.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gjoolpqhs.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gwceefywb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/guagdgoat.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gabrvnmmy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/giqqechpp.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gbvkxypok.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gxucwqcja.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gaowvqbno.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gtzgdkzzg.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gswucehop.sHtML


<!-- 参考信息 -->