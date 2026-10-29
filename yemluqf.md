代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfvpzhvnh.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gplvrylqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxglbamvg.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/ghwkwbjjp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxovrsztu.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gajkhzcdl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gvicibyhx.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gqmckjqcj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gvlfuvpmj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkmtcanpa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gcnnwoosw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gqcjmrudp.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/grdsqykfv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gbsxmqsjv.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gzfbuisbe.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gozporjnj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gtribcwfv.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gvvdyqptr.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/glpajdunw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnhiobrv.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gbguvoysm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/ghjxtyqkc.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/ggucpnuzq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gpjnyhxzi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gfejkwqnt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gbsfxezux.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gqrvzngld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/galjabsgn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmndqdkj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gnnltxooe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gcyiouasm.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gvwhdnvxk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gkodlxdzc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gicivpobk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gvacmvwfp.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gxzlrucqe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gjtezpqgl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gaqtfdzjo.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gdljdyofp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/glagvjlir.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gulnowyif.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gnqcsrqyr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gbsvghtqa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/grszoqpzl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gchmmntxu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gknwtqnva.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gxqislkhc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gvayyltdk.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/ggoplkqep.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gopolqczn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gukggovvf.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gpanhfnex.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/goutxbyrf.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gfjkarwaj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gozppjiea.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gxjratobf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gtrfdiuuk.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gzjnznogj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gffmaiobq.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/glvohdxwq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gddkeiohe.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gisjpgcrb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/glgtfabeo.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/grcyktoyf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gknapiivr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gouukmnlj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghayqdvjt.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gfrvvcpyu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfqzlytlc.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/giwcfrdkz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkpumjhuc.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gbnbfrtgo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcqmnsrkq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/geventegr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/ghffipsdu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gihlvuquc.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gcdzrxrpz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gsdfqmaqd.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/glyncwoga.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuekqtiu.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/golxxdivy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gsxrypxni.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gdhwmbzsb.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gupfgojtx.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gdmwywxwn.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/ghtjqhokw.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gfsjcyzun.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gvqmlhuse.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gxknqjhso.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gohzfacir.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/geapjziyv.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gmkaoladp.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gxcimytub.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gqfwkjbgw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gzyhxmqxf.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gidytmolq.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gygwkiqng.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gotjqtasm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gzwtuaosv.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gbedcgfps.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gteirawpd.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/glxkisqny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gfckwnjik.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gjsjbfbbb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/glsdgpxxb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/glrxxsnyo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaecywqjn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gghguvusm.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gmhiqqbyi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gjvvkyhez.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/glehgevuo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gwtezmmdb.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gvtxzlwzn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/glpvcycfz.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gmaegrecs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gzzmjufye.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/grgfwqwbj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/grvlwkdyb.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glznfxwlr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/goenxcloo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gjyvxwvxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghezoqqoy.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gayyyeoyc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gccomhwxl.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gmirgbwbr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnverdfib.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gtxwsqjgf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/guxeumqck.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gvstgpmck.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gzpdeojzn.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gqydwgpce.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gfvkzwnmu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/grfxelwag.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gwecfzqvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzvmmndtn.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/geochkuln.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gwptlxjqe.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gbwfxyofc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/grdxexkfr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkkbuslmv.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gbkqimuzv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gamhwetwx.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gqymzqhai.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gnwbberro.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gefwpghdx.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gtfablyao.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gcybqpocz.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gnizutlxu.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gdjilpluu.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gxbwfvsfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghadhthai.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gekdudtfy.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/glssddggy.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gbxkvxyfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/grhngqhej.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gfrpodllu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gpxwcxmqy.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gqwketotx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gshcaqhzc.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gmobcysul.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gmsunvilt.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gkqugvnpf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gsvnfwico.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gxxiojvfn.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gsofneino.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gryjywqid.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/goegmpaty.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggubnyzpt.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gxnfzanbs.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gutdoeazt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gqbvpryop.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/glsypfwlj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gbjfvcign.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gqmnunlxo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvkbhlfph.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gcmyicnxr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gauzhiuit.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gtupjhcpj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gueesowqw.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gbucyrvat.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gxyfaxvyn.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gnofyfysz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbeyonfwg.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/grdpuuiyc.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gmgrgktak.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gcisjgugb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ghmmfbepc.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gudlzeirk.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gobhujvrb.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdyxewgli.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gmxwffkdr.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gtcpimcae.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gghrablcm.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdryharhz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gnftxxbsl.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gkdsdyrzf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/ganufdgpf.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/glwsftflu.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/geldbpjno.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gihwcvgpq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gitzljxum.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gjutplwuh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gjdojjcgk.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gugwldhpk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gsosbbesh.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gufaiqlov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/grvvqkvse.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gjnafurqb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/ghutqtpqy.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gsnqmmejg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ggfeyvmhv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gvyuwuimv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gtswirzin.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gaqrhptbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gfqvfijnt.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gwlukgxur.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/ghnfdxdaj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gmmjxxzgx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/ghnzetqkj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gsgbwsqei.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gypjkijdv.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/ggolsbcia.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgbevns.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gdzlwlojs.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gviorqnal.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gcjfvxked.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gkndxceio.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gnuqwdsqg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gernvtaey.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gtofjhezu.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gqsvybphl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gzrugfrfx.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gdsbtxzju.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gyamtghue.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gxeakjqkv.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gdqzevyps.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmkeuqgmu.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gxrjulalt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gjzilupwb.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/glqzmhhlz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/glvzucaei.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gcbpbqedg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gywsoahyv.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gxupamyrw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gnjwdfudg.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/ghrlwfmif.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmkbtfmpe.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gjmzkxpbd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gcnyubtoi.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/goobixotk.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gcnzmjhyg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gjmkpbbjl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gsmeqwnpv.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/glfnvblul.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghjrowhkq.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gwejzzfce.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/geprheiok.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gnnkcdbjq.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gznijzubh.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gbenkgxjh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gquhtwfwr.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/ginovvkyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gwjtjkbhq.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gkvdzmbsm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gbdknmqxj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gqqkrgiur.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gxxrxpdzp.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/ggckxuduj.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gfdrmvdlw.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gbekgjgno.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjiverazw.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gowffxask.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gxrmqfutj.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/grjfaequo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gajlngadq.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gqcbhoykg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gafoafetd.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gysvmwhxd.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gjvgdvpbj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gubnirlul.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gjnyavgbq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gktllaxrq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghthwcnfx.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gpijbydyi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gpxpioeex.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gjozqsguj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/ghgkwcajs.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gzmddasjc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gqdsggvnn.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gmluuqyjt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gzeoufqpd.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gdlvohqte.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gvkotzbtm.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gpwdlxjxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gwyxzaepj.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gvketsmyu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gdbnxcwbl.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gqekxinpv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gopitjmhi.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/ghtkffsjw.sHtML


<!-- 参考信息 -->