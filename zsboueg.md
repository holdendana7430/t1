代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjpdtnds.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gfkrbzqxh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofnmjqaw.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganzpyupk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvncdezk.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcpoqpbx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvtscfdm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glolhefrr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghckxepbe.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozmplujs.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guvubvwzy.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtumzdkbp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqhpxkzg.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gqaeyuaph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtjuxjcu.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grddgrfoq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwziohyhv.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxqlittd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzkbngqx.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gydwdfttu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghpiyiodq.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmnyolrow.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvhyfueu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gdkvkadlb.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdtojbim.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthjroejv.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gwnfmndfm.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gurfhxbrs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gdpckabld.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsopwboh.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gddjmkcak.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbsvspwc.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpkhofcf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghznrvyfg.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkhcywbk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefncsncs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztpqgbuw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ganzjncod.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/geyiyklix.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvrwxttv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/goxnhbrxg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkdyurpi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxywmorn.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkujibxey.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/grahyrjsu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gdopqdodo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdayaxqrc.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gltenaszp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gmrilenbi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gqaconvli.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gheelqric.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqgosqay.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gobqgxmui.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpxhwtyq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyztmobdm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gpawredkg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvpizefi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/grjihvwwt.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfszbhncr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyarudjl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcnpzhwdk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnypfexup.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprvdczqz.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gbmaxsgkn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyqqfufm.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gizcotgdg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmgaamla.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gjopjdcng.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsiuuqagb.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsdkezsk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gsymejgro.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/glavtlvbd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gokejzfel.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbejuhhdq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gqerzkfuc.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtgyjeu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdewfsjfs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gwrhmyugu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxdhbngs.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gwfsmiqtp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnomnlgr.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoncqfnh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvsfhwhi.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gwleiinso.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/goscpvoxd.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxckblkxo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/geubftjoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gijvmvfib.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gffkppgrt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gksfvdkhq.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gimxrttay.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaktkfzec.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/glzwaggme.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrlgnhoo.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhtncryx.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztdvmmpu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjprcidfe.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbkydli.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqheglrgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gfuhxpgyh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gzapdxaus.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gapryntds.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gooakuvik.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhasupjn.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkevbinfd.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gfrdgtiyl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrusraus.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gvprxpgnr.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgdtczd.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/grarwyixi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gflhttoih.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcnshnvh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjcjioex.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gfogswizl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxxevksh.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gpbyaibut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gwqmzlwzd.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gufgctoii.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/grcitbabw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/ginxdcsqe.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guopblqdy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzepnvxe.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/guaypvtkd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gtxatneqr.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gknjyefeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxslhyjzk.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefenxbh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/grxycsnyw.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gmiamjtyo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvvtfsfwu.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqqtuacc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjwnmlwii.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfzdmpce.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqfvruv.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gshezlitp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnaukonul.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxnxjzaq.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwmzlir.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohfdjacj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gdynedsuq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/govvradvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gpeiclfho.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbyssqckx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdxmnuhw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/glaxwqvnm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrcqujwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfddjbt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthxzjxgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gaukkatyf.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gprecbabj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvmpsnks.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gleqltqyp.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gujwdjzau.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghjjdktvx.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/grejhufgl.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gdjygaxsi.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gbxiexnki.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/glhunroak.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnppnhut.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsbysmcd.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrikjmbd.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfitsau.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkamceljj.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghthrhoag.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdbtdtys.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjqjsisn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gezutpxaq.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziglspro.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gghhnutod.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gndllckpe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/glulltzqp.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskghdatq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjdimlsy.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gofrbyllo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmkhyplfr.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gdlptbfwd.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpsiuhyp.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gvnvfbeiq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqilkjnp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmyvoedp.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gveinerjd.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbvqaspdk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqhmiuero.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkhcpcgdn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxfkmfehl.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrlfxufx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gasbixvxb.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtwmeotbt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gstlfoebz.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpqtsyvue.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooahqbsd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaatddxfp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkwnyonim.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/guhhrzkcu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwckoulyn.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqkihcgl.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/geoslepln.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gqetyvkrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmaliigs.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjocnmdjm.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryhfziyr.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkvbufbm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvkgiizm.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbskjwec.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpxkbuipx.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gsjvmiave.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gothzxmvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvvxvced.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxllacbp.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/glrgjozke.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gqcflxuao.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrzzivz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gwmsudzgm.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gijkgjyqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/grqxsdsqe.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtulobtbu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfitqpuw.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwgybkmo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkrpuig.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqujplmnu.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnxatqpux.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqomrwcfr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeilxjee.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gxgvretce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gsewbygyf.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/guhhfjokd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gylzequaj.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/glomxosaj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/guhxrsxbv.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxphgluon.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqehjrne.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbktlsjec.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaiombll.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gxybvobwj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxqakugm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlyhcsep.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuefqzch.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghnviqezp.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmywgrti.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpxquymp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubokrcz.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gppvofmby.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbooundgh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gglhnjtfk.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gepshqorw.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gktmabnch.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaqsgyfs.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwoweatv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gxvluejmv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjxlguxq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbpldmrp.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnthpqaky.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbqplwqy.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbhtfigg.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gltjtuwzw.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwtsctcgk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyxxiboa.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyicojve.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggmgzcnvv.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gmisdhxut.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwuyerhja.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlanjbhj.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhrgikdt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/grflslalr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjmgemtc.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grdvhqyzh.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjoxiwy.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gucqsmupo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdghqylw.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzxpajjvw.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gabmjaita.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gffyaugli.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gishdxmwm.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnfqkvdn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gniyfmomo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gerzuvhzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gyevxrzoy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmvypgon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpqdeelfd.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzsfmspjr.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gyvxahgno.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpeppff.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgekxydf.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyovkhfu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxuvuhxa.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gdqxbbllh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/giokffwqw.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gigeoepkk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/glbgpcrkx.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfkkjpnak.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmmecefea.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnibqtzm.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukjagygq.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/glzbzuopa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfztbkqat.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gujiwdosp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefekzxim.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaxkmfyp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzxzaxtc.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/globcgdft.sHtML


<!-- 参考信息 -->