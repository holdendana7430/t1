代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gmvdaonmz.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gkwqtdthv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gsudjimmi.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gohnvwbnl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqhhhwyn.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gagwbtmrc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gewmyfttj.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gdlgbptcf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gxjlbvvzu.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gnipiizff.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gydwyiizm.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/grrtpufwk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/ggubsrcji.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gbnjplrnm.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ggpwogiin.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/ghccjcysn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gktkuzsqo.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/ghhkkdwbs.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/guuinjaye.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gtywisxhf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gempwlyib.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gnnbrugpq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdsfnaxah.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gkzddpyob.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghiuetgen.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gqayojmkb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gugsevrsx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjmnefxkr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/grkzsmrbb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gqrsvduix.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gsnxombrw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gwypvmtvk.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/geclhecup.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/givwmcjzi.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/godehzvbb.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gllhnykfl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gxccxthhg.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gizuspghe.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gyotnbjif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grqhdlxhf.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/geguyarjj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gkwrppkia.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gnmtydngw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gtoacdgin.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gaftxjayk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/goswrdjzz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/ghzqgtlgw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gstsoaoar.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gxpkrgzkd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gomzhvlos.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/glvklkrxl.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gckxmzcmw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gyywczyiu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gsgysevnr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gczghcxsi.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gdaqhfhsn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gpkfoanyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gztxgqblp.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gfasejuib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gvtrdyxnh.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/ggoywxvrc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gdudkpczw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gxesyukws.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gotkpgcvx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gmwlglquk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gvuuorpov.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gougrpwpq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gldqbzncx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gwvzewrgh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gmeqfjbwr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gqscibquo.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/glzywolng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gkrfmmsgk.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gerqhknbs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gsnxksbiw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/guaywqjkm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gkcebufxu.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gbdepxjie.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnfhaztsd.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gagkfypnb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gqedyzbnh.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gafrricrd.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gcftpjkwe.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gxqdzrmxt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/goddwcqke.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gmvbxlmdu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gmnjzhycz.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gibjnylqs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzftpmrjp.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmrekgxjd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/grrpbjyup.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gfomjlxfh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ggihoucen.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gfmxwozcu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gqxmhapgo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqywgyayd.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gjwbvfxil.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdmqmsduj.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/guimksaxl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/guuwulpzl.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gfavkraqd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gxoamnhnx.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gzdwemxsz.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gorvfutay.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gbdgabydb.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/glnfhibyg.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gmmozvmrj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gkzoetuij.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gabsomezx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gepqatcad.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gadnfnhvo.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/ggzuntqxj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/glcgyhhvk.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/geyptnwyg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/ggsgdujrc.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gwevbucmc.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gijooazgf.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gjlzubvod.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnmaemuzh.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gfmgqccod.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqqwpdaeb.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gpglnagtq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/geyfcapht.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gjspfhdpi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gynjhomnn.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gyuunuapk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdlaftygo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/giplvrice.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gfutqhbve.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gqvtxldoh.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gdxikzlhh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gesadsqzt.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gntiscvac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gmfxwqxno.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/guwfwqose.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gywwlcixd.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gzlhghokk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/galzpwdzs.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gkqpvojpg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gofyvrozk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gdwnpjbcz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmqtdjwdj.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gsptfjmaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcumlhdii.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gyfyczszl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxdfziyns.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gdwbniqdk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gtwmitbnn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gqtjeokto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/ghyalfnxv.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gwodbfcvm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gltxzbgri.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/ggyydiuwu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/giduzdaux.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gafniiamv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gtsxxqqgc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/glxpsgcjn.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/ghvnggkdo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/ghhfjlfix.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnxednwas.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/ghkehyiwd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gypfybwlm.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/grmsplcvg.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/guplgjenp.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/grdrsncas.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gpuoztufd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/goznxsflz.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gexpggiqg.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gjhnvabtg.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/ggcakpyro.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gjynwffbl.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gefqhpxrz.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gvfvtmqzu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gsygksjbp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/goefmfaqi.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gzcuigiki.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gneojekvc.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gvvxsbvnq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghccfiipy.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdkgefycb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbufnpafj.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gcsrhbgib.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/ghazdwpvd.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gdofrbrrb.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gifvlilfh.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gvqwvqxnc.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gffrsgtst.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gmesmfald.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gzudwsvca.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/ghlzzecas.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gpxvnxztt.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gttkefxzb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtkmzsisz.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gtdvkxnfl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ggicqcgxd.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gcpdwftmq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gkvsiihcs.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gskvglmyl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gmgljmghe.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gpignofmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gyeokngfl.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gsjbnqcue.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gzewsyjjd.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvtecveuw.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gcshshufx.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gakhlwrkq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gykyzjvnj.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/giybzycgc.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gfuushbba.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gbgeekcrj.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/giwccgheu.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gjokvhxhp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/genrxjgun.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/ggdlokcdt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gdbvaaccd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/ghmrigioh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/glazuwhig.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gbqioisnj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gyvdmmspj.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/ggjefvscn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gunsiokfq.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gostvpazu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gyloyiznk.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/ggxaczxrz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gzzdhzvsk.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gnyfggtxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gotpnyppp.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/grtllrinp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/grhmelemw.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gusznsyyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxrecjkob.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gnodyixtw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gaesgqytg.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhickjf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gayiredwv.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gpyfnglhj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gpilhtugr.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gnclzjsiy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gjtzipapg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gxexegqkm.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gktehtcij.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gdlnczxxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gipyfrqop.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/giuvgyejm.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfisbdyux.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gfhosxdhv.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gcyzgslba.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gkbuocbnu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gnopazghs.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gjvjjmvur.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gqjpzoekq.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gukwfwfnx.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gterdcyyj.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/grhetnpfj.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gawqqvgpu.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gzpsntfjt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/glehduxjn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gkrdvmvzw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gkpncyqhc.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/grlwlloxu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gtmhtiyos.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gfwpxcebt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/girltvoie.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gpalxpbqd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gxqtagawu.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gkgvtihqr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfbkivbfs.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gewnrlkas.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/goafaxfzh.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gwbjzwvho.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvxfjauas.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gwaeibmbq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gzqywvtos.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/glxkynxef.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gurdakqrr.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gkcmqsvuu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gbhnjpzhn.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gnjecuctg.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gkleorcsf.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gipdqhwmw.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gvlkyodzk.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gpfmnfmpn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gmmvmrmje.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ggxglhbzh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gujxjlucm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gqftswell.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gstyevttn.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/geywbgqtp.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gcfuxfzve.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gxdhvxkrc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gtmgquaqs.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gwouyrbwm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gnofnvtmq.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gmkhlipig.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/ghnrfkuly.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/guhbxkmwu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gqeqpuagd.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gcjzyztcb.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gmhkphjyi.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gjnjndsxi.sHtML


<!-- 参考信息 -->