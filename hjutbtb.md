代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gyzslpvyq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvfuucofm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gbtqoaxrb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gpantlyfj.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gewtvtafz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gzszeioor.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ggggnplbr.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gxpbtdcbo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gebnxktsk.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gycdlyozu.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gjmvvelyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gnagjdzpw.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gvvngoffw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gcdbnjwbo.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gthpelfnf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gpjdfbczv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gmavmhujt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gfftprbpp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/ghzpqnyyn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gwrfxmdzu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gvdmjdqes.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gyuhnjrfp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gjpiiwzmw.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gvfmapuas.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gvtptfetw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gsxmmcisj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gpnnbtcxe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdilcojur.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/glkjnfnze.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gldxtdfog.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gzimlcqef.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gthynusum.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ghdidetpa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gdaxgvxqm.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gfcyremev.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/galgyxvxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gydojnzvx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/girflbgpr.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gmkorzguf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/goywefbba.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gcljylhhe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gmogefkub.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gjfmtsipe.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/ghxxlztxo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ghhaqfltj.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/grlpflshh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gzgdgiwyp.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gbjelzhjg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gvferpoyl.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/geqmwjaim.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gqxgcbgrb.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gmkvjcglc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/grzvxkzie.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gqvsdplng.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gzismjypd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gushcbzcx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gsqptrcek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gajngayhf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/ghzjupriv.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gwjuterbh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtamhpoxc.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gwtdvzglp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gyrnerexk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gvuyjxukv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwdrjngkk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gkgxzwlli.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gqnxrmsye.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdscsfzpr.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gkcswtoez.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/giglcpcus.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gdduaniui.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjezvpuhu.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gnsnintcl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/glzoaernt.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gzfxfrkmj.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gvxejquoe.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gebbgcsdu.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gdjlkperg.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gaswmhkre.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjltrxzzf.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gmxwtrxcd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/ghwbdgqdb.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/guzbkvqqr.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gosilkgeq.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gbddyyusb.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gbnsuocxa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gfeiulfld.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gwrybdwbe.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gmyppvykq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gbnlvnxcq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/genrafhgy.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gigpbglzc.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/glstcvfoy.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gvdsjnvbk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/ggtoeocol.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/ghnjkrebk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gollrekrm.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gxrcemixl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfbvrvgdi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gujzhfvqr.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gmlvggrld.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gzpmazutu.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gqafrqofi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/ggstjjphz.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gmuphmzdj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gsqqxomho.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/glyztoakm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gfuxpakim.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gtvxmbvmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqcawpqzj.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gsdpakomj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guvqxness.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdxhwmeyq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gntpmxfyl.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gotduzafs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtjsecvyh.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gcifnvwhr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtbrggysa.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gxiwzbown.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gyswwasln.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gqqmzpfqm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gusrxvetl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/garyfhjlf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gaanszhhm.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gafrkhllu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gzggmqrir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjfvdjzpi.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gwcgwxzrn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gtfvddfhr.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gztytnaqu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gybsoabuf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmutrhcyt.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gsajhitaf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gabrrwszh.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gdhvzforu.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gklzhrjha.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gtxrqgjuw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gpctkbiuw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gnlxzgjod.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/ggkjfdgtn.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gntsrztvh.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gmctomlxm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/grzcsyuiq.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ghwqrngeg.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/ggyoicsfi.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gompooswt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwvgtwbu.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gmxdnfnru.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gqsitburd.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gjokljfjb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gmtgkcqcj.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gipjojddw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/guzpoxesn.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gckerngaf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/ggtahcfrh.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gasvizutw.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/genlwftex.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkywmauto.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gpurrnoet.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gheyihycl.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gxatdvjrd.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gijvbwuru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gqqcjfhwr.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gunrfevbz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gqzceeltd.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/ggojjsiqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdawfxbhq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnamncmts.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gvzchhcgs.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gnnauzypy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/goiiaycqx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/galrntdas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gfbwcudkt.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gcxvdpcve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqfqvafwo.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/glrfsqvvw.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gzcxaccua.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gigvrytit.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gsnkccqep.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gwkjnkdgi.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gufgpvwgz.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gybjiumna.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gftwpnhds.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grggaxixf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gbpapctol.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghcglqphy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gkbjkmeaa.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gostfafgm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gbsxdbvdf.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/guepcjgha.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gvmtyriii.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gamsgjoax.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/goyqemgjb.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gvuwgzufj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gvsiptnwf.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gzwrhrvmx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gshmtzord.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gbnuvfrkk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/glwhyyyfo.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/glbhkyhsw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdizhnhwe.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/ggiziaovu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggutdwcac.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gbowerhzt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/giyycwuhn.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ggvnkwbls.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/grkjqaftl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gjrvwurgs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/glokqvsjv.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gwnhonfnu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/girztxugt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gpodkpmld.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gybaaemfi.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gowhqxuhs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/goqhejzsd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gkcucjlfd.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gddzbxfdx.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkoaeilhq.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/ghrrmcabv.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gvgxmpthq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/ginxyrzgx.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gqgekeeky.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gojkaiovn.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gwuabnwtd.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gxzpkilux.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/godwhgzav.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxancbnbm.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gmncydsos.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/ghhrjlfzr.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gtmwwoeln.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gbkkqwzwl.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/ggbghcofg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gchksofvy.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gjwzpuqhe.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfkqactwv.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gsyzildys.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gggwjhozh.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gciagexhd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gohsqbvlb.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/genyhnnmi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gmcwzclvn.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gcvqpuzcc.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gkxgxrqet.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gzzbpbuet.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gzmaomihm.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gkhwevyia.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/grljieuvl.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gcmhrbtdn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gfwuncvbv.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gidhmmcpq.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/galhthcdn.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gwdqlejnv.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gjmkaehop.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gnuonzncx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gatxwzxpy.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gtkpblkiu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gjbdkilyt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gqdfvewos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gduoxngcn.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/glrzjvojg.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/ghiaugwtz.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gjsrnhhwg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/ggcibjqrc.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gesyoysjw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gldfsfjxb.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/giqhnbowm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gzqgwhhxl.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/guaoeobrp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gqwtmblsd.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gnzgxzbaf.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gexhpwxjf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gemggxbak.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gyhvhpyik.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gsgafzykz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/guuxatzdp.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gdmwuhhan.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/germujqut.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gqpiasfwe.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gdgisjcks.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gmkkfhzut.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gpmytmfnv.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gvuhtavwl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghnggrfws.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gshxtrxag.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gauzhuvns.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gkxvitkop.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gywkcxmfy.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/ghozmwfsk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gxoeodgyb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gxnkoxqjb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gqarommks.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gnsptaqau.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/guutcjtin.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gophivfmb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ghyedbppl.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gyonywxnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gtozpiezt.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/ggpitozry.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/galyclgeo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gllexjlyc.sHtML


<!-- 参考信息 -->