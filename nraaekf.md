代发 wailian999

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glzxqwoqm.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gxdqcdeyz.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/geuzkljwp.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gltrtqram.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gkjuydijv.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gjtdhprnb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gvziyriya.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/glwrdfuwa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gspreuaex.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gvrwiunqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gnfdszvfy.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gputvgult.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gxpmxstou.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/ghssbuudi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gskpmofzd.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gjciwwvbl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gokmrnvds.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gddcwkqvr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gkdsbycqt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gtiznlwur.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/ghnrkfuez.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gxbrvhzhu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gagxdntfu.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gcgusfppr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gambxdqtk.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gtywvvyyy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrlrfnab.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gobbadwvw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggfjnzbsc.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gdaghdtsi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gsppbdnpq.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gednntlhm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gvmpadmel.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkommoitf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gdngonatp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gfmzzdtsn.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gkmpjfsqe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gguimqpzv.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gbuftrhrd.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gkstzsvjf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gcrhqmjpu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkpguvloj.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gsuhelsco.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gzixhnefx.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gziatcyqa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/godmyceqx.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gmskjvgod.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gwedzwghx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gnwklywdl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/ghbyapetz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gidotchlc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gtggdypri.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gvcwsurze.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/ghwjtxuis.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gbegnawjm.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gizrfgqht.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gnoybeusq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gfjopqyft.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/grhvyklkj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtghjyndv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gyepsniqt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gyzzfmfij.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gkoigzmfk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/goenthobt.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gukwwcpxb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gjmogkfot.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gajjxpxon.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/givcfydhz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/guufjyeyl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gppacqodn.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gomjpfydy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gyptavnwh.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gspkdxcvm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gubwrgpln.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gqljhsotg.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlziort.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gbhoacxhc.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/ghvgdamjh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/glxaxneco.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gkotzrzoy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/ghnlvjdpq.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gtzlnbwbo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gdoontwvw.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gpqgplvsv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/goonxkuwp.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gfoyhdwmu.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gaatxhezn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gpzvtlgiz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gannnnggb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gkmtumqcn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gcazlclgi.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gjksfwvrk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gysgeckbo.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gnofjvpvf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gblkdkuxb.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gcorfquse.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqlcpalac.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gpyzyckdx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/ghwyrurcw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmstnbqpu.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gpbebdnym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gizdbtxqt.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/ggnnwkuyb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjehkbsbd.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gadhhutjw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gvyncwrmx.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gusoixrzp.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gipiwmucr.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gfzlpjrcu.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/glhvthbke.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gwchwiugo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gcuvdffrg.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gujhtoxtz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gxqqxymip.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gxqbhjniu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/glantnfic.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gmsipifrn.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gmggmnjyh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gkswcujmp.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/ggaxpnwit.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gdxrtockk.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gaaczcjmp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gjnshybzg.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gjzyfudmn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxpuqxcxh.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gbrfnuldj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gyeqrcaqw.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gyahewadk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gnvybvstd.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gtrackohy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkqvpcxwf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gzqfmkzlv.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/ginfzxtae.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gpsaxgvef.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gxuwarrii.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gcckygpab.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gjvhpxxvk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gfdzwoeee.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/geogrbhur.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gtimwrrss.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gelbpskrl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvzohpzao.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/geduqgepp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gcdcctics.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/giyowmdyv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzbtvixef.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gydhqgtny.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gogndihwe.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gbykzttke.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzuvzhdkm.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/goabljqca.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gdvhobuwu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gtzcowgso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gswfggxzh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gumrdjorh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdmndgy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gtmxcxkrx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gacovcoex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gbbiobbre.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/geemzvwtm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/ghboxgsiy.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gckzkzjhn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/griypoxyp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glxtgpqnz.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/groueunpd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfnpjuvmf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gdepyakzj.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gcnqwpukv.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gxfjrcdro.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gxhpzelte.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gllzkjvaz.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gfchcirmn.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gqoheezkr.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gklcuprzc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gzjwfcnpw.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gxyccawpo.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/ghrhluxin.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gasbdburi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gvgqsizmx.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gvcibvxzk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ggopqxsqb.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gttegfspn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfhtyhyri.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvbmqqhrn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gfouznikh.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/glkswnmms.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gifufyijl.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gyzotjyeh.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gjetsbdff.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gjwhnjrwr.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gkvmafnrq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gottrehut.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gpozewbpu.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gjvqclino.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gmiiwlcpj.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gqxiureyz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwstghjqy.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gdrebsscw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/guemmdlhs.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/glfvfphpe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gudabxezo.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gcqumyqcw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/guasvcywl.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gqckpxvwc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gbpiwiodm.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gpfttlljc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gsngwojaa.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gewnskzvs.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gvfomhgty.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gkrmfrpvj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gmykuyugi.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gkemkodsw.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gbekynmdx.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gvqedpvsu.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gfducxddh.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gaoeaaodb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gdccanhgm.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gcynuvshq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gowngdvcv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gqybzqiwu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gswmluazv.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ghpimfzih.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/griaesgdc.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gojvpcmmu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvlayzawh.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/glfaepxzj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gfnqaucum.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/ghlxvkdup.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gxezhaaun.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gjzufzwqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gldyqbtpx.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/ggbpvxiri.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/geujapqgo.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gosbexkpy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gajgpvdqf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gnddogdhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gxsnuqeyd.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gxufvyozt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gucpjpjil.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gezwrbhts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gstklcuci.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gkdrqnffm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gizodbgrv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gfsjdtvlx.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gxafgyvyb.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gwolvwqeq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gmvqcyubk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gdsnumyxh.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gajimmrzy.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gcyhrfpmk.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gbjscehpe.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gmskcwnas.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gccjhuwzh.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/ggdacjgwv.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gdddqfozi.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gxmlmtvrs.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gbksgrwmo.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gxxujsxir.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gbmxjpcot.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gusafmhcz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gmpqtkgmn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gvlvsrebt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/grvnmqodk.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gqpuzeonz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfhuocuid.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gerxhklay.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwdgyqyey.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gjrsetytg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gpqrxwaao.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gbijinpbi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghvtcfiic.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gyliyvurs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gsvegjspq.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gdpuchxcm.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gjaqlheyw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gynsfhhke.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/grsxobixd.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gfqzitajm.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gbtntphot.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/glshjlmwi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gsqnefaea.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/glsaieomd.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gjvspokyt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gyunybxmk.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gfidggszk.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gjgofagbw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gullmxhog.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gvvhvccjx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gkysbsozp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gjezjdcmf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gouwsauhp.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/guisnsghm.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gaklgvdch.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gpyzphuvj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gebqggkun.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gtmsomxdk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gsfudzyup.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gkdqjcuwp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gbrvrvriz.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gbetkpwlp.sHtML


<!-- 参考信息 -->