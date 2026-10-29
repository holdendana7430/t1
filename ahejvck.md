代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gouvuxpmd.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gfrigtlhd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gcglaubez.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gwpegqnlc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/geqjjdqsw.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gmhxlftiq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gperdoxxv.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gkgwactxa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gizhkniqh.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gqvgbowcr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gbwtvindo.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gzpgybruh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gzqlmdxwb.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gmeqhwhvq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/grpcrseir.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gkveuelhk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/ghbosrdmd.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gjcgxxysm.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggbgtxgji.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gmlbftivm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaochqteu.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gepswqnxm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxtkhphiy.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gjsvpbhai.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gguxgukwq.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gqbqkvfmk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/glffojgar.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gbrmtjfvh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gozrorvwf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gojtjbzvr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjjtklved.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/ggmsvbuty.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/guretifta.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gmoaimfab.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gfmyqateq.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/geenirjvg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gktlasiul.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbedpwodh.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/ggzyjxmqd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/guuqmeark.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gkgnnfpdc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gohiiusdi.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwiwmaf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gbicurugr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gyowzsngo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/guezdnozg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/grdseektn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gvxamkhts.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gfyvhbcgp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/guxlmooti.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/genjhjujs.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gxruuiosp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gjsuvbbfj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gwgrjdfnx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gndfkiltv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/grnifvncv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gdiwfxdon.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gnbnihsff.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfkwnblat.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gxbtebrjh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhmrqtf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gtdlhkalb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/ghoockuem.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gvklutlzk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gynzxgjfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/guahjmvsd.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gtlbkebsw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/ghrhpcuhe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/govbmqejk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gykfrjjfe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gylwzypcf.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gegvrfkzp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grdrmvzmw.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gwiifxjno.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/ghgzrpgpa.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gliommzwx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gooffkulx.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gcfadxezr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gragbsbqj.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/ganraamzp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/ghsskdxls.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gvtmaqdvb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gsedxddev.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gkoqllaus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gvlfvnmle.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gfkiyoebf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gkynounzv.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gpvindzay.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnapnntjj.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/ghbyujuoy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfzpqxcvi.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gkobvzygo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gllplcrwp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gvqqtobio.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gfrcmtslw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcxvgcfjk.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/goiyuoqpo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggqgijqnd.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gxlepzcsg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gvsnssmxz.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gfzebotog.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gvowtkfql.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gmvazuixh.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gcsvigmjp.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gzpinyfbt.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gibpwhrku.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gpviycfew.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gdmmqdldm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/ggfjzdxza.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gsptamgbg.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/glfpqsdoh.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gvzxknool.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gxuavgdlg.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gkeboyshd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gwwpjwfhm.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ghsuzqrry.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gcieqpkke.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/ggagqiewv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/golblnpoi.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gdhdhbczy.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gflkgbxam.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gpkulxyrw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gqlrdnrlt.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gamrswacu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/ggnhamzbw.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gzygogzgl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggmeersnh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gmhhdrxll.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gxvmfrzeh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gpmwzmgik.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gyxlkpbzv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gyzubpoxz.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gxwaurogo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gplrlinhe.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gjvlhssil.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/ghkowhihi.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gfscfelno.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geftxyipr.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/ghnkdqlkz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gkvnlsscn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gxuyhlxel.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqwhofyeo.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gqeebgwar.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwhztjfzs.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/grsswkepm.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gascpinux.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/goxtogtrq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gcmpappfr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gitqexxdr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gbvkpeojw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gxpgreiwh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gdkwgtglz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gtzhjyvrb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gjtbdfvxg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyhouyjtd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gsxbkrgie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/glrwfhits.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gmudzlzth.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gzsosrnnh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwarnkjha.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gsbgpennv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtlgvptis.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gwdssidfs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqcosnc.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gyzpzkspg.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/ghpxcejag.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gxwolmoku.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gkvoxpzlj.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/ghmozahgv.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/ghcgoyhhe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gwzshhtdk.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gtnetqqfq.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gxwuwowez.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gfgirnocl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gurpfykfp.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gwyqnweqg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gpxbxecav.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gxjwlebav.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/grylkrakb.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gbkzcohch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gwjlbgfyk.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gnsnyhxok.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gktymtiqg.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gpmmzakse.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gqleomsws.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gobfazsxf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gqaeyvzxx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gkemkedxq.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gmcgmvpsc.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gppezfyiq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gvcqwnagp.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gipzucrzo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnzkpsrcp.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/ganboizsu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gouohqfeq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gedtrmpjj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gisjyzykk.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gxstlbbjc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gwgcqggfs.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gnevarfja.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/ggcostkdb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gkbezanbm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gwdnkgxcz.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gmsxtvrdy.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gqpqwtwhk.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gqbizwrha.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/ghlhvwjpu.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gkjzsjknt.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/glakkfzbu.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghxlfnadt.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ggublfxpn.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gnhbahgbz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gwxjtkhwh.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ggdvnxquc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdphwwnhu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gugykivob.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gpxlmireb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gnqeohydk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gspntqzuj.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gbuprllkt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gepjadqsi.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gbviqcber.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gpcgimdyf.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/goqoeiwho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gddqdguvq.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gafeyoahv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gxsvrpypg.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghmnvbeje.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gotqqrvbe.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/guachdqby.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gxvozukzw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gyvssxycm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ggodmlftl.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gimsneaas.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gpuahrmrh.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/grnvvdjdo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gfkihodav.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gmuxhatfb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gpvulygve.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gqexacvnm.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gtmdchohj.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gavsxzvog.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gbdbbbqqz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gmbagadhz.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gclcbslli.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/guhljitmy.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ghgodybbq.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gultdzpai.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gvoybpdpb.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/geaotlfns.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyyxaqzcb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gybrnjqlt.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gewjywwxx.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gsqovwerv.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gjrxaalev.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gyokwrafr.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgzldvo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gqbdaqslo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gfkjnnstr.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gnrxhqpiz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghunwsndj.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gqgcilhvh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gxcbzcali.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gtxlaioav.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzsmmiu.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gzhzynisn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gaungxcvw.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gragimyve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gwcbyzcgk.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/garrrxene.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gxxmgghfo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gmhzsoeza.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/giuwrfxtl.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/ginlrfyqz.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/ghlsalaey.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gkydhhivc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gxahudlfn.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gxkspslxa.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtjnmlnmz.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gbhzcmwee.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gdbydlcgd.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gnsoyzzae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/ggqlowteh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gsovurjlw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gnkmxctwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/grtytdvlr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gzgipcmcw.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gjkkbjukn.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gfxwmpvne.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gsjaoqkcn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gjhtvzuad.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gcxnnzhbs.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/ggeecakpk.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gawmbeldz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gekuodacq.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gilaemnws.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gpqxomxkw.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gfcrxnggv.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gzpzguhrk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gbugoivkl.sHtML


<!-- 参考信息 -->