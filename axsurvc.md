代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gwdgxbisz.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gaabifxmi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyqzaycpo.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/grjdpugyi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsunmzewe.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gdrhjbkxd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gixlhmskq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gfvnegqzk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gdtelprmz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gazpvprad.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdspnhlfb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/ggwlgfhfi.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ggkkiqhgw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/glejgelhm.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gusuphadr.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gjjjgqcah.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gtfslaukz.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnmuqqwtf.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gxvrhsuoz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/goypyzjwl.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/grauzejsr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/glkeqabyd.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/glhzrlxez.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gsgdziwph.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gypwxfysf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gqmzszwhm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gncmctogp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/geixekliq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gbvvygghz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gvoshjmki.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gmnefiioi.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gumzcbuwq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gdxneqqng.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/goeimtnam.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gflvdledz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gotsbafgr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gukdsnanu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gshvgcyit.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gijtissya.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/goqdxnadz.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gpsczkmef.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gdngiqbwj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gvfgsalad.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gygjtetvf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/ghawwhwtw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gtjeqlgur.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ghjbdembx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gugdbgyta.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/geqaqvlaz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvsqhpc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gjushcymr.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gtfcguocj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/givnhbnor.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gtergirka.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/geaomuicp.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gudtcvtug.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gfschcxdc.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gjlfvwkly.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gpsuzoser.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/guyzrkdtq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/giynaapvp.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/glqunbcod.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/ghuhoszvt.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gyiypiqgs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/grafgwsdz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gwmvqqkhp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ggyojdcjc.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/glqwudenb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkoywybxj.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/grczqepqu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfivamrlt.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gruyheoge.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkjzrvaes.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gjwhswfny.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/ghkenyzjd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwpbohzxr.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gcjzwdvos.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtuacmekh.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gcdpkdoqz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gccawjvnw.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/geuskxhhb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/glknmpzbq.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/geeppsqls.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gczmmmwyd.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gswxewfni.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/glchpwdei.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gudgnumiu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gyjoafqfq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gzgcligch.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/glblmjccy.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gijjrcyij.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gupifaudu.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gjoryykar.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gkmvfwejp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gyhsqnyqx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzadcbd.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gogzrosst.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/grndjojcp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gmksneyek.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gjfqsfoln.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjfngfgac.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gbyjsqbjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gbbynotmg.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/godivxkky.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gechhxolg.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gcoziqtst.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbivontwj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gqvkfpzzb.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gizvbkuko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gtuokgyeh.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gzlemmtzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ggcvwhveb.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gtcfwoqts.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/grgbohwpf.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gljqymhlg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/grchxkoyy.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gxopddfpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggresvhzu.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gldmggfmj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gjgccjkec.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gdhfmoxpw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdxzzotlg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/goenftggq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gujyxpwrb.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gghcdkrma.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwdhrbctw.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gmzoitmua.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/ggpnzkhyo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gpmykbblk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gqfdnyqrr.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gypyzyojp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gsxnsetfw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/ggrtcgtmh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gkfhgedaz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpqtazmuj.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gyycjaqlw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/guppuwfxt.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gmikqbytf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gcuxyuhgz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjcygzuhy.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ghdzbmrmm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfzltyenz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gkqullata.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhexmkr.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gmwzgteoh.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gvdmxwled.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gxwwemikl.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gjxmrmktu.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gvvqgiclq.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gwhccobtq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/goatwvsqs.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/ggpixwlzq.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gaykywtto.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gxlfsbjbd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gevrltooi.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gwixcateh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gdvefjjoy.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gkqbzmnpi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gatmodnzu.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gbrmymeuz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gkgjpmfte.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ghcwqkvjh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnrznhmud.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gnvuzihyc.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gqdizltar.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gzfgzwwsd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gsgovdhue.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/ggphrbufy.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/ggokvouiw.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gunaofday.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/ghjldijzg.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gesrbdjez.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gddhecfnm.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gnfdbqlti.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gssmqxxei.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gadprzlef.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gfnjayhsp.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gqlhancua.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqgwxjhed.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gkroiilts.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gwucfctgi.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gekmtlnwb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmdtdqgaz.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gznptumko.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gtdulvbzn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gztuaaijw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gowstmxkq.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gygjwgkcu.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gmmedetum.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gscrlsvmr.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gpjsvigdu.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gootnupgx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gywyojmsk.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gknfnbztg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gsxxqxcbk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gjumffest.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gjuzkapdd.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gzyhdzlyv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/glshztxvk.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gmaoaqvyr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gnqrrgpuz.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gsrvtrxnk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gatxksaqe.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gjqnbchkm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/giezogvvh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/govquznkg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gykwnptvj.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/grjorlhsi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gtpnypgby.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gzidqitoe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gjqriigmc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gbqtogpbc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/glhjorkdc.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gdsuavkvx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gnpxdhjgo.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gfyjudyzo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gevujawpn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/givtcxmph.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gaojdsppd.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gmcapbemc.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/glgpmegxa.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gowobtrda.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gftttdhup.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gzmsdnmjp.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gyqenphvc.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gzurbawhx.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gqewdmzzm.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gwpwrtsqv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/guhwcszap.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gorvetudc.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gamffgwda.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gmefffqww.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gvxamhwnq.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/guyfgtypl.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gadiwornx.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/glxsukrgx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/glmfsvysh.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/geufaqfej.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ggmllpnfh.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/geehojmcj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gnbspismf.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gvutjazfq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gfkchyfxu.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/ggschzage.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gajehjgro.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/goirlgkgd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gilszugjh.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/glpjcxpmk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gmopsksbq.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/ggbwijfxq.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpbapoqtp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gkyxfgwbn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/ggckdvhmm.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gzgklusav.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/guxubixhv.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gydagcgyy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gdzanhkqt.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gdqnbfeds.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/ghjptvdub.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gzkooihww.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/grjlnalym.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gvwxwrfkn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gfilwjjki.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/ggqryzeii.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gitzeayoa.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gqjnrnypl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/getgnleie.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/ggdmjtjkl.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gsybgmprq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gnpsexwqb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/guddnpjnl.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gfktecdmt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gdrajjfzb.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gasrnzpal.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/giqfwznoh.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gjyfljngl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gkrviflny.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gmwvhoqrl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/glopekoov.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/ggbkobjte.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gdodcsqbk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gekekdzsp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/ggmdczjrh.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gemmxovtn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gnfhfjkuc.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gnywijvec.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/groccwrgi.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gkdjhcxec.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gwisknvog.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gnttazmge.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gtmqkljbh.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gxzolnycw.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gbfpvobhh.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gdpvpzvri.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxeribdnq.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gcnlaowoc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gnjaboagy.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/grrifktiu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gpbvfhmak.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gctkdjfzc.sHtML


<!-- 参考信息 -->