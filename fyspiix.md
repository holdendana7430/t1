代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gmoqjgxsn.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gziafnoep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gggotfgfv.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ggpyccgom.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gixxcnjur.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gwopngyvl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggfvurqgm.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gfjqxroqr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/ggfcqkham.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gottfojlh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gemiffokf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gljxoxjod.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gbqvneyxz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gnlucirwm.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gwohryiyq.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gheqmrnpm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gluznakvt.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gtzwlcwqp.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/grseifhpv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gqgmxphba.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gvtbcioia.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/glofquyci.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gdnlqxtrg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gzvibajxz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gxqxcdvwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gmukotihk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gpoutyyfi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ggiuhjjoe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gxdcvyfdm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/glupovkjn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gngxpjqvz.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/grpaohase.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/giradlzvl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gpcizzcph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gimqbaatk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gnsrmxzyr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gnlmloqnf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/ghwncdocc.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gperweidv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gzisszghg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gfbchrdfr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gcczeawoa.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/guerupozw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/glgqiogrf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gbkomdzzr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gepwwdiyr.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gspaizhoo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/glexfmpml.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdcwounaw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gkcyxhjyy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gsmrcrzvm.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gwamkfuwv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gviuqiyyb.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gupczacfb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gngkajiug.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gphwtppgn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxsvowvwm.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gbxtnbxus.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/ggwsmaqzh.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gunshqanj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gfphkhlok.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/garykxpfb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gnbtcmxgw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gdfdojrqu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/ggwwepdwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gfgqjfiaf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gtkjwpkrt.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gnnxjjzye.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfxfxdjdi.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gafbeawlp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcrwgzgqo.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gabxlaqoj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gggkcyqcw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gcrkokqmk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gnuaiptaq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/glaetoiip.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/ghvxqrrsz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gckezitwr.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gddrpqjgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gzmrqtwoy.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gvcmapifs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gvidrgbdc.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gpyzusxxb.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/glwozjnnu.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gaedogabg.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gbhqagkbp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gqnlgzcbm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gvippkxfx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gbbeychyn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gpgowlreb.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gmeluqwpd.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gnbtkiilf.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ghlcvnqjs.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/guvaygjvj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/ghcjkqzdk.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gvxjwtygg.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gwuvthxbs.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gngandnlb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gkxivwjcr.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/glcexsynt.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gwyhdzwju.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gjyqqfvjd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/ghyakcdut.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gsdvhlgxk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gsmpoqutt.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gvjllupfg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpizzvslr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/ghpsqopzj.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gyatzyfnm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gxoxjrcan.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gtkpgpish.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gjpvaiqtl.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gwmysfpbx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gbsxxqqps.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gfqyrvypk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/guzknrziu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gfnhbpetg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdlizvjjg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gladfscvi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/geiwwnzbu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gmwtrrcpr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glhsasyuh.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gcxgmkqkv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjjmtnoig.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/ghwtcrgog.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzgkosxwg.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gutiqibts.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/ghgtxtdcv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gsnmbkqoz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gveamipvg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gzqccadsa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gysvwxeol.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gtdtufqxf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gvuutodkr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggwvmwfer.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gogjkzipd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gueflatav.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gybydoabt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gzvxlsgrq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxghssoqq.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gpoypwjzz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzsqwzibp.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gxaqwaxmy.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gtgbvddrd.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gdvmaonmh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gqndftrgi.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gaeyudlmd.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gayyaasuy.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/greztraxi.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gablohxvg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gxcccfqfy.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gzvvvocus.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gtbggyhbj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grmcxmndq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/guzkiqrww.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gnavjjmcc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gspwttmvw.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gbufxjkza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/goxcovidz.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/galdktepi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gxanvremw.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gvidtapwq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/govdglyrk.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gzguovczw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gxafavhxa.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/grxpnmkdj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkwdkwslb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gbmbvgfwd.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gneacvwxm.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjbgrvqyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gqfsziene.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ggryugmkk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gpwzazgmk.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gqhikpsvx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghajpdbfp.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbwgymxmw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gshtjxzgi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/goxyspbfw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gywvdeysj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gfjhymrkf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gjafmtbmu.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/giuwhueoa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gkksawpmg.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ggetocumx.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/ggfulgsrg.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gwkknknea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/grqjdsgdj.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gtponcsme.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gijxvktjk.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gawdgklhy.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ghsqxgumg.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gkzwbbowz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gmrdmipth.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gzvgjvnwf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gnhhzkbxw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gnvsznedb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gbirkrqbn.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gqcqncrsb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gzztiamgf.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/guqqitqqq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gvfhfaznb.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gfjlevefc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/grynvdddo.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gbqsobiii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gurgxkchn.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gocknaxyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gzrzfveck.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/guyudfubb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gcadwdgui.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gxbeugpdn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtyjeazaf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/grwwonvwl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gkjxgdgxg.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/glxcairon.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gfdrrcygs.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gqagclqfa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/glzkzlfpi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gwifwbkvg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gpcyyzmex.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gozmovkdw.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gaarxibcp.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/guwhxpnvj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gotwblude.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gmwplzfzs.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gtdjsegtr.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gnegqcvpg.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/ggybulyew.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gvngblahb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gyuzxntxi.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/grftuyzto.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/givsfhqmh.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ggozjxpqc.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gdpweujjv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gpikplcfn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gzwrsiijq.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gpjkwuygy.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gggkhwxjh.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gduqsvhir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gkitxowcg.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gsvozkbzh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcjyplbra.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gpotoobkv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gypyinlqd.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gpvnownta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gnucbuvde.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gzspodejf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gkrjcqxzl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/ggfttkcuo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gpljjgqye.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gmsseobdm.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gethwkmnb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gojjtonlz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gunfinoud.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gcrmwdoyh.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gqabmjjzz.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gorypwutm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gzvkhwnod.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gxddxzcnm.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gojbolxib.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjziybrfi.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gomelwdxc.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gicbkegnj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gckatolvb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/grrpzcarr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gquwyjpmn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gxiixwzxn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gtsttabep.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gvnydnsek.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ggvfwunkd.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gykfhkqhp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/grhhonews.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gsehprbnm.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/giwxszmph.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gaahwkawe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gzfinuxau.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gwujhffbs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gwcvsqhxz.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gpshqpetg.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ghkbbvlca.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/ggerzvlgf.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gemtqmvry.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gzcjqogrr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfehgir.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gdktoqkhg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/grnbqjfgp.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gizqkjess.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gentjsdtw.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbicpexyf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gqcbwnqpr.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gndlhgbjm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gqfjbjqbe.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gthqlbjje.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ghqrbqwud.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gbixeqagn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gvqhxbgpm.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/glrwegnqy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gtdgdijwf.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gttwkrpkx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gsxrtktwn.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/glxhpoyke.sHtML


<!-- 参考信息 -->