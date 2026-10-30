代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gyfdfxima.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjzinnlug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gzqgnfvxm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gaqlameij.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gxynqgxgz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gymcugixt.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gxarcktgc.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gjjbuqgfq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gwjvszlwc.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/goymkatqe.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gxulamxki.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ghfffbtun.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gqbglnjfg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqarqvzs.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gmxnckgng.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/grxupslgg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gvpnkrhec.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gvwnvbokt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/glmnmmyit.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/grsmvvkiu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghttuawuz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gjxtbddfe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gsqgdsmwl.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gvhmobdaq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gknzrxmvh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gyomgbdfj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gavkkyjpa.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/geqoafetn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gfuuvbdzl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gncsagxij.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gfxqoaaqq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gsxeipvgy.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gidghbtkj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gwqrjzwsn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/ggcihlrwx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gzyevgmxz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gpkggynpp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gnyyxwjtf.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gmbcuxoyj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/giroosizw.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gbpyjnvxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/ghcfxxerx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gqezqohvl.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gqzcxpmix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gtzvvohbb.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/grouvhezx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gseshrzww.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gdpoxqkhy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/glwkkqdqo.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gzidbgjoy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghqusohoy.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gdicnuoxe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/ghyfvsvzf.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gzfsihaky.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/ganvxkwoa.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gflpbapjr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gftteaogu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gdvimctxf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gfeigqxll.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/ggxithnse.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaqpraszf.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gofryngja.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gfelwjprr.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gnxfhesao.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcvfhancx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gryhnymla.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/ggtimvkpr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjgxwfqjd.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/goqpormek.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqkxqzjrx.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/ggtntypmw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gveplhrqr.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gnkaaxrjf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gdtgxcrvm.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gwrxmttwt.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gbezpqija.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gjhujqvrg.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gxepwxatk.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gzshjfmvx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtcddhsse.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gftdohpvj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/grylmacca.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gulwtndxd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjciicmqa.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gvcimusei.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gcyqmqtth.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/giwaheidm.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gisqcbvif.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gdvqfmzml.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gkkptyamp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gnipkepak.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gxpqwhdqs.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/ghbzvfvrk.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gepeeybsb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gwjygulkl.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gofryghri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gnfqdtzjj.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gmjgjfeui.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giksopcie.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/godydcvrr.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gxmzkirod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gzfzghtbf.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gxxxopzbt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gkaqiwvto.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gesmbookr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/geaxikvfv.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkdwynpia.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gumlvexzx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gwvorkrrh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyzjrdahk.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gpmyglsce.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/glizlpsoy.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gtqipvveq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkmmxuszv.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gvcapijdt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsxykklfs.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gacpoqiev.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gismpnbwv.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gcmexzgaa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gthijumys.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/ghfefodqd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gmgvwnihf.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gskpmmbyn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gbackndax.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gszqxjrtq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gthbxklct.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggvjqkzvt.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmdyingkz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfenqsmbq.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gftbbyutw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gztuczlii.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpbnqlfxt.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/grjgphesr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggrscznds.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gxwbasxav.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gmlgouhxe.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gypjcmqqo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/geioimfyc.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gbxafigsz.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/grunjvfig.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gcxifwetq.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gsnvbofak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gfynckjkb.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gewcwdomv.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gzllhvalu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gtcnxljjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/ghnmyshgz.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/grwkwexet.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gegiopqkl.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gemuwgxxe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gelgteavr.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gmpxnwyos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/ghrktlvot.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/grehwwusl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gsqmyptel.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gtfmafrth.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gooljgknv.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gpfnkkztk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gqzsqqqtw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/govtajuku.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gxwbeinms.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gllgrkdbn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/glhidbcah.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gjsbiqlph.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcpaisvtj.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/glljyumrd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gjyettqfv.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gllsejrjp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gnnppqnmr.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gxwljimnk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gaxoxjeyu.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gkdjrcsws.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gzhffpeqo.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/guxjqvvsf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gnxtzrpgs.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ggtcvonnu.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gcyndtddg.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gbcjdmwou.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbecvtvid.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gldcbsmad.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gmhjphwqw.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/govdrutmi.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gruvdcrug.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gaknmeqem.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gxairyuws.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/grtzrjjpq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/ggpjanrfe.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gqqedhdjn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/grzuukbnk.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gmobmywgr.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gvgnzlute.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gqcqtjgmp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggbwiwmsl.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gpsrbqcny.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/giyzggjqf.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gevbyxwns.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/grflhqtdg.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gmjbatdqf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gwtbjpugy.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gmrfmlkoq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gnajkuisa.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gncwlhbis.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/geaafdrkb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gcvinmdce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gstairjbp.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gswljjtre.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/grjshongt.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gchaodamc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfmzwxb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtomxcm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gvytqgjxg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/grnfmhvmk.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gqwytqjai.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gjvmfmpbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gdtmoisgy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gthfyoqwq.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gxxclndeo.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gptnyxdrx.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/geuvalzbr.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gvnmiijnb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/glsaiirgh.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gbthlxcsg.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsndnekgx.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gxyieuxjc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gptjqhnvw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhgxhbz.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gqpfayrtv.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gxvcrpkye.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gtaxqevyi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gvbzifqlm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gznnwqpoi.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/ghlxxlsny.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggyfewgwd.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gkpeagiyz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcmisgt.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gyabwtmlo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gkgswgfqo.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gnsbtvvkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghbmbmwko.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqgmsqabc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gowuafnwb.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gtfvlpkcr.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gjmcbdxkx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ghamxlzxk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ghwvmocur.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gifcmyzud.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gitvfulgu.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/grilxhzdi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/grpbzslck.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gtoyjfzgz.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gneurqwor.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gpbcakgmg.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/ghauixqga.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gdntqsvnu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gdjumgcnb.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/guqbszuvr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gmafgrxwz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gaocflcca.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gaunafofw.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gxlttrofq.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gmefefnst.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gmpjjaftn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwdgbwbjo.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gmrftzujb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gwdmqwscw.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gzkuzbdtp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gogzbyzmj.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gainvoqpt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gvwmuugxi.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/guaunbopv.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gjqyrrcqb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gyqxprgbu.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/goikubuhr.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gbqqqwwza.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/ghalpzwlc.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gkqoovdcn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gggmhhkgw.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gnkeawcoo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/goakhaosc.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gpfdhtvgq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gyxxikwbw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gplbdwcdh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gbpdqnhcl.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gnrlvbfat.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gwjyqffzj.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gmuntkaji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gcqmvctuq.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gfrgkkypn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gufikyivu.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/godozugix.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gxraumxmo.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ghxzxkgwb.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gabtmvtcf.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gudihfigb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/ghnptprwy.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gfeopjiqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/glxtdotda.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gjxzwptog.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gumojlfpo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjfbupizc.sHtML


<!-- 参考信息 -->