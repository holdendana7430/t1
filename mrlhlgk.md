代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/giyvrdzjv.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdkahmk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjqrwezx.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbccdniof.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtcfiskc.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdldulpj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gujwpilec.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/geytlvupe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwtzshvp.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdupujpa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyplimirh.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpnfygdi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpvicgad.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gvutycfdm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadmerpqz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyrpsere.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdxijfl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gbveqsvyj.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gcomuoxyh.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhmyzasz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gtriesmys.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpyradxv.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfnlrsuk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexingpc.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/glzmveutv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhaapgsr.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gdmhigfay.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzpbybrct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbivcqik.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpwrktgl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gxfknionw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gdruubnlh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gamnvzvrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gpbazjauf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrnwgwol.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/garazbclp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpztkyhho.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvthlhbs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpussmvve.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/giagadgbz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gxsyymhvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcpgpqkr.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gmffzhwjf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwoliabz.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiblemjd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoxacdzk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdynkpbrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdtjuxci.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnjvskaxl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwwjwlqf.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/godstfxiq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gvrfwnyoi.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsskwxhjv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexamzmiq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gdtxfuqhd.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkifpmb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gajctjaev.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbtbaqfu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gouheacwm.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrvusgzd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gilgjcndr.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/ghbwhouhr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzozcbsf.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gwnzbambi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdspmwhre.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/geykhojry.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmvwevtw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gktgaxrnc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gpncchgij.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gvjsrjfhp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkkfyjazb.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/grkxjgbtm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrdnicvs.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gwskniaee.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gylyobcjf.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gcthfgbev.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnssqvxqp.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gltmanegp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gstxsfoho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gabyhkjnl.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxwqsucy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gumsggyeh.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgeuhrhe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdryeevci.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjijwidu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqbtfgqr.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmifloneo.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhrmuecr.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gphsqejpk.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzfbifwa.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gfydpfccz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtiaffv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlqyxlhf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gavhyincr.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdqqmhff.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzxxwhm.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqmoclbgi.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejdndixd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqtwykwo.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gpmvdtoev.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcghiflo.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gzjtuatre.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuldbkyt.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagzrjca.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gobgweehb.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gpujhekom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gppsmvxzo.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvtebxph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gpkbwvkwi.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gelfsdboj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkpnvrbyk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/glnzguidq.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gydjzbaob.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhljgfl.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfnbpepy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gxpxjdddx.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpptvwlsq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlqsnqrc.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ghcrfebtx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gtqkbvpxg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubhmlmfz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmuzlmzhe.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gthiiivco.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwhewrtp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guywwzgis.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ginzjevkf.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/grjhhvuwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjveakszv.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gziakrqvl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggunjjqfc.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gfinrbknp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkjgjonl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqwrdcj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdwjfebp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grejzzugy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqwahpcw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gkvhzsqhw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gxhrvyajn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtudmuvjt.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gomhqnwbl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntlmilwb.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/glnyrlxyv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwmcfjak.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gritseoxu.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gidrnjliq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gomswhshv.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gdguyiipx.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/geyeifcrw.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gcfxsxcmy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqxpmbxf.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gexghhadc.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqcsejssd.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoyiezxq.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlxuvvts.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/guqrvahuf.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/giicbqghs.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyucctzze.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghpdnoyvs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwcldigo.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfnozkxhn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gixstxaxg.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcguigxjq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdwsvsn.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdtshnhiy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/geulukyjo.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/glzzodzsi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcrwnvnu.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gllotdnqq.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gdkzhkpip.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvtkehra.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuyqjmaf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrglcvyc.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gefzmlfpx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjnmnvgj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gytjvwiem.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gngtmmjcr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzfyttsv.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gsbqprpek.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqvnasak.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngopwqpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqbtvwyv.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gldfoqnbf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvrbrbzs.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/ggybjvhin.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggdfkbium.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gsflhjkum.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzuszcjy.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhweofwl.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giojbhckb.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gitvmwtcw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gukfaeqrr.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdebiksm.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxkmtbfg.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gzxgcgsfv.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfdcyfqua.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/govtubvwb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjsjleji.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxfmvuyy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvunhumu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gyvvryflu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkpdarpb.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmludkdim.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfsvuow.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gqahamnpo.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gltwtrxef.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gkutckqfp.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gcpomalpd.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmuxqzzuw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghpvbwjko.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/godoicaai.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gslzmeyoz.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmexypqpn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlxqnpag.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gfafozzni.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqcimrgz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gwyvrzzfn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gkilxhorw.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gvmcicsol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiknuoip.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gviofxoia.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gcqupfkcv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlvlforl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsalklwi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqtlnjkn.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gooqjybzi.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkvkozuu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyfwstmd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gzrvtvdbg.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyhbygky.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwsvvrjs.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gawqrfzgn.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjiwcmpb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gxdmdmxao.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gtchczuvi.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauehwfcc.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gybnzfumz.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwubrfte.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwysszyu.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjdvxoekf.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gocrtieqz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwdrjtjk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gyordfcpt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gortmatlc.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwgqvvmln.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaqqrbey.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywymxyyw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeahhrfj.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunhtsfq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/ghecwcewb.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gjsnrrxwl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnnwonnx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsammsbf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gtraclzmd.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggosfjytk.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyofktsxl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxekenph.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqmibbaqy.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbxdgxkqx.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfqezpete.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gbtfonrvm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/guplurvco.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gsamooqxy.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiwncjbb.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gkxgddkgh.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/geylkbtfu.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzjupndh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gplbnnftr.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvtafmztp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoxsjyog.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/giicmugmy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnafxngfo.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/goesqnwsb.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gglrcvzud.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpprrnob.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gicixoams.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwennehvm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gaceprrap.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvehvzjd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozjlejft.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnmyukw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gulghivnd.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpilocjzj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpjlmngu.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gfnhgviqx.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gumpicvuh.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gwkiqduzg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsatytgv.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxccvkozd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvblldgbn.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdbohade.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ghyybpdpj.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvmjopwj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gjzkmzgmu.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ggajqmdxs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcbektkoc.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/glsuiiygf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmntytqo.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgzulnft.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/giqrbqopu.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtukznkef.sHtML


<!-- 参考信息 -->