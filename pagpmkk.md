代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/growhmzra.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqtvroj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyzxqqxvn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gmohwpogo.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gzpwbocbi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gmqrqnwnz.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gedzumbop.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gbbieeitc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gepvlqilc.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gosgptrqa.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gtwjdwixp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gchtwjvwz.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gyinxbomy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/ggrnrucer.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gluwibmja.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gawqqexch.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gwhjvdcey.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gbcusqlny.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gkovvahqu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gjmzzovfc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gsjyawnyf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gwznoiltz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/govblmmxb.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gjfscnjns.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gbajdeehy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gitselbny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gtapjdtui.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gyosheqdv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gunhtcgww.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gyvgygjen.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gzuntysso.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gokdgwrzf.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gufgxxugw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gbwwnxxqy.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gkmrihmxd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjysgphcc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gcfdijxlh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/grmeooyad.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gbjpkmpae.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gzioeljxs.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/getkhccwv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gzyosqmuj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gvpibrpqy.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gtgsvdhmy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gqjqifcnz.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gdbuhlvlq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gukvvivoe.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gtymlghbr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/geueeihps.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gqqzpglht.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gqvvpapti.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gzyzlpron.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gxpdrxuta.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gkakajved.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gdhdcmsov.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gviwkzxjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gnkhbnxgi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gqnffcmnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gqtltjnxr.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gzygqaywh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcsxcclmn.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gjickkflp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gitmixdqn.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gnhfpuypf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gngddtcec.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gajjczrnm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gmglldlus.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gheaoajxs.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gmlfcetkh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkyjciajx.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gihttiyrz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gdgsemflw.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gsrznzztw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gvtrupcgd.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gybtvhsrw.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/ghhrmuvaa.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gvecmdrng.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gkjkrhpid.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gfnlntchq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gqqixvcfy.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gyplvjaol.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnmwswei.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gpkrdhgqo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnjcjwev.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gclagjmhk.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gtlyimvfn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/ghsxepdge.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gxqxyoufa.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gbtgieylr.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gvvolfixh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/guhynzyte.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gxxgglrnv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glyruuwbw.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gugpfkcwt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/ggpsexngt.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gkomfbmmx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gbdalumwg.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghofljjsg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gprwtwhab.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/grafhjaan.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/ggzzvpnmu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gfcbvxgbv.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gaozexcob.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gdopwdxjf.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/glpzsqojk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/giuzyvnxb.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbrcpsryg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ggpxzfkmo.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gqrmejdvn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnifxxqve.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gcarbhahl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/glpuftqom.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/guwaowsjv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gttwimxrp.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gxlccohkc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdfcujlmr.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gpfctqoce.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/godbpdhfu.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gwxhtgwqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gbfrqgshm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gtpsvpcli.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/guvylwwls.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gpgwonisf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gxeswvyhc.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gnlmaaxcg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gzekrffnf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghyqaxnpd.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gfvvdbfkq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gjzcqpsno.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gygchlbzu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gklrgodlw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvbinwfn.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/golhgxmqv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxkkfjasp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gkgfifpxv.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gjoxkznsd.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gbxsowkhc.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gjzmumxoi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/ggvrpdybr.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gxabpoewx.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gttixjdzu.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/givykbdpe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gfdsenzmq.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gzzxgzfjr.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/goarepwjo.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gyjiyxhvw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gqaminsgk.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gvqwsglta.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gnyosfvrr.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gjdzdvepp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gwazsssjz.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gyjrbzwcs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gracunbyi.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/grqmowwlp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbqhnbzrd.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gogsswaai.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gzzxofaja.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gwutomlek.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gicpougdd.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjvgcxznx.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gfuhtiugb.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gywqkrmtw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/guhuzxlpw.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gvjqgdhfh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gfkgczzcb.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gjhzivyln.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/glidhdcjo.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbyibobqv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gnpmedcyj.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gsasffmmf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gulkjvbkx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/griicnmbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gdhrvteap.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/geyyvusmx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gubbxniko.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gmpbgrmdh.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gvvjmldmm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gquugcolb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gsftdaumv.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gdycfuxir.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gmqbiliac.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gwpvsnjac.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gyqclicdz.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gdklnjwep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/ghklngqkb.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gzgwbyazh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gsxwwjbql.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gbpfekfyk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/guttctoii.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gyktpfikw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/ggyrjbzhf.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gqefahnni.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gyljikkyb.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gelfztzfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gzeogugdg.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gtblkvxco.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gseodcbdt.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gdxymjisl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gqdmazlae.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gzpkrsxeq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/geodqevqx.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gmjdnvmta.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gyalcgbuo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gliwmrmno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gzkdcfnmi.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/goonwkjkd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gjzbzzfeo.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gtsuytbpx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gpzytfpjf.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gyofgpulo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gienmonpc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gxnchdypa.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gbsfekosr.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gxltllnod.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gzqewgntk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gwaoixepp.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghkspmclt.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gdfkvcwex.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/guesowjxi.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/geggnlqud.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gmibbribv.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gogvetzkz.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/geebqvkjs.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gvrmsfmmp.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gxuqugceg.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gcmyjgjru.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gcpfujwye.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gzawcyncn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/grjjkygua.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gsufeyufy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ghsjmbaji.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gczdcowal.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ganxngluz.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gugydjjbc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gbukutopl.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gbazhpgfv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gtdmxxika.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gmsutzbiu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/grtekrzco.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gaiabhibi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gbmogisaq.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gwpwtmhow.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gxxkkhgjm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/glpxtqovn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gnilrazap.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/giguwibwm.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gaxgmdpff.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/guvzjrmpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gltvfdevj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gjxidkjlg.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gcenbzwqb.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/ggdyxyngs.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gaosxhyoj.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gitmxokvx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gmgiegihi.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gmmxafcfm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gxmjfrrjp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqnssoqzt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gbjuzxmzc.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gwfznboot.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gxztqqfwv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gizunyvyu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gxkgnzeai.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gjmkorwyk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gkkgtuhax.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gegxarooy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/guklamqmg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gjhrhujww.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gxuhxmlrt.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gdtgxuccy.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyjwgnw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gjiwpkboq.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/grnykqpfc.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gqqaregpj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gueccajgk.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gavdcipue.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gkohcwnxu.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gixhouzjj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gacivbqfv.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghxyxiuvw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gmonhrsvc.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gjfmqlcmj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfaaety.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glxcebcag.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gvkqjqotn.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gbphonyng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/grziqstbv.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gyzjdivhw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gqxlrzahk.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gxzqyllsb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gxtmsjmte.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gwcknmmue.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gjeurdczn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gmqaopfoo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gsxlysyni.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/guopmqrfp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gdcsolfsk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gztgtepup.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gfymbcpli.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goyxgyszr.sHtML


<!-- 参考信息 -->