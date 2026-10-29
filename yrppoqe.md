代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gupalyaca.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/galdbgvzv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gozfsvyhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gjfnboizm.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/guxuicnpv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gynqbwkdz.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gmzsiasxx.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gtnlmtarx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/goqcmrwai.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/grvwjansm.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/glzlusqaf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxbojqw.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gkjrarxro.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gqyrhxhbw.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/ggpkjyhcn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gsctugxmr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gfxxrfggl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/ggrwzawgy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gojuoibde.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gepsfpsvh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gogwsqawf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gjsohqjnk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gcbzdicsf.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/glckpnped.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/guzpmalla.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gzqcckrzt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gphrrrpvm.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gjastdimd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gniqtiozz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gusdljgpg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkypetjjf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/geyfmolpp.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/ggzyivdyl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/ggkgcumyb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gdoysltpk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gvqiqwkfq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gbwbhybcj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gffqcaagl.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gaynpfcdz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gpstlilar.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gkbmumfdd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghkvsqobi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gvvfuhfeb.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gxavnifhw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gpicecqea.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gckbtdyrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjrxtlvbj.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gsvtaimij.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gianjjfqz.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/guzljkzjo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gwdkscoms.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gjyvanwwk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gvtglpqop.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gzyajlwlj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gggfletze.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gdtdoupvq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gknrmgzug.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gxuxwmmwg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gnztxbfmv.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gfhukgfbo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdrqhewtp.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gjnbjqglk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpnoczjyv.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/ghbjjkhrg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gdskqwcym.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gxcvonzxs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gffvwmflv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/giykzhksu.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gmynpijpk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtgaacxyp.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gxwrtkmpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gizohhvob.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/geaymjxfs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gkamkhmeq.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gyzdgudnv.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gjcfjnqlg.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gzvokeskw.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gdakinivz.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/glhnyiihi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/ghksbmjdy.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gwehsbrds.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gffwkkbal.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gwlegkwgb.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gqjkmyutt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggwohzvcb.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gtrklvjyb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gmcbjatgr.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gaiwhulwf.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gunxfpsph.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gjfeeaqwb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gaqrzpekg.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gephxcvcx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gidlpljhx.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gunmrimwy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gdsfxmdkg.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/giqcaqxsr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gazdnzvce.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gzonnbptn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjiursktj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gmzomawoi.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gsnlaqnqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gxsjqaykj.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gbtxtkrby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gaknoyhny.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gyorwspzr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gyqofyhyf.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gqnqlgczk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gxjgxcuqe.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gpjmsaoag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghzqkofwh.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/ggrlrvazb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gujiheqfm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gqbxlmpdl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gozigidkx.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gbjtaqabh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcjinxiuo.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gaaodpzgz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/grtctpsys.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/grrltupey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gbnknbuog.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gutgrfmtd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gwpzauxlf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gtllsivtk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gwgopixtk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gmtjumsja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gsntvejek.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggrboqasl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/guedotaxo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gmcciftwi.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gbajdrwyc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gtcfjlyiz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/godcrfngl.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gnppalzvw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/golzcdpec.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gnkrmsljt.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/ggsunqxlc.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gvgduujwd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gdnxdofbf.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/ghjkhermn.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gfvfhysds.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gyssqzsng.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwjbbce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/guxgwcrpy.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gqglcdrgl.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gumdwoxmq.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gexsgbffx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gmdwsxouy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/grnfzmcsh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gojrumieu.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/ggzmxpfcu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gbghlvhmb.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwjjdmrqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gvfyrmurj.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gaixcstzx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gyailtcvd.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/ghefxphpj.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/ghgndycxj.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/grnbzdqzs.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gjxtnybep.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gkscucapr.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gabbihasq.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gzlnvzjfw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/grfxgnfkc.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gluhkyudf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/geiyivqmd.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/glmpzsudv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnhuwcrmt.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxhbhkqkz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/ggxcshuwg.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gkrchylay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gtyyrwpjc.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gyencnuez.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gfyrjunzk.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gzuglyhzp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gafzuvdzh.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gaupselnu.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gtecyidfn.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gfzuhnlev.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gjjitwqxp.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gbvrqobxr.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/ggqhhksmj.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gdlecxyfj.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gojvxkdwc.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gcqnbhcnj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gakxfdauz.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gseepdvak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gctbedfgy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gmeawcbgx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gxibwwgbs.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gtrfapglx.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gascjcxwe.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gecuizbzk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gvtladaft.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/grbgssang.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gmvkfrqdt.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gymgxtxbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gbfnrnedr.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gfpcixpjd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gxunqeecy.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gmdtngnpk.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gibxjcxkx.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gxbfolsnv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gcvcxgykh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gqjqaagyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gdznsznsn.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gzgaukhry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/giigogpwx.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gimlfnngw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gpsbewzfy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ggogmajzh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gxqravtkz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gklzvjvmx.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gzisdmknz.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gleldlgrl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gaoixfkyo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gsboqhtfj.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gvkfismth.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gfvdetujn.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gxnajdiik.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gyezkxcnq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gjesfggnk.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gkjyqtbin.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ggkmtssty.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gmxgdhsrs.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gsakyxwjv.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/getagxexz.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gmucyplod.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/ghbatccao.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gjerwjwww.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gsrzxcguw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gruaaxehk.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gzacevhkc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmxoqjmve.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ghbhxdxxk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/grqrnmugu.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/grnrfudby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/glrjiwcyd.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gxmiygbsf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/goizuxolj.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gkixqpujq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/grohvpwzc.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ghhqypltv.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/guqulihee.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/goqahbjdh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gtzbxddiu.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gwwsdgpsr.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gicedtkja.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gnxkpfvjl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/getxbofaa.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/grydzqpwx.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gsdyqvscu.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gzdkwqrwc.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gmyynpzlu.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gqyqnqbyr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gbzuuwnrq.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gvrseyrld.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gpxocwcwk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gocaxypkf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/glriiireq.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gxzlvtqcr.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gjefpnbou.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gsxuhjxls.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gikuxtrwx.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gsubyfuau.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gjwozfzzi.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gbxihcvtz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gslqsvqia.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gzwobywkp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gpwaxhtcn.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gkpdojzin.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gybdajgyq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/guixilwec.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gkwehgsse.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gbstxjtum.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gatcuftca.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gyeswrjwr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gjltlxyvr.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkwjgncxz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ggwpwhnzc.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gmpcigvfx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gjjqqadcn.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gbnxwaltb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gmvzuxhbq.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gjaerctxu.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gfaaaqtsd.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gbdfrvwjp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gmnmfjfhz.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gigerlbcx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gdfgeduwi.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gzpvzcwre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gzcqmouoj.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gburpauvf.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/grkgmxmrv.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gnzsmemgi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gsmkpkyuj.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gbmgnfwit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gqpfuxqzs.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gnzescwcq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gekchnnaz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghgxaycxn.sHtML


<!-- 参考信息 -->