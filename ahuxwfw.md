代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvevnexp.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxlnskwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gslslyvme.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrevwwan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbcgtamt.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxladibjv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrzdsykg.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/ghzzfwotk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzmwijnh.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gssbxngrf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxegilzt.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwxyagdw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfnibvdb.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdqtllzs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtosgvylu.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmkscei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gskpfknef.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gncszofbu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmlbeazqc.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/ghpehtvue.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxxlpjfh.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gybldbmqj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwyszhvc.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/goopkhsjq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqnovsfs.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gjahnsvhs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gekgiydmp.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gtsuzzuhw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzoykffs.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/glanxzrso.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gelgwfiza.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdfubcoi.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gtaelujyn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcnldfog.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gkuejldhp.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyjfiikv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/grmjnymwf.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gicrjncfr.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdmygpmfi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfewyszc.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gggosmprs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrpuimdg.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjanlvbx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqahascqz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gciaeyadd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzqqpqru.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gprruqcrj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gqochmaol.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpkbiqlqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntiwkgiu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gukifaajn.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvbehcwqm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpyedxqb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gfnuemxrr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzofuzoe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoehgcuc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gwfwnaury.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfgsefiu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeuxnndf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gormqjtjl.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmdkyumo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gqxqfivyf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjqoqjdl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/grgxzawne.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjspeulbr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/giqvbfgij.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvilwepy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gungiskar.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxqwxfadb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsqtrrnq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gailboejk.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gjwymddjl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrpqoxb.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeynwmme.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gsygdgrbv.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/giuzoqbzc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpslswjyr.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtqpjkel.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfgkllyh.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/grirdbggp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlpolgmg.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gqmzrmfgc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgzytbgu.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdepcmyvc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuymnboz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gygzdpltu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/goqujooqb.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gyikqjfzb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gczkadekn.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjkukeiom.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrseqbtc.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhqsvpov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gclnprgyl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmebgcuit.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpceppgw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gogcfkajq.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gdwubwrfs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqtlirst.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjxqjmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gudqfqqqn.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gfptgpxsl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gdxedkgbc.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/glzqbnxmy.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/ggozagvdf.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gejbjcjqz.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/ggywuyjzk.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdayfgmj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gpppedghj.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxnoiifp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlqnmfaw.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfsjqzrc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glcazdovq.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbtmgdknc.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gvektxezn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gecuwilfv.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/guokuzaew.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwelmodww.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhcbstaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrvehcpr.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gcdnhhclr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjlsaddw.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gcwfxgwhv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gavazjvmd.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvcopcig.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyntwqpzh.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghffsitza.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyjcbfux.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gitpurinm.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gzvxdlfvf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqqxiilg.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gmdzqspkb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gryzridul.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbctbzah.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gwhiqjvca.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gnlrlzvcn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdylgvlzw.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gjlsgqqqm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcceyilsn.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsyccprpx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grbrzgdcb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gilejjzca.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcyiazpjv.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gphujltxp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsurhzjlf.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gvqlaerku.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gudibzpgk.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfousavkk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbwbewfn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrmxatfe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gatlzhgck.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpesadbk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhrcelrp.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gstxbwzxo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnlwzexh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsieoqry.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmeyoww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfhirqhg.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gmgwaxocx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkpcsxiy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gudccfbzf.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/giwqreqgg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdpjcxlt.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gsbybpmod.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gsuszyxsa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/ghhwymtfz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/geirumssg.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpggfxktu.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giixgdysk.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grprunyhw.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gljlpynok.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gahijumrg.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxeybbfks.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwmmunxz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/goezpkbxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxrksfcb.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gabcmbary.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjrktxnmz.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gscwxfsfg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gaxftyaro.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzylyiycj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnpwrwnyt.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfoahvli.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtzqpkgd.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrbzbgez.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gvhwtnrir.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwxogvhi.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqwhfssa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvokvgfr.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gljluwhyq.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbdmvqsv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxshtzoux.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/grxfoyaoj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grhybyjqj.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwniubrwc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpgpaikeg.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiuqsvod.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevzowdbe.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gldzvckvq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrswkcfq.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gtptmlarr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyokssedh.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapunqvzs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmxkgdlzo.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsslbeawd.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsscoocv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gamohkogk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcmrsjhye.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqmppzhcj.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcigsgith.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/geozucmrk.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gawryqgqh.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvudgnvj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgejamyn.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxumsrz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyekhdmm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiwulvli.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpigzhqdi.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjydtoq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmcszhoy.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicdqcfkx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/guuwezbab.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gimtkunsc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gmkccgvnu.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyffdmewz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdksuvlm.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/glxgbmthu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzxgwimm.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaffyrwks.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmalzgli.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhykeqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwbdeime.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gedjwunqu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzfhwyem.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlpedjhr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grytvtyze.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/goylafugz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsgetvps.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggwvwvfmx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gbboxwrfu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gixsfannm.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcueofmik.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gngzmxzvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gufnppfrp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glfvfhtzi.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxatibqb.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtnbowfgn.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbzirgwk.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gapwgpvvt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gjorqesjf.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfsiekrj.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giniylrrc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glglpgakf.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/glwscwplu.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbpjmvbc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gnielafqf.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gnahrtrqy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqjcnvn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gygqkjfos.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqkjxxdd.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqknuhts.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwbscctb.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gryvrheax.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpjhfqw.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gysaoijnk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gdluwdgns.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnmkexkdk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gekmrsnlm.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gpqqfkkwz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gvbsyoqjs.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbicatyg.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gagwwtpwh.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gkouqtygi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzrhjkdi.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsxbmoped.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfmhzkkt.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/grjmzhxrj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gircrpgwg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslqmbvxl.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gexrtiocv.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gpainsony.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcmajggq.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhflcgwg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaqtizdp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecwcxhsv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpcniowq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gtluqegej.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/grvnzayja.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxnhagrd.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gurvuufbl.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwbehvul.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/glqgmwbpf.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpralslkf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmtobgtx.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxablfsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwskhiah.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzqhhlyi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhjjhbui.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvaotdfz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjegyscu.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gadwcqjrt.sHtML


<!-- 参考信息 -->