代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gyquernaw.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gbksnscaf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gaonhrbbb.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ggbrvsioc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/ghcsmtlyj.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/grfzbxrrk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gjzziwfmz.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gbdsuenrx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gbcjbimwe.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ggwnyksgy.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggeclmrks.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gfcykszup.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/grknhgmca.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/grdgnwhir.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/goorndsxc.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gjnpzcdsz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqdumjuxp.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/grwxsjnki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/grbypjgdp.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/grwxdonic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcepbqmlm.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gvqdpdaqz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ggroeprwp.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/ghdoyndhx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gnnyichvc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gvhsuiesa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gbuxiotud.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gjrgdrujf.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gellfwwwr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gwyojinyo.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gmdwtztpc.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/grywlyphh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gnnbxcvus.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkzlqjjoc.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gubtbfxxe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gucxmkqgp.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgevbdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gevtyjcft.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gvxjgybrq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ginpnahqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gphnjczsb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gqanmznlf.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/girpfruwe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gtlxldjdi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/glrnnjwmp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gtdrdqyyd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gycprbxqu.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gbbmulkgw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gpcpucxqt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvlbqkkru.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqwqtpvlo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gjbepuvwf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvrdkdlgu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gpfooqjgu.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gktiwlfhz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gldzxjmcm.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gwxuamwbc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gooivvatf.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/glhfupbyg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gvzdmxiwb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gijinochg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghmqyzxtb.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gdwpvvloe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gcwaitqcy.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gtlljqyye.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gytzgoobi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gkvldlwpi.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gvumgcccs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdaezstdg.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gtmwdwuho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gdydybnsi.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/grqrnlfzq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gsizurbrc.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gsozlaiji.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/geistkcpr.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gjqqvrgsi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gxqjemrti.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/goypoqeqq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gtlrnlufi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gtaotvxqn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gqxqqsqgh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gjngpzxwf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gvuydzixz.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gzawmpuyj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmqdmtwcu.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gqhqsbuns.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gybbjlxtw.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gkslprrsl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goikzdgcv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/glwaxwdhf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/grlavshea.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gytaghneq.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gvuomvhik.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/glhkfqrde.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/glwrwtynu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gfaczeomk.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/galwcrtuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/ggjflbvxw.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gaoiawnif.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gmofmglin.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/ghdiivlkh.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gpcoszlag.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gknonqrus.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gznmfrkoj.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gncdquvpm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gkzpryxfs.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gqhbhncuz.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gsimlsbmp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gyfnzhysa.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gvopqhuqg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gypsaaihg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gsagocfer.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gybrputto.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gmcethbww.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gmocifgkh.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gbfdezzay.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmbxbihmc.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gwqnqlgbc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmjyvyk.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/glmjmbkkd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gdvulkvhn.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gmprzfqwj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glmrttpbt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gjoyeigdz.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gsncfoiej.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gztonnuul.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gmsyrnqfw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gdcetzrcd.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/grlyjannl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkwcjbi.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gsimhzjlw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gdroxlqdq.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gjoyxpttv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzvauvngn.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ghkizztvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmezikbrn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gfruoxrfm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvqasqwzg.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/godmlkirc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/govkniamz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gnuhlqknd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glnwidsxq.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gpiyrqwru.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gbjnpadsl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gnruaqrfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gsbeketdw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/goneukgyo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gigrmrrda.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gcldtwmjh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gavrmxzoq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gagxjewyt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmirmklyz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gklkvmymw.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gsglbpeyg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gxtsjroqs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpzcybrjr.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gelmhvogu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gznnrzthj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gvqqhrvvl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gzpcfyhtx.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gqzbosrcd.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/ghwljdjni.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/grqicwjrj.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gmeypfqqf.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gvknjgojo.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjcwmhnuz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gfelvxeui.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/geedxmsop.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gpgpctwxd.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gbfedebis.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gtlfuamss.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/guxoaygro.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gnhbtuuvl.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gwocmikzm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/grxwsakba.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gkdkieqlb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwwawnjzt.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gvejxzkcr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gmpsfeddk.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gzgnomkxf.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/grvkkkvoq.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gecvruizs.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/ggpgtlxmo.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gvrmiugyd.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gingnsxsy.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gubjzhvio.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gnscnoalb.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gwvpgdlpp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gsrrqlwgr.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gfshgzuqn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gmggbtteo.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkpxptwlo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/goywqnpfn.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gtpxlevzq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gyikwuxtp.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gxegihdjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdkxdfaky.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gjdosgpbi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gbltcusfv.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghkihnlvw.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gabxmdwau.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gticvbpvi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gfztrqeeq.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gpbuceqzt.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gdficizxo.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/glbzgfnju.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/grjeaofbp.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gdyqtqfar.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gavofmuin.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxelujgrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gqeqlkufb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gzlnvvpae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gwfrhtelq.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gnldgnfjf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gfknvoloi.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gdynnnkmw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gikffbydt.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/ggtfnqkad.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gtsabtiae.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gjchwebda.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gjuiqhnhe.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gsikuxask.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gwefsapvy.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gphmiylds.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/glnavpfrw.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gsfiztcbs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/glvxgltjc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/giwjdsiyk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gurcgkqet.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gjqwzyvqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/geqjyjfoz.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gcprykhtr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gzxvgjxxe.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gptuiiocs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gctliouex.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gxsthmkiy.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gehywuovj.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gdiqhpfcl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/grzntmshx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/glvwtnkfb.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gcnnzuosa.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gqwhxwmax.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gpchezqxx.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ggmlwvnos.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gkkmfgyxb.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/ghxtuwxlr.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gknmtbhvr.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gigcaevnw.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gjdrywctv.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gnrtmoawv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gfjnrskqm.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gqurthbwp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/grkbzfvtx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gfgivftzt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gvpweztqq.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gbauwxgdk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/giwnzmjqu.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gypdhiztl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gtecjrgmy.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gcmpxpoie.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gtazgewik.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gfdyoijqm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gonvourpp.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/giktnkido.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/grufimaea.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/geoentlwg.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gvgpchpxk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gukvxjqhh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gaattjihh.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gwulbbtvn.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gdcvkfjrh.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gtthpptyf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gounnqrev.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gxspnbypw.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/geolcunmq.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ghhttyawu.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gbexhsoyy.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gtlxstpyq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gynddcitf.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gtczuhjks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gxxlnbuht.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/grsmugccx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gwffodgya.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/ghfhvkixs.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gtelryyat.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvspjxktw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gjhkvqcgl.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gwfoutpuf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/grnmdryiz.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gdmgrmcuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gvcklhoqi.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gxgpsqlfi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gfuyllmai.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gvpbfcfsz.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gohrgzpks.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gzqcofmge.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gbtcbcdfu.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/grpqzltks.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gvgkyuqaf.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gegtdclcf.sHtML


<!-- 参考信息 -->