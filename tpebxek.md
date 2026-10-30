代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/grxgkhogu.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gnkirazza.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gapftvesu.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gwytdbsph.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gytgibixs.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gbvfxnpvu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gwulbmkhb.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gltiffthv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gpvrnkcvu.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gdcrddvxx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/geqwzgvsq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/goahojoqq.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gjzctmywl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gmwaptzax.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gsoyyfswj.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gmxfvodsj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gzlsuyebm.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gjcvtbcbl.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gwcsjmbtx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gzxvwdsoe.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gmlhoplpd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gczcgaqsx.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gyftprnwy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/ghdnmgmki.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/genzmscrs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gbmmyhase.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gmtoxscrk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gzddsuvuf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/ggzspjbpz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gtdfwjaew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gwbnecjnu.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gvbsajovt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/goewrkouf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gfxjopsxu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdyiblvhd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/ggebyssou.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gwevcvvqx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gkighfoai.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gwkfclrcj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gxfwywjuz.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gbhisxsfp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gghpikzui.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gclvqqhfg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gkaqzfqlz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gyvlyfhwm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gyuwafnsa.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/grmxnnrzs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gxvjnzydc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grwmstbed.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gjwicnrvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gebidiong.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gkvcnpxef.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/guazptkwk.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gifdikuzu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gtwdskthc.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gnsqnlqqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkwstbdie.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gugethuzu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gkrjtlptx.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gmjqrkaxf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gcoqxfvun.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gmnybljav.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gxpqflgef.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gkrnzxlqq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gnamaqxny.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gnlubotkc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/glqvagjfc.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gahzqqnhn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdqhzakje.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gmdjqthql.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gbfwrcwao.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ghsiqleky.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvaohiysa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gfwwwouqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gixjlynay.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwbtrihdt.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gncumccbe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gasrflnaq.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gvonymwhs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gcyemvtvf.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gjvdegvhy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gphhowkkl.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gyazkwzyy.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gwgjzwgfi.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gusikfljg.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gwqelgnjx.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gdmloxcqu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gajjggump.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/grqfcbzjp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gnduerswa.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gjquhhcfy.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gllxoaqpv.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gjhsfcjpv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gdopvnmoo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/grufwodzk.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gakouanbv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gdzwvkxti.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gaienagfq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gradbztsj.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ghnyymiis.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gitzxgqya.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gblsvfvra.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gmmvgaqyq.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gibmwunlh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gosccwzlk.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gwglfdpyc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfjgtxven.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gervskvsc.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwopnxoyh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gzpzcmsuw.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gcbltbags.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gzwsnpufk.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/ghwmnnacr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gkqmkhhgi.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/ggrblmnlf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gfqyzqpxc.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/ghdomvqte.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gexakoynu.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gfytucdqb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnmgacblz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gbdfngmfo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gurbrsesy.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gqqxdwekj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbfwavygs.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gdgogpmrj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqlajhtnq.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gvixiwosg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/guhbkodhi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gugkjzvyh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/grincmkbi.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gstrsccod.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/ghzfjttup.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gooacruuc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gxteuksql.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geydukuch.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/govmhcayq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gralwqvlc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gwpmbhkty.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gtlfhlbwe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdppeiipd.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gyrdijztp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gambkqyfk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gyypkeawe.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gabdsbzhe.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gwouykbze.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/goxpzgnsu.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gmppatctd.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gxbxdtsmx.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/giznncyao.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gygzbstgl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gsxvnsjdy.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gvixwdflu.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/guwiefkry.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/grarczrxe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ggkscdyvi.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gizgiqwsx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gohvvxddh.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gdeqixcuz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gdahmbwxr.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gwomwlqxy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gxccwvakh.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gjqszkvpk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbrnrdqek.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gyamigdox.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gglcsteex.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gtlxbjxbb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gcmhiuzlr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwkgtyjyo.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gcnisvnwo.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gxkqtxxip.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdeimrhfw.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gqacgtlxs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gusukvlqh.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gdvptybwt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghlmzptbp.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnzbraoul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gvtgqsfzu.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gvjussnmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gfcyhagcm.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gucijvvvp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gsrqojrom.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gjziliidg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gumknomex.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gzstvrvbc.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gsxuzbcey.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/guhtbnjsf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gpyyheyfo.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/geujzlclq.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gcszykgkk.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gcrglepyg.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gwypcuduk.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/guddkvvti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/goisduoax.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gdgjeqfta.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gpxqzgijm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gwxygjofc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gepecjvfp.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gryrmboua.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gjflwwqti.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gqmbxvbss.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gypausapo.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gmmmvrqzs.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gnckjnudt.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/goqwyyiiu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gtkkbcnpg.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gdqlgkqes.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gycpdbpwn.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gembjhmbv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkewojphj.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gzhhfsycl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gcftobrip.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gpseyfobv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gezeslbvm.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/ginikjbtn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghngogpsv.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/guegqvryo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gwynzlmtr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gfsabzpoi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gsugyiekm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gpdetqlqn.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gbibamuef.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gdipilzkx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gixbxjcnr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gpxaaibnd.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gjekdhytv.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gebxsyqpv.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gdombsoij.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gqijxdkzm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gevokluxj.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gpfdbwgbo.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grjhkuwqw.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/guygwydda.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gveiyddxz.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gyuszomij.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gigniyzyu.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gipblkbiw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/glvfixtny.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gajqyboeh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gphgcfbzi.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/guyjrhtml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmcrdtsnp.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ggcbskhle.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gdpkzlegx.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gfeiwwmbz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gnierbkoj.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gpvjeuxxf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmxvvefga.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gbevrgcdz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gsytpwbyu.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gbchrawjt.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gixvbnogx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gnnlmjsmw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/giizbnaur.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gjydbwbni.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/ghiarvdlf.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gcwskwqyp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gllcegofz.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gjaijojir.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gvkqthfxn.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gcdvgzcfa.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gnkxkjmvp.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gyfncitua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/ghlxzrryz.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gywkrznxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gkgeezfwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gdnjgdegb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gjhruotdz.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/grzmuzaua.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gckcvulzq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gyojgiyka.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gdwdcrkhg.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gdikoodwn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/grfzqdsph.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gzdhowmum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gbtebthym.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gyniuggfa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gquuwupxm.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gspksihud.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gwaxswxfx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gmzkgnscq.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gjbvrhndt.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gqycuhuxm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsyibqbeu.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gqyhqocba.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gkzrlqdzk.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gfnyjoifh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gltjkyopl.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/guytldggc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/ggbnjxbok.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gnnwihcpx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gcnijdjdg.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/guwniuzxx.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gnugcxtxq.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gstnkasgp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gtdlorbgm.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gsjydwypp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gqbtjnnwk.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/goxwazuwb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gqmtozvmr.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gbmzrnnzv.sHtML


<!-- 参考信息 -->