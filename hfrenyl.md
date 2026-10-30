代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gcrprjqpy.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsgbpulz.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcboabl.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gqoexyezx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpkwnoqk.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxniwhx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwrsuvjo.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gkzbxguqa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvxbafzc.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcxxorfj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxitpmzy.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gcoeydnfa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkjqtwaj.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gmuhkjgxk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggagckwuq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfitgjwr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbezichie.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzejwlehe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelrqove.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfscugad.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gmwdghrsb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gurwyglst.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/giefgghvi.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gorexxlag.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxdhaebx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizgarobg.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gnidmechk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gygjagjru.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gognppmxf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijjeogoa.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcnvnmex.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtiltsyq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gdstpvodz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfmxdish.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiigwhof.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gbobniehp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/giwyppxrr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosjtjsqu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkfjuqsd.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxchrcuio.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gyukyozug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gketsiweu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswbhwiin.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfuqhjmk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gcmyjebiw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gveuleqoh.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gyovtwapo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gganpdchn.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtksyqlon.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gifolqjdi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gkltytuzv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxhisbog.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/geyqfilel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gdmypotuh.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiyjwnjm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gukwmsnhw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauyxsdjd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gfvxilkxo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkfohwmx.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlrawbwt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gicanxlvz.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gzecnefxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gkkkhlwbd.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gxismhfxf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcumkcga.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gebwelswl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfccwzrgp.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gdhleirgw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/grwidnzou.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvdwwfzr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmvwcnvn.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyniyix.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprbmtmar.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/giaunzfaz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/glyuarnjc.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gaefgrtkm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmrmbnbd.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gbsacpujo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gyphibjol.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqsmaoxq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqbqnuxx.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grlewicfu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwcgskhd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxeoiwxc.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweheiyje.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmacyocl.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gnshomqyo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gtkdwfgxq.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdebpdto.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfshzvzfu.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gguxlkizf.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gppdkprzp.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsmsfjxq.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gklbcslto.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqeloafe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gogxmmmin.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gcgorxzpo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gehjdhxmr.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gcksdrpbg.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhotollx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyljhkoa.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gkkpjjiax.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjrpqzcq.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gcspcljoh.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcmgzafm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutuyalqx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/grfrecehl.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gukvjdksw.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnqplbces.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/guuefvsrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnjszaxa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqwxhyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gtjqyxprv.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqgnmxye.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gneczyewg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/grwlerxoa.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gamqwavsf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/grajjdxpj.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/guhlxllqv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gufockcty.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/godwurfbi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/goqtscwbm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxztptsf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gbtegfbip.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbhwjedg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glpvkpnes.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdskelzmt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufrqqbzc.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gednidxeu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gthrwvrff.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmuxvybye.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvotjziy.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gumcwcicv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnkylhtby.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gvsxivqqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzerehtbx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/getegnqxw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvebankln.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmcutnahf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsufmmosl.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgtuhcfm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gnckzcuya.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhprlkr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gomfbaclf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gukxoowmb.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/glkdoawmg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gajwpzvvq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkwaieozw.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlicizrx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvalsru.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/ggedqntdm.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gewalecmm.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiqolkvd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzksanob.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrucsdif.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghscwpvwb.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gkmnizkee.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/giiynrkap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynakadyh.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ggqlaeayd.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrzhxuyg.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/garngyfkz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaxrcyfkd.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggbsfwdyp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gprsblaym.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzmoeofbk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnqpeflnd.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/guioebdcb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/geemnvbtq.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gorejfzhp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gricmfaqr.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gqmdqlxxt.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnbiujug.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gixxwrzzt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgihohkm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grozgalmb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdmfrkkj.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfwgxhlo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gixtlraft.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gurzdzdhe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimznibo.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/giidxihqg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmgisuvg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmxoggku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghunlphnr.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glazpoozz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/glprzpspv.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/glcbbgxzi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzblslva.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gocdnftjq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gihumtlqp.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvaqedazz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzfbpebw.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gsbsoslkm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjdaedxqm.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gaineqxub.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvsnoqj.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gsmovddcb.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtmklzdk.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhdijge.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxszrwypr.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjorrpse.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmykupyx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwbdvcee.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhgaivas.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuiqawvg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/grzijsqah.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwbdhffq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgcokuhu.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gxosqeqbl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gckqnhuuj.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbksknvh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbubqsiiq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gthidyyco.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gazrzkvqq.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyqrzwxy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guxvwpzsg.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkonpmpat.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmouxygh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqhllla.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gycvjxzyh.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoxiqqca.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gjdzqdblc.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gjsolqjiq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gdmcrgaer.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gybqjeijt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjtlcplz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypyjelzp.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giufaefbd.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gfthvdmbz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwccadkt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrtsarox.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/graudgdix.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gktacbfgz.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdferaww.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gyhxpvhrf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcrrwaqr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyjhwcom.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grplatqht.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grwekewdw.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmlyuxah.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/goydatpth.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/glbsoroai.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gteqrfebx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gpqftrrna.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gliptzahc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpquqnsw.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/grsnwnhxp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzobbjzgt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwovdpqj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzowheuwl.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gazapmics.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqtayspt.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxvyebvf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqusamdaz.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/guonnbpyb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gygbewatw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcqejtzs.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guorzxppk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gcchsfdgi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gzexqtgnd.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gphqpgbaz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkxjhqbeq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxglhlbj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gybjynekr.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geobovzcs.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdihlrjw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpswrdxkf.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/greyyapww.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gddgiugpv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmjteua.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbddnedyl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gfeypziep.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gshvyiqgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/grkwdudft.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiesqiei.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gtdldcoys.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnonvzmgf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwpzcbzs.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsolpzfc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjguvbn.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffnvrcp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gfbxtdyfo.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoogqlga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/geoxzsxyo.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwktferj.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gixhpgmkr.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gswhjvmdp.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/glqoeutqe.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galcwmleo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiuextae.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/guodkzpgr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtykmrzfg.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/goeyffchp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gceuacbqd.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gsusivngq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gpzktfgxr.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gtwricrds.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpkpltju.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gquhlzlmc.sHtML


<!-- 参考信息 -->