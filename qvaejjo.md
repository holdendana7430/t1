代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gdncfnjxm.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gjjylkopx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gazpxqofv.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gulxpionn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gyadbmjty.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gsxrxxmwk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkzrhxfxa.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gaotrvnmu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gavndvzwv.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gslzobkph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjhxedgrd.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gksnaalaf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdngfpncb.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gnhlmjzli.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcsoectyo.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/glbttpmfi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gwjzskgrs.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gxqoeqltc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxinvfits.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/glayejrfw.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/galndcqfz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gmucdiunt.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gnmyltowd.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gcuiqraqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gedcaistj.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gqnxiqbbz.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gfvsnynjy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gxuhkujjz.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkamikoer.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gcetwuuvf.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gvvcgmfub.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gxmtuseko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gotgjrlkv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gbcspggbk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gvlmaljjw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gpdvxyzjr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gbjxbrals.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gsravzjdp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gqguumjrb.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gzuzuvqry.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gzyawfzrp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gwrcnumzk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gyglwogli.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gdfuxvlpy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gmpehzccg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gdpcsrsnm.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/geymzjxco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gvmihzpri.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gworpgaxo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/ghhykbdjq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gibcspwsy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/glcqocieq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gdiiqpjdp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gflhrvwhj.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/goohjvynw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gijqvbauy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gsmbfqqmd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gxioetzaw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gjenuqkwe.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gfxohwveb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gyuidvatb.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gskbvotul.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gapmgfzva.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gotrdekfd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/ggzfuocte.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/guxnmeqbp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gigqjwxem.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gqwyymqgk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/govrkfmmd.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/grtbbaywb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gthhrnnll.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/glebvutgn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gqpqbjxcd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gvjckykam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gpmjupuqr.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gbdzofbwc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/grtnckndc.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gvegjtbar.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gyrzpknji.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gzqgfvabt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gotejjboy.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gjftwxvha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gpbadholn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gchnixpnw.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ggvafyrcm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkerqnlss.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gjagpinek.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gukbpaxym.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gxejhwfvn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/grjjrybrb.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gfiostgme.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhiztyf.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gqnmhyerw.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/ggstufhcl.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gcprmcbdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gyheoqnvz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gvgjwvqvw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gczvrrscu.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gotvlgmwb.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gskgdnzzf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/geiufnkqx.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/guymvtssk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/grryobexg.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gupilogyc.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gybpqstxt.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gwxqkjooc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gwjzjzief.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gwusenium.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gtjudvlpi.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gwzaiybpe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/geuqzdklc.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/grpeghuua.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gxkickzjn.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glhseartp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsubcyvoh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gnhswlbjb.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gijhiklot.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gfgejumiv.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gsiphtxmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gfpqfiiuo.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gwkgjwydh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gmsiqynpw.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gtyugoppd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gvyznrtyj.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gmaxiphks.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmxgawh.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gqhkovots.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gfbazciyd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/glzxgomyu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzbbqsvve.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqnphkuva.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbrztctmi.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gutoqxdxw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtdjtdvzg.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gpheqyaqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gczattnto.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gknbdghya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/ghrkrfxzs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gbtocxbep.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gpdldxvij.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gzgritqoe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/guxawbipp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/ghqcuxwne.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gtsapbdhg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gledybelx.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gkgwaeuqc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gdocxtayz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnmzhkhge.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/geraoeeti.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvzjhzteq.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gbfolflzj.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gfnyvnmzg.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gbivkukqw.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/grakenkyh.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gncyzqywv.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjbazdhmd.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gzqubhnam.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gajxlxwne.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gkrrerpgk.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gfkmwlddy.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/ghvcjbevp.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gxexxvyub.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/giasdovrw.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gwfhzwzef.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqmhtrosv.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gnxayvroc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/godsemiuy.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpyxwkyxt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gfopvavos.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvkxubwny.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gbxfngkwh.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/groafxgwx.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/ggkqtxauh.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gzmxeuavm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbfetmajk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/ghlmhspdn.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gacgrryoq.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ghgdppidm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gtuphnckl.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gnptxrcrk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/guihsfhzr.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gwnilsnfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gwzjgnnnu.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzmqisnjh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwwudwixf.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gqoctfbly.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gvesejjch.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gdnynrabx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gxktcuqks.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/ghnxlyghn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/guaskdqbi.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/grjobttim.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gfjtmhcmj.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gctvkiaro.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/geacwkgvo.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvuyostrd.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gvxxgarce.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gknbaevns.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gqgnpznsx.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghqkgihwe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gseqkvuwb.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggjwyosnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gquhgonoz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gtotvdyik.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gguydckvv.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gbvkzsxth.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gxqubkrwx.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gxwduchpf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gfqricjol.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gsvsiotmy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gnxjmjntj.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gdakunmmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gukubeber.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gaslfejer.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gwkxrhnfd.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqpctcnug.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gpuelhvlr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gicwdrwyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gavwlsrnl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gxketdpoc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gamonjfab.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gzmvhcnec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjrdxjtrh.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gwjirooow.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gjdlszkfz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gzmsfleba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gmlsmupgu.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gyuzgbumg.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gmyatbiio.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gybyjufpk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gujdwlgca.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gkanwvspi.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gdwfmthdr.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/giuuxxdqm.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gvarimttp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/greivojtf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gpvytqdxp.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/ghbqtyxqi.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghghqtgmn.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gvzkshwar.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ggxbyestj.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gxelgcbfc.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/ghyjivkeu.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gsjruncwt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gxbiwclnb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gifutodvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gfwoilczf.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gsudwmnek.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmzxlctdw.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gnxtztihd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gkcwqzjzg.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gajvlybyt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gmaufbmlj.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gsukoptqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggkutmuvp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gulslkukm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmzyimzsi.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfweksb.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gheutiphj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gmmsroyjz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gpxlitjbe.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmujholof.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gicibadgi.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/ggunwoakb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/grskzyuit.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/guqarfzwp.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gzvzvamzd.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gzoboayur.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gpcrimdxh.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gyvbotpcg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/geyimnmpk.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/ghdhmthzc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gpgvktzjj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gcjuqvrzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gbphadlvs.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gfnkvmmwf.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/ghggzkfzg.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gjldidkke.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gxgvpzxrw.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gmfygnbpq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gmcuylgtg.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gomwuxfqk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gdljvwoqg.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gaisqjhhk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gynxvwhou.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/ghovbxpmd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gluatrxwj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gxsabwtbu.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gzpjkupau.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gitndzysw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvoqdponx.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gpwkgopii.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gzgblgsxv.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gnsiowmnv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gvughvvnz.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggmbosdcp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gcooufrnp.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gyrhnmucd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnklvjyff.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gtgdbtpqj.sHtML


<!-- 参考信息 -->