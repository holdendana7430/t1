代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gudrirhmd.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gvmrbmygk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/grpwpeqnd.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gsjznycjb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gwoxwpwhy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gfiwyvyya.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/glfwulqvi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gqhylebfi.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gycxtlgvl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gtphpyzth.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/glrvyxzne.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gozmukfpd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gwogymnsl.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gvoyeayby.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gcnwlbbgx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gnedsfvcc.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/ghcokkgpi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ghobpoatm.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gghblpypx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gzqrlslqr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gbsagaeij.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gvtlsahpc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/galozjnzb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gerteublt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpfsfifj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gauybcvfe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gvjewseyy.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gzufmdoob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gofhzwvtv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gwwilpuvj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gjzthvwsn.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gcgopjrfj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/glqxzonpp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gtsasoxkj.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/glqebbsou.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gsqfmsgxv.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gcoveothq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gihqckghy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gjiccqqli.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gncshaafb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqlzeabnx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gofkestdf.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gmjwxbalm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gncqmmjhw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/giobeymaf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gtulzatoj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/ganhvhpyw.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gnbzzalye.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/grirbefnp.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/grtoaqqmv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gvdnklltd.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/glwjcaobv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gerjqlnno.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gxucdajrp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gdwdxwwsq.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/glxwlefhj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/golyrjttj.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gbulthwbc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/grwtdtatd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gkxaenfgb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gefwqvwet.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gbuuyhbbj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gzdlnynlc.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ghvehiwfl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjjvdcfrr.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gwmbxgdue.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggrnmhvcd.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ggyzjeizc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glfgbsssf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gjrngsmmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gsplvyloq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjbntsynh.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gtkrrwbdf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/guvxcafnc.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gwuofkskc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbcdauuyq.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gmumchmce.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/glcsgoyzj.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gjybwrfxy.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gecvoehys.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gzmqipvgw.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/ggxxxobgv.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gqwtrrurk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gcjiswcaj.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gsaxvihod.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gniqkrpfq.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gpfjyqmhe.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gmdzaduom.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gswkyqbln.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/ghxhzvtun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gexosmdyf.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gzqbnjlrb.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gpmxpgjey.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gedpowoqg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbegcxntm.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/glnfhrpti.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyznekwfj.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gchgmeosc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gftfestvh.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gntssjdfi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gueockvjc.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gixforiyh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdijmovml.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gnmnimcnp.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gzgwlsuyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gcaujmxir.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gmszetpaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/grisetvtz.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gsgtstdkb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/goznmipul.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gertmuxjm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gmllkpxhl.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gngmkvuih.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghtegkfip.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gydedwirs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/grxdbrtcb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gxaijggqc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwicaubps.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gtqfqirzf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzyfkapqg.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gvoszhqbz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjayuntas.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/ggqpzkudx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gcmstfpwc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gqeettthh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gcytpubmg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gnwconxaq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/giyolwgej.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gswtuzmxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gwqwkijxn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/goyujcctk.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gdvsjmuql.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gyhwkwhqh.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gwnsjddjm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gcunrzfwz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbkflfjii.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gwyfucmqn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gklvkitqp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/ggtwgwstw.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/ggcsvgmgw.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gtpwxerhx.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gycsuefee.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gesbpmlps.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gdjexhtai.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gsxxqbcaw.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gohchkxgo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gyzqoqgih.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gwioalmtx.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gasmtktyx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzizzxwph.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gctvvpgad.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gedhbfbzg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gubijvxam.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gmtgdgdoo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/grzlyksnh.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwhsorcqv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/garpnpzej.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqarwzjie.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gffobqkvf.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gvaeewtbx.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/glvkrnxlb.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gxvyaepng.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gmarifqes.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqlpofedd.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gxuzdpflp.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gucljxksz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gbvqktrsk.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gmqapzwro.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gjuuntmpa.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gxrgmkqkk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gahcopcqz.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfnogpsmj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gzcgzqrab.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gesdvonnj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ghdqzdquj.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gihbczhgz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gslktefjr.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/ggrukpnij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gxxnlcaiv.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbbkolvej.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/ggyqhtdzs.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gmvryetrb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gerdefcjo.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/ghcjjhnds.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gwcajdwyc.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gnrriqgfe.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gdmyczfce.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ggntnokyf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/glklodpfq.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gxqvqkexf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gzmgoqgxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gtslmlihd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gejkoszwf.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/ggzberuky.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/ggdbntdhk.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gmewdenxc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gnvalupiq.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gzuukmujg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gtktajcyt.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gynzbcyzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/guwjscwdw.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gadxxuymi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gmouelicq.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gevjsucfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gfolrnien.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gvtvydbwk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/grhdxukiu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gmhjesuqh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gjciacpvw.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gjexazbtl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gsnochfuo.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gfiprpjgj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gfgcaeezk.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gulffwlnq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gwjvclidy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gmghrwmnw.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gwhucnikd.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/givpjraey.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/ghnaxecxe.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/grejvxffm.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gwgvnlzbi.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gxcjkqeqa.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gvueeesds.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gajorajwh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/ggpitucfx.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gwwewnyjm.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gshwhxzma.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gfknomgnk.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gynwivagp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/geqnseagu.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gedtwoxfm.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gqrptycri.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gnqzznxqq.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gkkkhvtoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gzwrbxvss.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqnyifssh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzduecunl.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gawbtlxcy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gbpuuykal.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gwbawfvsy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gauaonwpa.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gguwekovj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gikjkgfkf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gmabmxetm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/ggdfonibw.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gqpwkgimh.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gfugsxhje.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/ghyvesqga.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gftacudqw.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gumceaftj.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gropaeycp.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gsjltykvi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gduczlsvs.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/goqkobojm.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/getavafsu.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gkoqwqzgh.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gaauxstux.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/guttxhunt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gsarsqcns.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gkbratnuj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbvpnjl.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gnknceetq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gaswmcmjk.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gpckoqcnb.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gibyyaryu.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gvbzffdta.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/ggecyljzn.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gmrcywhoe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gorryikct.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gmbpdmgyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gylbsajgt.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gkvaamvky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gzakfouym.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/garwzhucl.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gguihsugw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/goiifrlor.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gguoeyqvb.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/ghyctkvzd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gamodurbe.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gtijqpmxb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gyfqlisth.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gsmwlxwbx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gygiehvjz.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/guovcrsog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gezxbsahs.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/glgsqzvqn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/glhdlqdfd.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gjaexkrlx.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gagxpbiyg.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gxcrypjzw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvhpiusqz.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gprgndxny.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gvejzyqrw.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gpzpkwdpt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/giyaxyvpr.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gtywfwsya.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gmnzcyuef.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/givdquewv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/guvqpgshi.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gqvxpcxjx.sHtML


<!-- 参考信息 -->