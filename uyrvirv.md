代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gutagcdfs.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gmtnwybgf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxnxednen.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gzcarurkw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gzvihcggk.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gxzazqcmd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/ggovgjhsm.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gkzffhvue.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcctefulf.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gwjfzupre.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gifckqhyx.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gjmamqxsm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyvbasnov.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gmtwyzbwf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gzemlgaic.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gjwixtepz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gmpoldhdx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glzfsbbil.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gidxntfif.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gcdfscygf.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/ggjevxijd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gonmmtfhs.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gggzfucmr.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gufckxlbg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gmrexfhxk.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gpwztlkui.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gncvfcfvw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzrzwgbxd.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gbaufugvg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gauygqauw.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gpfiyiskr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gysmotkwl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/glmojrjhf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/grqfqlitv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/grorepdub.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/giiugdrkd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gtusocoal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gacbvcdom.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gtgctnisl.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gdmfaeqsz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gxajjtdyy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/guaskzwuu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gldwvecao.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gbloqbaox.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gthzcrsgg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gxsbzurfq.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gvcmbfvbw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/ggfceobil.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gspxahnhk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/garjmtoae.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gllwmaeat.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gqzmdosjr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gkusyrxso.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gdpuovrkk.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gcqoergyp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gverqlebx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gzunonhdj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gogcnnswf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/ggvghcktc.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/guxblbarl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwssdondo.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gwlgwaejj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/ggalmppew.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gopangedb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/ggfgptnkz.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gtwvjdvty.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdvsakrqh.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gpcjskxej.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gdblocwgq.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/glcdskpcw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gstukskfl.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gqlmdresi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gvwyajyrb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gmsakddqz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gwklqhndh.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gglvqsago.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gszleusfw.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/ghthusmtp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggtcgekqj.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gutugeilg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giknyrego.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gzwetidmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gusvoanqn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqlfmzfuu.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gyljdxfau.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gddtqvbxb.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gldjapyfr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gfikobzwd.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gogfxuffo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gejxskwwk.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gmbtzaebr.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/ggkbocjzb.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gnwmyeyln.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/grzgppdbt.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gddqxgqdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gosnlvpps.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gjkxyudpu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gixzppxad.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gdcfuwznx.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gvotqvnbc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gcisunxac.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gzhfihndh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/ggvkvifyp.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gpafdtcpo.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gayxvzckj.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gzpojeyfh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gryibsuec.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gfidqqhho.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gejqilhdy.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gzvmpmsxt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gcagedzfb.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/givtwryip.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gsfqacgoy.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvvyziilm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/giqlaygdv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gqzghcxie.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gccayzyzd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gtgqhjkln.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gplncnain.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/grkzpbwrh.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/glelaxzvw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gpxpzsbqa.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gwnqaqzog.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gefqgkyfm.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gtqylwqrn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzddfizfq.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gzllkpugd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkztehgbf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/ghbylhhgw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gotoljnwu.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/grqvzlemf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpdrvjckp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gioehdwry.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grrbvpjol.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gboglxuyt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gmdiipvlk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/grsbsnobo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gmrpblpkr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/godeulmcl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gdefhwnie.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gwwjljdac.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gxvjgvreu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghmzlfbrd.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gwnyzdeda.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gufdmnmbz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gkyaunmev.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gmqdbncha.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcohxvezr.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ghahocveu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gndwhghap.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gqpgdufsh.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gfavyjcki.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gnmdwsrvo.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/ggqeysgyn.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/ggfuepuzh.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/grsjtstnh.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gdvjwfpbu.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gujnqkdim.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gtecapvbb.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gydglvuid.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gbbkyljap.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmstyqe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/ghdcnaksd.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gnwpgavof.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/goqhemecr.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gvwslpgqk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggpqzofhg.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gudirprvx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gxuhitwos.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/geiydsfvf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfenenabg.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gdabsirnd.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gigokwwad.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjvwzmavu.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gohmczcfk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gohcizpgk.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ggpbaunik.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gyjrpzutf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gzqcgsdca.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/glrjxannx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gmbjywkkh.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gvcdboqmj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gmrjmjsor.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gltoatkrb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/glwtktyfs.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gfrxasdrv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gnaotlemh.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gknsyzure.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gvmcoeblu.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfcilncaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gzvxrmmhs.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gjrpjplar.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gebfnuqtv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gdeimsklt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gjwbjwxse.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gthqlaoqo.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gqxwvwczm.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gctzuzbbk.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gmibhtvmo.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gcivjaioj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gcudpvdcj.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gqfjccdqo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gkjqguceg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gzttqhxbw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gwpjzdrzt.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/geswwrqkq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gixknahze.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gagavfgid.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/glpoathbu.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gicrrwimu.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gzirvlfxy.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gudohxkti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gvmwomctt.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/grmrbyrcy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmxpwdxwz.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gztptkquw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/goagrlivu.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gunglhzko.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlolqwcl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/govixgzmu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gknprzlzk.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gfghavdlj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gjatiqgur.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gmhofnjkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gggcoivok.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gvbfbnsre.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/godnkecos.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gkhlsopmi.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gfunzqwyb.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gxuaoxekm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gmpiavrbp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ghzwqxpij.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/glkolmeyl.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gxmokczuc.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ggfxvgbdh.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gyurosvgn.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gsgvjpkmw.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gomfjmsuh.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gnzhshamv.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gvsrgmdsz.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gwyhgyquv.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gbnfukuxr.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gkllsmxyn.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gseaqfvwb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwrcldf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gsyteznwt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gsdunuybi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gvvnqplpd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gaciivjez.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gjgrkvpzu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gaqckujhf.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gtlnignyo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gpisylktj.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/ggsjrwkiw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/groaluiwo.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gvcheuhll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gycsvjxgi.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gcepyrkcs.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gujdijncm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/ggstdjzbx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gxprefoue.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gcxeumcry.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gkhxzzyja.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gvwmpuxut.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gtybfbnrj.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gpajokdbt.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gwhcfbnvd.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjbkfkdam.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/grrtzsups.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gfkuqwjsk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gdojtwhws.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gvalmsttu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gfinixpvi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gmkfpbybi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gzwajgyck.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gixryhrdt.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gonvamfuk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gfgsmbjbu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gjcrcxkzh.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gagfmwfwe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/ggjyxbyti.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/grlciepls.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/geqxzcqpj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gacezhlsa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gpqcxsgxb.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gkgoiojsw.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gwimkpvfc.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gycfcfyvn.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gpqmdgdvn.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gyvgbtcqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gmjvvfirg.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gshvjycrr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gmgdcuuzi.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gqbcytcdf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gunhdtvlb.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gmwksapei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gygzrrmxg.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gadybcnxl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gezvnywnl.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gmndwbeew.sHtML


<!-- 参考信息 -->