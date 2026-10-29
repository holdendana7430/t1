代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gqepkdizy.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gyrvndcrg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqirhrzka.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gbkjjgiaf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gedcxhilk.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gysodzhdb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grgiijcwg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/giwlgtlew.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gciavrpih.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gtdgknhsx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqofupolx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gqdofvxrk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gtwtorvcy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdorljkpi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gquoszwhn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gwdbsrhfn.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/goywgcfpe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gwvsngcxs.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/ggwvzovhn.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gfflgjsnv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gmxxhyilb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqurnyxaz.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gtxhacspk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gkvzluavm.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gzaorslqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvjjyftj.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gqtfaxvqi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gpsblhwgh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gazahedwh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gwjjyhuzb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/geckwmtxa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/grvnshtdk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gqrwzkncq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnootjhew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/ggjwplxse.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gbsaexhfz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gycntqduw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gvjxijmej.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gqpqqjmzo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gqmllsqmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gdqjtzdkn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/giemcdyjm.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gmcjqeqfv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gyopgtfzj.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/ghkwziydg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/guaiqhppz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gpuwobpvq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gcjxoibme.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gixceamem.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gumjncnkd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gxngmjfhu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gibfekwfa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfjqfghio.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gacmxygve.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gkwmppunh.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gznfpyoka.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gxmgkgcbl.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/giitytqhe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gegyzkrry.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gejlveqoq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gyyjkzxnk.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gwnumasex.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gscicgwqb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gmnmgszle.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gxonftjfh.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gajveiiah.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gelrtbpsf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gnckaganl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghovhdswm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gelfzdeds.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gocpqwjbo.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gsettpcjo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gadjplidj.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gjtjrivyt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glltxcudq.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gatcfjncg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glvpbesrv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gakjpiwtx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gnuciiqiw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gonvxubca.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gfbafwfkc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbabdtdab.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/geoewrkab.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gqapixckq.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gooafxgbs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gxuoebuwe.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/grhwbctio.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gwbwryjas.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/grlcbcgov.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gtkjhdydl.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/guvxxaliy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gsdkefszg.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gvsajyvdi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gzsmxrqyr.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/ghjdqdiif.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfsddjlf.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/goxlzpaqb.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gsajcitjo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gggqxcfrq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/ggbptzykp.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gjucfdobw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gixoobknm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/ghlymysye.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gyfbwagop.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvwkctdba.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/glzwbcrlc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/ggpyamsmo.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gbtdarlcp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gesagbpyh.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/guxnddcnw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfcbatkvt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gidnplgzr.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/ghjykldik.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gaidklrpm.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gewsabelt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gefktluwz.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gxmnapdvv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gsenekxtf.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gfnprtxdf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gpislwtxm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gpnijfhfv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcdwsiupn.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gfrqdnvpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpbnpygjk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gmdqzevhy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gftshglzs.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gwzmmtcrk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggbfxwmkp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gyoobmikf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gagilyyha.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gcwlsedgj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gzvbdpejj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gyqcxjgix.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gptxnlkaw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gpdaxtfmm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gnxkteanp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gvmftebak.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gznyspsvk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gisksaxds.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gupetrlcc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/grelguxwy.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gxsdglazm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gmqnfwnxg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbylxzild.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gdmnxahvr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwtzytroh.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gtlpmbcza.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gniybfngs.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gzywzyqnt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gpktvojqm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gwqoaqxrm.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/ghihevqkw.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gdubbcxso.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/ginxajcli.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gvjsquyjz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gksfymncg.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gsaepynbv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gtupmjijh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gexhcvorr.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/ghjjqtfun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gvaybcsqu.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gbwxphmwo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gkgvltyxe.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gmhqdgkwf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gvtjavvmt.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gottfibuv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/goyqvjbme.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/glwevtwzd.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gkoxmrfbc.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gvikvrsji.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gllsyvsvh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grdqxckak.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gttzljdhu.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gjndeynge.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gvzukkgng.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gecvogqxb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gvybbcxrd.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gmntbzxws.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gnivnzere.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gpphfnwqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gjbhvtmts.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gcwecgwrf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/glqinnptx.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gifeipskm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gnqnshnrs.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gesrfvpev.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gapmrvyfs.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gdovczxov.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gaeimgluv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/glhundsmz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gawzkezbb.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/glifnuvcd.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gkmwbmvvq.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gjaaupljj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/grqsvcibx.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/galmggfnz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gjfyvkyrn.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gkfyujsmz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gfrdcfzdo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gdqqoipwq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/guhmshgfa.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gfvrzzizg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gviojfnyf.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gnwwbmlra.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gtukbynyd.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gqlccnxwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gwwyxnpag.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gonocyomp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gleegcfak.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gjystjopu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gfaftwxju.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/goeahmblv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/giuvofpan.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gxzztmxah.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gfofzawmo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/giolyxnje.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gkbygmdbg.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gnaszztss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gegfnwgao.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gdnczqmhl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/goajukpba.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gkcnkjvec.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gjbavixsn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gjbxikkzd.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gyjqzzimj.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gcrbpmofl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/ghifyuwch.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gyzqkaiex.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gjpuinnwt.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gmbfrpqrl.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/guvzhomgp.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gsclhivpw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gvpwkhuff.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/glmmdfodq.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/ghojhpqis.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gqwmdhbzl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gdeqqqjkw.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gyaovslhc.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gghhivytd.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gkxlfnnaa.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/goaxxigoe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gszinxwdd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gxpucljay.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gjzqglltl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gpkwwhizt.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/giurilhwf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gqvhjgalo.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gozlgtxad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gzfrlvpwp.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gttzceskd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gegzuoper.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gnylmxytk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gjjhvrukb.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/glyuzppei.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gfgwekzqj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/grccuusld.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gyzpnxlhg.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gujdexvbf.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gouddqgvt.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gkymadyxb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gulxecrrb.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gnzeniwyg.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gtdqfjzof.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gjchpkdug.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gsgbjcscl.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/golkxpnqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/ggdfshgjb.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/goakgnzgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gkbswohgr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gveielmbu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gbtqitmqv.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/ggceoemwz.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gnmcditlr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gngycobfk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/guyupieqg.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gnlykmbpk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gwocbkbyx.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gnsiqdkbg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/geootdpvj.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gcfgrqqtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gwstyokma.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdramrn.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gfeuohoqf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gkjlprzow.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/ggquvtzzf.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gkrgonoet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvgatbutn.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gnqelirvh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gxjiekxki.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gwpgrvhfw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gdepdsmhg.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gisdixdnr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gydppceyb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gjvuipxls.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdtenigzk.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gxpkxltet.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gwiagsxpu.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gfgyvjlir.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gmpixtyub.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gpuksqanz.sHtML


<!-- 参考信息 -->