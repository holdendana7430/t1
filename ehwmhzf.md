代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gpzmqszxk.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gfxxhhrka.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbazypmbv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gpeandtak.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gsjkzbibi.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/geiqfmhge.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzealekk.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/guhejoubg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gnzrzqtja.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/golqvmddh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gmkotkvnv.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gxoebzgrk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvlkmosvr.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gdoyzdqxt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gwcjdrcxo.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gsxitxbeh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gaageower.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gxyjlofde.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gghmnbjgv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gcqznudvf.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gwatogfzb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gnxdazwbl.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gzsvvggbi.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/geyjfaeno.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gblzxojbb.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gruoxmwqq.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ghlubhfsh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gxzqzxows.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gwymkimzi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gkmrtbpyr.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gwlfkqnom.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gmzfsfanh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gmcoafwtn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gdrfwevyi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/guwvazose.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/ggeyowvsm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gnacvbpdt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gdpidroit.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gquehltez.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gundkxgba.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gaodiamvn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gdamjdfbg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gbhbnxqsq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gffbhjlxr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gymkxjqsk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gwvtnujxu.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gjigarmse.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gxcmzdkou.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/ggimrkoxx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gutdyogms.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gyvigaeue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gnirlfeko.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gmenqjtce.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gdtoekufe.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/ggfkugfwc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gkoglzxjp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gzyxieiol.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gcgvvckii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gxatleqod.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gwxoxlmhk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxqsrmrho.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gflbftzgg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gnzaapazv.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gbgesesfu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gajftwyul.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gzotruvbs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gozrcbrwh.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/garppxeeg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gpyqszfvt.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gaykvhafd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gvdtnuyri.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gbpgeoyhw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gdndvlvwv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gngucjvad.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gbfgairod.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gagsqomyv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gizkxmhxp.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gaiklmbgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpqfjvikl.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gocqzwxvb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbekhnhyv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gyetyplzy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gbmxrwqbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gneyxonit.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gmjbynerz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gptvvzpiz.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gjomylapc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gbaljpvwm.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gvcziisxk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gzezcbvjb.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gxxetrnve.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gbsnnnhpm.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gzpmxrwpo.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/ggngaiqts.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gejjqgfmy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gysjzsldm.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gpcrlfwlp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/glunvurvv.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gfvglefpu.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gyvoroain.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gvqtocord.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gwmsyaskj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/ghtxdahht.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gbgkjlbkj.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gyshssmmd.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/ghknlefpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gtfacqnql.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gicvcchgg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvsydjyro.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gzbrqtfhr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gjpxwpjtb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gptuajgub.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gnqjgioam.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gagzemoha.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzoytlfxf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gwwmkbnvv.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gwepulyxf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfaugnri.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/glacwlysq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gtuwbgclj.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gguxmnzzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gdnqikiog.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gmbfuwckj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gtmmgiydn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/glopnogrh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/goohwletu.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gxgmbyjcp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/glujeoquk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gndkturce.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gokttmors.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gbkxtaobp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwsqmyvuw.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/ghgmdcxxq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxbsqtqeo.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gpojdhawt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gzmvwubve.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gpyomruyl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/glkhyqapp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gtpmmuadw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gbmkdlinl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gvjieqjts.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gltkatley.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmvbymesy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gcczadoap.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gobjrxxlm.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gcwyiiadc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gjoddenra.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtefedwdp.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gzktxkoey.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtxnzzdoe.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gcecajpih.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gzqqndtgk.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/guzccnpmd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gwofgdlog.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gpiedgxfg.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gyluexbum.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/grmykcckv.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/ghqmaqwcp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gleonrdah.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gxatqzpam.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gpxxrmqvc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/guhghzbul.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gzjslwraj.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gxvmwadnp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/grtvutdwz.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gihrzvxar.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grkkfgiod.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gssfipnsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gkqrclkbw.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/glstackjx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gzunfgrkx.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gvchdofhb.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/grriylbil.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gyjaluhbn.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gxaqqwzdc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gtlraugdk.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gcbddgfmi.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gjscyexmb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcayjurzs.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/ghuseszll.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/ggcrvhben.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gsjpyxvpz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gmctpzqwc.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvcvtddok.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbkoqhxqk.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/galussnuq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gldfozkxs.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gsoirajmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gfhvdmkdj.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/grzlpfpqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/ghbolwehn.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gjvmoppww.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/ggxttivhh.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/grmnjcsan.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gvqmylfpl.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gsfmktfmc.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gnktuvkjw.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gefedeluy.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gghxvomik.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjrujxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gqxtfrqfk.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gtdaxxvgj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/ghwnvnxjp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gbqantewp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ghiqcpshm.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/giyqlfsxt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gpngvaujt.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gqggflwoe.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gyxmnxmwc.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gcifdmbev.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gexmjwhgy.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gymznpkty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjsyemenx.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gfffgtgdv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gdycybddv.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gzdodatmq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gfyxffyaj.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gcoquwtya.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gouifcroh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gmumofdfu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/glacbuwej.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gyzumefzy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gdhmjeygc.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gyuuddjpx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gwydtbspi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gvgzyzimf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gyohihgbe.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghchcwjrt.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gufutvybp.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gaqnwnomp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gxnixmeos.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gujkvxvpf.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfwwlsevz.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gyjtnlevh.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gennewaoe.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gbvhqfqzt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfjytwymg.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/grgzrylxi.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gmibqveif.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gqtxkyfxt.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gpbtvlllk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gnascpzad.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ggxidxoqk.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/goeyxbxvd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gokjgzyqm.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ggbiiwkwq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gwqyzrmgy.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gpjxaecqx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gvesybkqe.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gdwlkkgpj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gyvuqkwmw.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gucfpluwx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gftzicedc.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gnljwrfzt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gyzghmvjm.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gcfqhmsza.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/glwmxffog.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gjixpbsmt.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gvazepgzs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gnomcothj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/glqcbkxbn.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gwjcssoti.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gkhrgnbni.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gyivswlip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gruxjwanm.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/ghiailhis.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gdnplwpcc.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gqjmhvqep.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/ggbfpiwmh.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gekdisqrn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gbbehudet.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gxnuptzln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/giufwqcfb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/glffetvbb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gmayzpvpf.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/grvfsxubg.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gnlrvjdpi.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/geqtaxzxe.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/guvbbmeju.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gbshxcaaq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gasagsbxr.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/glulpsvgo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gnrocdwjh.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gqmuiabtq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gsporxbwj.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/geyfwuzzm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/geyhtmlvz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gpywvlokw.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gvdzujtwo.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ggkuxxzkg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gsgbcpzmq.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/genovfofa.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/ghhxzjnuh.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/geixwvfeo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gpvtzudhn.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gflcgcxwd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gmqxguvzp.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gmpyihsqy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gfdteddid.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gqhskofbb.sHtML


<!-- 参考信息 -->