代发 wailian999

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgilhscn.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gugcienjg.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjqelcm.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvkccpcjd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzbcrmqoy.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaufzvlt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbqpqfcn.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxacefod.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtnktnnp.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/grllymdyt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geajemdac.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/ggfmqtvns.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gvmaxlgdw.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrwrhapj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/glzzrglzi.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gfwvrfqie.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoawbhua.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqujzyivd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmtdpnjph.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/giqmzsxeu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvekpjhf.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gyfqlgqxt.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gezuxmvhl.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkawudfba.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyukfelgt.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gsnimxhgx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtysifhrd.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwryxjsiy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkztiqmrh.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gyddpaduy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrfxgzaw.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gabjmyrwn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkmnjicc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giktqxkvc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxohbqq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrpaghqw.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqsmipoz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxznldl.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlgjqqgs.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gncbdiwzh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gokohqqpq.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdkrqqjc.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlhrmfht.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gjusugfvk.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgjsjaov.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaclalkii.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gemcwmofv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoxdnugg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxhlxhhw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhooitfi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzpsoevd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gouynomea.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gggauykhg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gegalfbex.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfbixhef.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhxfelom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gikqlfgsg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/grtbacvcj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gftirkiox.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbifleadx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnxhgtne.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqghbdyz.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmfzalp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbcjpjug.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbzeujpqb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffbjrvt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmlvoizc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gslloxbri.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/giahodzru.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrkzwmiq.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gotqaagst.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzemfsxff.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gxcuhbkib.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfdbkcjk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjmyftlcc.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gliynknas.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/grlfrtawp.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/geszeuleh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/goqjztmab.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfomtjtg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhlvnziz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowsazwxy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokmuaqtc.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gyuyfihfl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkzvlxnu.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/girqvdsxm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gfbnqyhcw.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gfjqktqcu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkomxvplp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbidplgc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gnkepvzkw.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gqgvjqmlw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnneccar.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgkhuikw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glornasyl.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/genrzqtqg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyaniblv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/geyttshhp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsslnyqjs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggztcfdgi.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndlbobuk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwturrmo.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhhtgnrl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcshzmai.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gffkgtykq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gftbfdiji.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/ggknbuhqy.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/grnutfofz.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/geyvrqxxf.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gtffipnmu.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gihuzzixt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrpoerpe.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gynzlpywp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqvbevaq.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdiucbnk.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhebdvya.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxfotghtk.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvyhgjbbu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gyohfkwyw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuprmgvk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxufvwjcb.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwcatzpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkbxtiit.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfeduags.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggosizinz.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gdupujamf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gbxxhygkw.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gpmqemnyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/geimmmpkj.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gekajzsjr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvriiurfu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gprcduwcq.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/giuwgylaf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gpjuxdhbj.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtoksmar.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkznetoag.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfscbcqvz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbihchyio.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gtulfyxbf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqckjdpw.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/ghuktvhdw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzpjvxazg.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnixeuqpt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdzpxiwt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqyetlxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghykmrrok.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gccretjtq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gboowhbuu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/guclvoxlg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gypunxxhl.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gegmlavvp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfiyiuev.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqfuvri.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gfjrmdahk.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwoxwcgcr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gzuktxmqr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/geklegpmx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gkidaftya.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghakgkqyq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplkojlnq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkdjoaiw.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/glzrlvcih.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gemstkdej.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gijhubgio.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniqgzxfa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzvlixt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtekmfkmf.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gtjutzbis.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfkcqyzo.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gurtckktw.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gsznxdgzz.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gktuidest.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzklbuwz.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/garxtsjlf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gburrmqbh.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gtzkznhkf.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqtmmzah.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglkyrbyv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/grceqpurm.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzzshusjx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttcuonh.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmqfpmj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfhecqxh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsvkadbi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmshmtbnv.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gchqetrgf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/getrahjvm.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/giciafgjy.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhcjlxkx.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/geagajtdi.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdomjdvf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtcvtuqp.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gbunkibua.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfvxobo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfqtaowpx.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gussivhsb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrbbosho.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gfecwtxfc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkbqddrs.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrrmqzmd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqvpfevpw.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gudspqcxs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guopgjssl.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gutseblfc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmjkhrwcu.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gewkheerd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbhquvlxw.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsenpgxb.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekvmgoln.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gysfaoscw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfogyutmc.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsijthtky.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guinlfwha.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gahkvlksy.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqwxkyoub.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gabpmlzgk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggerwnldh.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmebmjizm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcgdpqes.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjcjrzks.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gatdrfcva.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfcdytdp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbubkuv.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gsppvtcdc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gibodvzwj.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkoavmtz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gctipkwcx.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmzwbbia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosyycyoy.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gslxhlcdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/geiblgolc.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzvjbnyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzdnjlyc.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmhxjcab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozvutawo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gsreoxbkm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoitqutc.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gkpomqbyu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgocmegd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrwwilxn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunmfqbgy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmcfymvt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gserorsyl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gknjwhuhi.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfoedgmf.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gmtowjnsg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfurrpgx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gtntwsiby.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrqbjbir.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/giywvgptj.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gvztvakou.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/glrhzdhsg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdlierv.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gphhkgykq.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzljwaboy.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghnthhjbv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlfilien.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gcdvayijo.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxfacgfby.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtatduz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiscccrv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gobzwldja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gieuvmjsj.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grghdrcuk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glfvhbqik.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/grmjjuxnv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmjpudqyr.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gawzkllmr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdprtfp.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqzinyjcf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqwfzaja.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gsnfdszmy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gteivbacc.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gqrtaunpk.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcstrfezg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gvascxuii.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gseyfcnet.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfxgrjxer.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyjvukdl.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcgshlni.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/grcawyrmx.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gxthldoqs.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gxumwefth.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gdcjvjmef.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ggkxrynsj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gczvrpzhn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gsnuprgfo.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gprtekmqk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghifqbjxb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbrktcdbx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gvlfilnum.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgutarix.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjgukhg.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghofcmecm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjbwoahd.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gknletcfb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gbndpspdz.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghqzukyje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbzzwfdp.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhewcpjz.sHtML


<!-- 参考信息 -->