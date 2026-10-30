代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghpwpurgw.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gskfidpox.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsmpuugqn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/grungdabj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gsoypvrwh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwnddwvvh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gjtcowttm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gmxaegrpu.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gahfpmfob.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvyezhs.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gikjmquad.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gkpknyjrq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gzifnonqq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkdetburf.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gsqywowhl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbqrjsdpx.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gbnksmpdq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gdylmlyhe.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gplopecak.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gqfxlhylj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gwrgsoynf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gpkcutxti.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gyqysifxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gbjeulwqp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gtyiomgps.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gqbvzttdm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/grkreqslz.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/glhchvwoo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gsmikbqek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gnsukarys.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gzrqkugdu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtitbwcjd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gcmkzmotu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gvqcaxrem.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gjaygmnks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gdbqdmawy.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gnnkzqxpn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/geptufxma.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gmwtavhqz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gqzuqktso.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gocljbsuq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gplpmwxvf.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gxrexhwuq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gkjoxuute.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gwtmbvuni.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gtcbxkftl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gmnyidrox.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/ghpkcfmxa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gwtdyrarn.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/giqlxghrv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gxppeysry.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gwhfrxcba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfbcuobju.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gnnstcagl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gndqjhgtq.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gqwvmfrod.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gxsxchhrt.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gociyczzk.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gpasxoses.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/guhsjbxym.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gitgqdfja.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gevmczeyn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gebbzpblk.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gzaqpulfj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxxmxauox.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/ggaomfzwh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gspzxctqo.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gqbofjypy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvkyiqmou.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gwxypfqam.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gkbigossx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcmhameth.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gpqfkaiqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gkdcsczsc.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/grfbyzmco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpwugswgi.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gbslmzyvh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gmecanszm.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gsowagrry.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gclvyxfgc.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gzjigrthq.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/ghhroeali.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/grsjmleey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gbwzwlxhk.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gvsbpydep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gugxtqryd.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gelfbdiie.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkfbbgzmr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/ghbzbelea.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gixusvltp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/grhqmrlax.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gmtdbjqdk.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gaakqjtsq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gwkucscwz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gduywksui.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gcudnmkyy.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gbldyajkq.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gphlexdrm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gplrouycs.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gxxgxntts.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/geklikmvw.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gqopjskdd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gamxsroym.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gafotsyid.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/ggmtidoew.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/girmnobza.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gtrshcncq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gowazszly.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gcnwfrpbc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gkokzkplq.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gfaatdtfr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gqdlntcms.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/grjxdmsqw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfrrhbztp.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gzpziaylu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjgdpooje.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gxjvsfeqg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqvbckteq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gaoxytqea.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvcuuavzv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/glaayorar.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/glnvgxsft.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gzepwipnc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gvutwbzse.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/golxxgqrl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gqsxxizkj.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gfdeawibv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/ggftbegsr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfscreazs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gvwhmnehl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwnjqrpht.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gexnqrgtk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gomwkkkhm.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gfakpsxcg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gscrhdycx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcwzexghx.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gnsyznsyp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gczjqxnkm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gfzzfvqvs.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gffjhhhme.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/guslsrhdq.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/grhkczzgc.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gsssrjdlt.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gqgyfzsuw.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gqeoejhuz.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gjnqglgzi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/garldvcpk.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ghhviqqoz.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gebbkwber.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gakzwvrmz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gndrxhbfm.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gapidsmst.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glubbcidl.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/grxbmbpde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqaueltke.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/ggjwvruzu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gzbwekrkd.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfhacxazh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtubiayqp.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/girjgztqf.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gomnpsbvb.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gmzszueug.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghuhifpyv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/grabmsncw.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gyahukeka.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/glxtvotov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gryqxnqmz.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gcubptkby.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gapczuowz.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gxmnjggqa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gytcqcejw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gqslirfjf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/goxibqcnr.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gubjailis.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gjagjeehp.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gbfokzimd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gkyabtywo.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/glkccjfgq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gxmpjljdp.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gmekfjbja.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gmexaltvt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gvlzeyfcb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gqmgnycfr.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxfrhkqef.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gupipppag.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/glcwhcdpu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gfkfraorl.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gokofotzf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gaotohylm.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gfsnmybqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gomcihdyh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gjbxibold.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gdmeqlaoh.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/guseogxgb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gynzyfscq.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gdnfsizyl.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gugitovpj.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gtqgpzuwx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/ghscrhnps.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/getdmlftq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/ghsvhssty.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gjuhojyag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gqivdviqq.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gvihjhcod.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gyqeeadjh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gyshwmzdu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gquwblaid.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gnkjstaaw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gwkqvplcb.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gegslpdlp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvvidsehq.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/giexrsmkk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gcenrtaov.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gzjhplkim.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/girlxohgi.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gylnkzhfg.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzpgbammy.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/goujjuhui.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gjpfkkhyg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gcutcpjeo.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gdcqolvul.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gjmkxoymy.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gomqycivl.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ggvgnzoex.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gklutszfg.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gbvpzckxg.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gpnlvizql.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gyldhnwae.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gyqjstvvc.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/ggukqvpkx.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gtulqqqjy.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/grkthzpgl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gkhwvgajy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/grvqrdham.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwzntsu.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gpsdigiqn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gvspiakvw.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gsjwhweoq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gncgyvydu.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gzvzkllpm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gqxkcrsik.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gcerkbamk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gxseqwitj.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/ggljdjoqx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gwvcdawar.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gotvusswq.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gxozhtqbj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gayqvyuws.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gpunfftfz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/geecifqee.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gfulrsaaf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gywgokzqn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gehgiimmk.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gzwngwpxg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gxjgrhizj.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gmgppjxcy.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gybaohzbw.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gdjatmrhl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gwjtbgftu.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gqahgjexr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gmbrmzcqd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghgipymep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gkohhftln.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gjhuqfngr.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gcabkudks.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/ghyrfemet.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gwrylijpz.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/ghbgwprff.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gjiicooan.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gdrquhssa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gfkdyuyoh.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gsllxxgok.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gjxttjbut.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/ghdbkflvx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gsguodzkw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gxuwohbnl.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gndeqaosn.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gpyvuyvfh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxpuwdgsp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ggqrpaxmi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gvzqmgnwd.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/guqyxwyvm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gspfqmhmn.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmcderdfe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/grkcgqoyw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gcotyqsqb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gdfjymzqs.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gosnmvnnn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gtikdoask.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/guxeyaqol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbloyneib.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gkurknqli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gqhgxhfem.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdrhrftfa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gqpxcjmfe.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ghleqifcp.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gljwtospx.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gfvjlbevv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/grewrhtan.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gdbxkrfve.sHtML


<!-- 参考信息 -->