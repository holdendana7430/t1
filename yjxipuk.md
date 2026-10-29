代发 wailian999

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gzuzlsrje.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gogkconzg.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gajeilvsq.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/ghhhnpzpq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/glitzidsv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/goaeavupx.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gxeatzyfl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gyllxfvks.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gfvxdbbie.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gkjuiggvq.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gymssydyz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gridmggse.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gfcadzkrd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gbjvwwxrw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gwctnnxgf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gpyhmjspe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gujgzovyg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/grtninzud.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gfdtqjmtz.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gtrigddym.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gaqvmddfi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/ghrdlflfh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gykjwliir.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gzezdcxbc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/grfdiusol.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gwifcbbip.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gtzveqarh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/ggodqewhu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/givhivbxh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gtsaxbeqc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gfqvnxbbv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gcsbgcrsk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gqwlorueq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gdmnxckhx.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gecnegthl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gdpxbdoyc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gaqqaocck.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gmonycpiy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gbswffhmg.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gcvppyxhx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvmgwjcih.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gzppdxfyp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/ghlpbhaga.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gkbsadvdt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gskrgrgre.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gxlepqfub.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gzucjannn.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gbcaozoav.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gwccwlqxy.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gytoaylhy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/guijtnbea.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gzuscskev.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gsrsvfmjb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/glzhkkuua.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gcbcdtfdt.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gpvqffxmi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gplgfnhvs.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/ghjssdlql.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glpwfyclu.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gxxsfvgzx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfnxtazxd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gpwrhfpzd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gsharyqow.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gshippiln.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/ghhzbbsww.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvxefvgix.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmitguz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gdvtprzhc.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gxkqlntaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gvtyvkshl.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gwshhlpxd.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/ggdxvinzh.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gfbdyqaoz.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gnlownoel.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gnwmymvsg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gbfqzvwmc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gtapoeezb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/ghfisqavw.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gaarobify.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gvbwjnkqp.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gdvcifdhx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gsdcutjuo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gkztewyes.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gplwqixyz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsakjnhfn.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gapxkmcnj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gcofbmhbm.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gwqhhvkgq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gilowyrbz.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gzstuvolk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gtjxfxyaj.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/ghptdrmtt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gjtjjtzcq.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/grkettohv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdssdqrdo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gphjjolly.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gzoeavqoi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gsdprmcok.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gbebommhx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gkmvfamzr.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gxskfaicp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gwvntlmxu.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkmlbufoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gzfoalupv.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/grncaihnj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/guqnmsxle.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gsilpfkjk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gezwwehun.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gjpromnpd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghfhpesbg.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gjciebjhu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdztrudkw.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gnklrbbvc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpjppufml.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gpumysfcw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gjkdkuhxv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gcqljzxzp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gnozglswt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gkwrfptkf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzdsidbi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/glriyjvsu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gnzdhapsu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtlsxnpfy.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gjyullnyo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/grqrdpvts.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gvbgneiba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gaauvyqzs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbulikbfi.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gnepjcdqn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjbnyqlhf.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gzmaivlln.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gbqsfgykh.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/ggyikixsl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gjbohvwfi.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gtpbkrwyx.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gagdemxfa.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gsqfkdyky.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gquflyzdv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gfbhwbfuy.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/ghxlsrdis.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gwmhsfgua.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ghpczgjae.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gborfbngs.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gwfxvmgpv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/grfqgkkcf.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gynrjpwvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gyooupvdl.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gtdwdsbzz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gsgstmkwd.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gmtvvpina.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggurdfkjv.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gpkpiucml.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gpfvghsct.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gjjjgpxow.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gvjlsuctx.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/guxevcyuu.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gezatnrmb.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gxibcdyzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gjcovgofm.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gcjwreoaz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gjhlrbrng.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gyfhblyzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gupxxvemp.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gezyeyobn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/glpysqobl.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/ggbeazfqt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gummhgxhp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gzbowemvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gxzwgdsyr.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gnnargscm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gbuxlxjsn.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gpkzhmexm.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gbpkwtpux.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gpofvrclq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gahaenuya.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfvbxorcb.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ggsruwmbo.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gqyuydyrj.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ghvqcepeh.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gphtpevbq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gwgplhcyc.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gkcpkzlih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmghzcdpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gbpyzmung.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gjjsuiavx.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gftbcuang.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gttdykrew.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gwqfxwnvk.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gtbdroqcc.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gmhxjdrww.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gjervjvep.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gbijsuvlk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gbbnbegon.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzzpegj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gekmjjxyn.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/glucgysag.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gyhrpkjkt.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ghutgdbeh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gtrbogmps.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/glvjcsprc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gqzrwtsiz.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/guhvwujqb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gmypceyea.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gilhdveso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gzwlrwicu.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/glgnuazsy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gvvpmlvss.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/ggkeephos.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gtqbggykz.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gaedendbs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/goxpqzjyt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gqspjbqbw.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gwchpqkpu.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkqmnby.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpnjhhu.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gwgnjahwq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqqcdtzwc.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gcyraaivj.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gsofbzzgs.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gvymsywpw.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gbwnvrfoa.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gejvmhbrt.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gpbledbju.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdizlksyv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gdwuuwsah.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gxtakucua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gfwfzfjso.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gmkfwcugg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzchzmtqc.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gctasvedz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtfbafpbl.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gvrqlnodx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gwhstwlhy.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gzighrffs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gdqvydzbi.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gevxspvvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gzjhcngly.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gfldhroli.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/glikthfdu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gglvcdcjc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gwotdynnh.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gkpamgedy.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gvykplmyt.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/giibedyec.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gdkmvfgfz.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gxbqecwlb.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gvklyjvsa.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ghwwyivxi.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/grluxxjpr.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gzicdyoej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gkvjrixns.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gdflkpqsf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gbgnscwda.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/guhosozfw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gifyvkwvl.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gvxkizxyp.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gjxxkxmue.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/ggbuwcksk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gdxurdhkq.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/garxeqbil.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/grkmtogel.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gsgcsnyzt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gosrnvhlf.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gehziaynf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gbekugfea.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gcremrapt.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gmpqmfuts.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gfxnmeuky.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gidiveiei.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gckwghtvd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbcyulvdr.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gxvlocopz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gtkzluhwu.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gaadqhsej.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/ghqenburw.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gaceocgpc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/ggzfiekzg.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gdmlajxcs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gwtniucnv.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/guvtjwkid.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gngepqgzi.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/ggyxzyfqp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gafvanacv.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/golyjkgmy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gxcakvwoe.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gyxbojaxm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gnnsldvqy.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gwbfyqqxe.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/ggtoqpeev.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gcejbztwd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/glfeozncy.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gkjqxciib.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gvquzzdyp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gjdpjysbr.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gqgljndhh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gagzgtlpa.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gitysjfgk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glpyypkhl.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmvxasnfb.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gbmtsimac.sHtML


<!-- 参考信息 -->