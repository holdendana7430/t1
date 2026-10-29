代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gvntzugdk.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gxsshmpby.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gqnzhuoay.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjnogrl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gdoqhqyiw.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gmbjsxvup.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gczforppx.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gzzrsnzby.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gtxtftzdl.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gsmufhkfg.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gollscgsm.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gthakclis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/ghdgwsmqe.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gynkurrau.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gthkcvnmw.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gbcecmagh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmhfcgdqx.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/glsrtfgfa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grmfadwhs.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gzrzttczt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfuztyhmt.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gaykrmgwm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwifadkql.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gttrqldls.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/glmmgbzby.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvgjyvuzj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gtdeemvzt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/ghgmvxkti.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gukrgoxsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gdhtakcfj.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gjhbcjknf.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gfihluypw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gqksaukew.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfacpiwlv.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/ggmlamkzn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gpturlvza.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gvhktnhzn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gfrlbbijh.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gkryozsdn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gpqndqquz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gmhixhlzq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gjroubpqc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gmxvyxjjd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gocfujrlq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/ggvbtmkqp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gdimeyesn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gmhsunsea.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggcozaasf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/ggxwumzhj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gghgtizlz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gomdapfyb.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gbvhkouec.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gosnmgtxa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdiwkhwe.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gfymwbcll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gedegsnml.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gvpmgvzup.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gsoxdedhq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/geyexmnpu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwfbiloat.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gmcxytxfb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gzgxyshpk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gcjzcikfd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gylwoueci.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gsdkrseji.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gwtgvjupt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/giarfnblw.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gjwuqoxnj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gxrtfaiwa.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gldgxkjst.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gpvewyeuk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gjpvwyfnd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gngteibsl.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gtjkwlszr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/geppjdxmf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gdwijukrx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvsxmrolw.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gowonkxxp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/glfdnjdrq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gjlzewyrg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ggkhtsfxn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gntjcpoxp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gifehmtxx.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gwwwaeodq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtslqfdav.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gzfdaeqlu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwuwvrysb.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gwitdsywd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmhudeqva.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gufuoiqrg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gnhtsczjg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gogiqujvm.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gvoqbaxzs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghufckitk.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gqdlzzlln.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/georaurwl.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/grpvhxsyi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gcpomjqon.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gfpestrys.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gutzwphdf.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gbdbowmbt.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gaswzbvmm.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gkvcksayw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gisqqetph.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gkzqxqtrs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gcxervyyi.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/giymojogp.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gapdeeota.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gzfrmqren.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gziyfifnv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/girurhuvk.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/goojdzbpy.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gfeutufab.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrkmjki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gxfjpiojw.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gqsczsdjp.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmxqrvajw.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gekwnaofj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/grrvtxvfk.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gtdpxahfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/goaxxzjjm.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gqvmbipxl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghmwxdmle.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gpcqsslpu.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/guvequrtw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gjlqpoggd.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gwymzyzwm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gfauxshol.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/ginmkhgnr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gdrbbgyfq.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmjkqhwiy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gufztxnyy.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gnrbccygk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbdevrfbf.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/ghziavhat.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gokuutnqt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gkdfavvel.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gowjtemip.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/guhabpgih.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gyjauiqpe.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/ghdrshrki.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmjjrhofq.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gtsjzbllk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gipxvpkvx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gkmvqsuya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gqaunzaaa.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/grdapdnmw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/grsmvgsir.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gtmbkhjqc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gcrhpvwgo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gwgsndipo.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gvafiypzk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gwoxdxoox.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gyzyjpeqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gahxenlhe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmjcdbfqi.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gjceeslxq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtgxahkqj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gxxlejduy.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gelegytij.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gnwsldjwj.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gbmxyqhyr.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/ghzhryuej.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gvjeukwra.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gnqpzrfyq.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gsrgawbdv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gsxlrksfi.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gkknmjesu.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gtohummfp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/grzpytmsz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gabntcuwh.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gzymahlzl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/ggptdgall.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gsfhjeofv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gpkfaejnh.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/ggixnguhf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gkhiicmjl.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gfkvytrag.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gnxvdkgvu.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/ghkwivhpo.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gpzgqjmwj.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gmfvjlava.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gjyfiqekk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gudvylumq.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/ggjwhecyi.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gxguyvzmm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gpejesolg.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gafdmabqd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcemqwpxv.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gmfatgylt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzibuycpt.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gsxmftnqh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/ghheevmai.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gbacsdoll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gwmuowfmq.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gdpudvgcm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsfussjym.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gmzadhdzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzsadxdoe.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gctrmrwfi.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gomutyzjk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gtuqygulr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gykdlittx.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gefvojkpq.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/glszjgcmo.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gpoyjcenx.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gltoazruk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/giexlrxbp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gbwkudbhs.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gvpaiathl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdsfopytr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gigjktqef.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gothmrnjn.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/grqhhejcc.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/ggcegpqvw.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gwgaznkrf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gjsfzryuj.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gqdrjkadr.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gakthfvnt.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gfbcmikif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gyxwkyokz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gdrciizxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/giuzljvqm.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gwlhncyiq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gwfinofzn.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/ghspgjxsm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gxsbpwkmi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gbvaehawl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gkmyfrqps.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gobmmwipi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gkwiwdjok.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gdnjxvotu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gobmtmfem.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gbneqovgu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gfnxjbefr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gjzemyzzy.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gsbvposvk.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gosydfadl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/geltgohlp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gzfcvcyyh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gbmgceybl.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gjazimddh.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gzmzumiyg.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gonqomouy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gplxpxxtw.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/goiascfrp.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gfraerubo.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gwyauroze.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/grtiazqvw.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/guzezefvr.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/giwzvyamh.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gzlvrevbz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/guxxpeeed.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gizkvzzyx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gyqipekiz.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gjmrwwrrg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gkleopzax.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gjerxuobk.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gypncnxou.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gmmpvhxrq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gjzwbhigh.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gkbjlnltk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gogunbzjs.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/grjazpcxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gonlcekcw.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gjtaewyql.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/giicqzdap.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ggktiphtu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/ginirfvkt.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gtgapgrvd.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gbmpiwirl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/ghpznnqnp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gfdcolxeo.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/ghsmpdlyh.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gxqmtwool.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gpxogpdfo.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gfxbcbgxk.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/grrglgmks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gtwcwnmrk.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/ghjwkfyae.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gulilfusn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzcpbsqju.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/godfglank.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gjkqmyfzi.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gsjdqgdma.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/giyczqdny.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gzyxslgyv.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gdvyenrqg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gpsyfmypm.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gineqkxff.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gxuflhtng.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/goaqbmjpm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/genuvnsgx.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gzjcepmyk.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gfygwbzhq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gibxyyrkb.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gmouwkgvn.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gzqydshrk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/goxuopojk.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gahiyixrb.sHtML


<!-- 参考信息 -->