代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gjvqzytyr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmtuenzig.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gmobtpzta.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gdmlimlsh.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gviubycux.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsnvfpc.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gwzcgctub.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gjdoerrjw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gyxvpsgox.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gxqiyjicd.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gidfuqztk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grwonehkg.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gmgzvkfoo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gtmjbhejv.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/ghzhsukdi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/grnymnzvy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gquufglgo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gkwzkphdp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gdxzhqhmf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/geuucpifj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gkkqkxmps.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gqnjmbcem.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gibcfvcul.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gmetvrsul.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/glgzechlc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/guhegailo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gqodcxipk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gccoabjcl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/grmsyhhkx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/ggxlztuds.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvjngsrfp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gpzwlkmue.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gvqsdmmqw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gmatplgfv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/ggldxkhwt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gyjdduccp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjgggshzm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gwfohdbas.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gxkejnuzb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gwwhlfxyk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtxaqbrna.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gpbnfugxo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/giojrykdg.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gxowbwctj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gpridyfdd.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gyqjbftje.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnyfzfjbn.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gpcmvxrgr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gjvlzmfso.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gwdoicysb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gceawxckq.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gutiqqmet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gvdprfqrz.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gnkcofasm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gkxknjezz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gtndhfqlm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gzgkftfpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gpueuktfj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/geihgzzxe.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/giefmxhmj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggcbvxthu.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gpdogemnx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gakigiaqq.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gthgpcftw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwajbyxjt.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gosihlxca.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gtakaiszp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwiieqr.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/grmtopuoz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmevntnov.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gozzxseoi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpscvgmzm.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gytnuacdh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gzhcovwwh.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gjmgzgzpl.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/glhbmcbcb.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gpmncoala.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gkawlrofv.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gntfzbrje.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gqmigztps.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gfkwubvhw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/ghytvlsjq.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gtfchqwkp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gmlcylidj.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gsojmkpgo.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gghzjmtdb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gaqnebrjb.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gcggmoozo.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/glzwosihq.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gioullxwi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gpvflbszk.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gqyshjnzu.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gozfsigov.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gdckxbahn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/ghigxbmqn.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/guogbypxi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/grhosktfs.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/goycgzyjt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtkjtiltr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gtdiikagp.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gegalbfmu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gzjfrqkbe.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gjafqbogf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/ghzapdhnz.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gyvvmizmb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/ghgyfbnfg.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ghnpavojv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/grragkidt.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gewkxeydc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gipbsnwwn.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gnwtbaemj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gzixycxzz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gmlazwwvd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxjnbuugm.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gpwmisrdd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzrtwmbtw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gpfltifqe.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkowbgfdy.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gxdjtwpok.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gmndzcxgq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gcohyicxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gdksiruky.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gelidckhw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gdhgyztey.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gqkgobacg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gnhguluqn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpqyclyot.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gmaehpdtb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/ghgsllyyx.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/grdgqlaax.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/geiafvkhg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glpxhejgs.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gzvujyicw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grpzovyoj.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/guhwjyfvv.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gjnkjkskf.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/grreolgub.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/grntxdtgs.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gaaqydxls.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/geyhqjaby.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gwuipetqx.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gjuncrqmz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gippiqajv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gayhmcesn.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gpaypclmi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gouohqcte.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gdieeiffb.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gahrxcnwi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/ggzxeineb.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/govvbmblv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gkwpoyxwt.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gduajmsro.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gcorpwrbu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gjwvmzssw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwbnptbdd.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/guackhdry.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gygjvvrip.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gnaoutvth.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gojhfvfnl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/ghbotoqgz.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gbxdodlbg.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gfbbxwrmm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/griezikzl.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gsdiheenc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkgsmpsxb.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gxyljtmhm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gzxtlgxnv.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghdctwqmu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gqnbmwtwq.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gsepcgvlo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gbwqpjmho.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gjtqprikz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gnigxmjbz.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gcksxjpdg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/glyukhbcz.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gjyosptax.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkwtcvhid.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/ghhqxnomo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gljgpfxwp.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gnewtbskq.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/glozkywoh.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gawcwqmev.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/ghluenago.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gnlcanplm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/grjrjotru.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gpvpqvugy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gyfqlmuwl.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gpzmibmlr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gasyvrcvz.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gadmgeuuf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gabtqitim.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gekvetijy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gjicjojjx.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/glyeajyyd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gouknklfp.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gkixdrtnb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/godojtlye.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gwiblwhqa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gbvobxgtw.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/glbppwjcu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gwtdccppu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gjktydasi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gcumpsugy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gjxgoabtf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gwmauzpvp.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gksiiutzu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gcbufjdnl.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gwqghcatm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gdzmrtced.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gsvuwcdlc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gtihepfse.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gpkqaftzg.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gmnyuuiii.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gemkkprri.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gsheehbwt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gfogljsps.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gmnriaeup.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gpnodxatn.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gtbeahrpc.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gcjnvtpjg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/goswkrtmv.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/ghzavnpjn.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gareomjky.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gffbbtvex.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gujnyrxhm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gordorlrd.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gpqwfqosa.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/goyduhxyf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/grfuehmvf.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gdvqynxul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gecjvjrvo.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gmvpvkibn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/glaghmbgw.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/givlnihzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gaixwnabw.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gyiyrhlzw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gieweuesc.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gongdxprj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/godvqihdc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gflbqadjc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gxcmusnkv.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/ghdjvcaxf.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gawcbydic.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gddeajiig.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gjrxmfkej.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gebgsdxzg.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gnthnwjof.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gyrrzcktg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ghoekbpkq.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gvvxmkckr.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/goorvkhfa.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gywhpydwr.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gxvcnaczj.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gpunvpdgs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gaskibzio.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gclnphjte.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/griqcxhel.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gvmabzokk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gowodbong.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gfoqstdlr.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/giplonkvg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gfyipspcy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/guvtjrvxa.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gvnumbwkn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gkgrldmij.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/ghzwmgkkk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gozlcmzzk.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gywfxjtyb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/glgxqskja.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkqglsn.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gpptctxsx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gesitfvxa.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gxoqtfnan.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gfsfothds.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gfndsthqm.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gmddthpaq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gwkiunook.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/ggcpanzut.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gziqeusbc.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gagpigbpb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gwdzmvcem.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gjlzkrves.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gkevakfht.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gejvsemnq.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gcabqyetm.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gymlyxglk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gpxtzvgwx.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gtpgcnwnc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gjvhwwpxm.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gvrnyejrr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gvorcnjay.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gdsejmazo.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gildebjap.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gyhvtpsye.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gqtocegja.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gyjhzgkwp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gspzoejnq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gytxxzfsy.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gyqwjyzhm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfyrrlgka.sHtML


<!-- 参考信息 -->