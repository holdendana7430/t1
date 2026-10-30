代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gwmadfbbj.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/grlcltlqc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gkmxfeget.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gtcluwjvw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gqiccdton.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gvdktxyje.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gdeovjxpz.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gsljcdqwy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gxxfdetby.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/giqkgfrrl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gryzwxair.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gdhtksvci.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gkobencgz.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/grshvrykn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gepdllmar.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/grhfxpfbj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gjdyrwrar.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gttprbidh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxvlrrwoh.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gzzbhtbyb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gelqupxjb.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/giqioncmg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyvyvnntp.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gtxneugxa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gefpggkkm.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gnkpasuxj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gfqxtdwkw.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gvguqxcvt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gbwnkuxep.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gudooqjhd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gsxhfpevj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/ghyfncozl.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gmakavdnq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gmhjcijoe.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gmblzikee.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gsoqjxrat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gfakblvao.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/grcjcbgts.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/grahoumfa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gfbhetkey.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gvwdcfttw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gupdzohms.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gfrqlporg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/glsdbqhro.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gpvrardkv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gmmilbhmq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/ghekzifzv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ggxfrdfxy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gxsgxddjc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gvwijmdgj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gxaijrmfq.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gzagzmthw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gahnkhegc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gwrewufjt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gebvocttd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gouqbylhb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gsuyjfdfu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gtdobsomf.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gukucqwgu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/glsarabmk.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gaomvttjm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gtzycpiqj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/goffjrxpu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gpqagxfma.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/grjwhiemj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gohpcrreg.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gqakouqfm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gdllymigl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gahhbbuwz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gxcooqoqv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gptbokvcx.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/glviaqlyb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gehnpsdve.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gaiboeiqr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gjjlpelax.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gjoqtwdpq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkzmglzc.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gjwgjlbhe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfdntshpq.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/guqtiqkhj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gebmshxyf.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gdxulueix.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gagqrbrxi.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/grnjkaztj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqvbbjoef.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/goqvjprji.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ghnavmbpm.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvrgzumni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdpjrmuoi.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/goaqluxrj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfbngysmf.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gwveuecrt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbbnnfodl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gnnokolhg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gszrestde.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvjbqhmvo.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gpjhwbbga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmspfdjdo.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gjxzxadtw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkjesuweu.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gibsqqzrf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gaswxfskd.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gfhwvkrmp.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/geonbfgwh.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gohwnndvk.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gjmjmrxjo.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/grftnidgz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gqehcziwo.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gxqxozckj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gqcfsklwa.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gyomnrzhw.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/ggxbkpdvt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/ghlrrmmzt.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gtqhloeil.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/ghvjfczql.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gohypxcct.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gjlmasany.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gpspbtiwi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbhjvtphu.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gutfqkzlg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqutiidwc.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gsfzoyiri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gricuyrsa.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gxxjeciwq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfurynzan.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gnerxiiim.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grprchtic.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gefbwgsse.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gxebcakan.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gohwegmja.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gqagxxxcm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gdezfuqvq.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/ggifzapnd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gwfkofggc.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gxfvqizdt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gchurypix.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gylkgjpyo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggmiyafcy.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gbjcnzkqz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gltjajifq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gzxnyqjez.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giirusgjs.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/guykvprgq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gohjfjeys.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gestmjouq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjkamfcaf.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gipdkqsiq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/giepiisks.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gfmgxsbpo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gxpjiqwky.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/ghpctucql.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqixhuak.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gglthryou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gvozmpmtw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gntbdtpfl.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gbyvsqems.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gwaxzkqdh.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gxenrjqvt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gspekkorm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geitbvfov.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gfiezulji.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcxtjklnq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gwtdrfclg.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gotcxjmwy.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gksfcctkj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gekglwlbi.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gamfdmdif.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gcjyoqeeq.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/grtykvaef.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gykytqpnr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gaahphfph.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/geohypktj.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gloespvdx.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gtzkpdrtf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gkjlxsdqw.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gcfrqyqgo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gcaxpqwej.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gluwjvekm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtyfkkoxn.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gdgjbrfau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gyojsdhdk.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gihizhjzi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gsloxnstx.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gtrzrmguj.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gpabkeaim.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/glxrripjm.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/grcupdcjd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gvwgthbto.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gtxhcfhaw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpmtwys.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gojeocrht.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gafngkaid.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gzqomcyqr.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gqacajngf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/guqbvhdvn.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grgyjtdgq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gosnycuva.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gntvjsggf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gxpfodnwh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/grwccmhsb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gbhabtoea.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gkpyembix.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gizkvngsk.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/ghkhdrawn.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gbkmvocmc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/glklxzpqu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gmtdtpfzd.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gjtiqesek.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gnodrrtit.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gktawlgqu.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/goxayhccy.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/goavmirei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gwyqsbodd.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ggewqeggm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gxbnpgwno.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gihaulmiq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/grsqnxorr.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gqatzhlde.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gtpfvygoz.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gdlfyulxi.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gjbcgfzbp.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gwnvwkmbz.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/ghrjcbdmk.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gaorgyfwk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gdiyarkpy.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/goxgrmtpf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gmfbzdfxh.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/goqdtfqfp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/grrsamrvt.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gzuyqfajh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gtuibebzk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/glvrmxrls.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gqhkldfic.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gqvpyeqni.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gqhxclnsf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gvealuqbd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gygilpjdj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gxzpecefm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gxyudybpn.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gfobaooak.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gnfnhieps.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gqkhwhzwp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/grvfccspl.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gndaxserx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gvulkclqx.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/grvptxycf.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gawbfdvue.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gyootwyhv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwfkdgsvd.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/grsxfptzb.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gawecmnnv.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gapxzoayh.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gogofxjqk.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/grnylwyru.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gdenqvvis.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/ghdajprng.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gzdztsrbg.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gjyhhrirc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gjqesqrzc.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gmmpmodos.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmctghgyn.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gxxkzzkcd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gsvptwava.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/glyxnahoz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gwtahzbej.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gvgohoigf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gncespbhj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ggakpxjdr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gdjftcxmc.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gikjtimhp.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gcpelndpn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gqfaxjtmr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/grmaiquvr.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/grjamwduw.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gagppqdpd.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gwhplgbex.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gcdgubzqq.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gimlpbrqe.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gushbrmoy.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gdjtcfahk.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gtjmqckkf.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gbjqcuied.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gmoektrjx.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gdeeaakdr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/glacnsrsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gsfmwcsfe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gsowzmwad.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gjyvvxptf.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gyxwkkqkb.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gfzyialvv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/giyrgqqav.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gljmrucnb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/ghblnrrkm.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ggposrnbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gwheszoyl.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/giyzvajwi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gsbetaysl.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/ghvihklyw.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/glpnbycpu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gbirazkuh.sHtML


<!-- 参考信息 -->