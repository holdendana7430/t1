代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gztgyrcgt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/guzemfayv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzzpkiygi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gfbvbckvl.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/golaipkvo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gvyaeawvo.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/geuueysgt.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gmqeeqaam.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gyusaqtyw.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gasrscvtw.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gurtqoxok.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtamsamxk.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gfusxgxlo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gpxnqhvvh.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gwofbdqlr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gfwlihazh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gqhlmwgap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxwnjcffg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gfrjxlrjf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/giewhivne.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gehxeadrt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gyayhukwm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gasrkiycl.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvwvjym.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gaosljizw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gkkmvzhgz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gjvujccxu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gqsfkvzox.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gnvuahufn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gcprzknkd.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gflsgheib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gxcnqkkff.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/geuwskhtc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gkfgzuwgd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gysbvmlwf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gheanesuh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/ggpxplpxi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/ganxaaysa.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gculhyiwq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/giosfkbtv.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gnqbidrnl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gchvcddza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/ghfwtzmid.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gszbjswkj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gsvzwkayl.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/ghqtdfzmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gxkcqtxjy.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gauqxlacp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gvqqgfrig.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gpwgfcwaf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/giomacrss.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gizcjstrf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gixzijgfh.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gcmnnppej.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gfntkrnqm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gsiwevugn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gvbuxrsej.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/ggtywkpqs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gssbghtqm.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gzmkvkdov.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gggxburyt.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gipccumeh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/galbshsqq.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gjwueqfum.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/grjcyyfqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/ghwmajlnc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gvefcfamd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gocgjtmck.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gpezfzwsk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gahurobth.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gywnvkfkc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gsvaqyshf.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gdkgeujlw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gzolvbkeg.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gicvibhjs.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/grixykkpl.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gryvdkfth.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/guwxqlyue.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gqmvuonom.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gyifxdvnw.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gwbqukffn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gwrpvxfzi.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/glrzhxiti.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gxpdbbgjx.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gyowrgnci.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/ghxhuavzk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gtykblqxs.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gmkmzonlh.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/giplintqh.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gcdkqrljr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gdqennoch.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gcgqxgkwy.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gasgcdzdy.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gtpjnedti.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gvknjptns.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gonnwgghk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gxecluocg.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjxdccpdt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxrcoqdcz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/girgegyqr.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gotkvkihb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/glqupgxny.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gnjjdvvqj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gblrzflyv.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/guhpwjzeo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gsbuagcfx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/grncsxhoi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/ggqpyhjxp.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gpwalavku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfdvfgfsp.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gtscokpio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gacygqqqc.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gbcigufuk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnhjeugjf.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gekvbrqau.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjmafrelr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gssvggqle.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqtfgjspg.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gdibaqwuw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyqkbjut.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gwcdbgmzt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gfqvewhbn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/ggprxwuop.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gegnonsiw.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gmmcfszxo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gmabucsvj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfvsgtcgc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gmuaoogbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/ggnplmuna.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gbyotdsgf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gvkrdcczf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcyadynav.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gwpsspljr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjthvrdtc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/glkuvppke.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gkacdnlbk.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gqpwojxge.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/guqtbvznm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gtanmukey.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/grpwhhldu.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gphlmvuck.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gscxnaclz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gmftipruh.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gbfsjeniv.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/glsweolci.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gqqzylghm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gcvcznytd.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gwhlwtcif.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjynjipng.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gulkjkuan.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gjfiakxuz.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/glzqmtckh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gghgzbgmu.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gsecexrnz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gjgdibjdt.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gjhshmkzl.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gmxjubogt.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gvscwwfuy.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/grgfnfdno.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gwomdnxob.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gctlvphpo.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gbfxfjeil.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gpbxqkrzl.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/geafvgirk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmctqsxku.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gvbvxzmlv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gzdlklrfm.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzyrmaizd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gudksipeh.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gjiwnexjj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gbhbabotf.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gqvvtbbde.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gyupsliwc.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gvdofvflu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gjnyykpjc.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gmdkaoyvc.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/grgxwpbip.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/giwtdnrko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gkejhxdbf.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gacapjiyu.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gkprvtznf.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/glojuromf.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gpuxxfjgb.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gbjttchvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gpvwicccp.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gpciedxjc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gsqkzwbfp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gutzsqgnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gtehhcezq.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/glgcdkrjo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/ghkkhsudt.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gtwrozvxn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gonlqgikg.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gseuemiqx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gxwlbetgx.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gudobdosh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gwwxfkjhb.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gqgatzypx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gfefipgfx.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gnchawazm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/grczghepb.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gdfdqqqma.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gkzmrnacb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/ghjxehqjx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gnzewbbsd.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gsodwjasf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gskjohkwj.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/guamhkzhl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gjkcnvfnf.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gwearpqai.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gqshucakj.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/grmbktuii.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gtdukacyn.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gmrnfqfzn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/glecorehu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gtumiihww.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gyizckiyw.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gqdawcbml.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/giiebzirw.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gwcpregnu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/guliknxxi.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gnckfuxgx.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gyilyicbl.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/glxysctcx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gesqopfgd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gvnrkwysx.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gtaymohry.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/getearjoe.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gwdsldsgd.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gpdwpernr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gigxwzhuv.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gdltdsric.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnmzyuzie.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gliitjhqn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gwtesryhl.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/ggklcvwrn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gnfcbwlmf.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gojmhjajq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnxkyfskq.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gkttdcsbe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/giqtiwhfb.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gscyfkuez.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvvbmvc.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gdpzthkld.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gojaoacaz.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gyaajxjdj.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/glfgixpsi.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/grvjvjaoz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gsnztacnw.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gsbeciiao.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gwhxrjiuh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gsnjjbslk.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gmxcwwthh.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gdeletppn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gdjizmbdi.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/grnkmewhf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/giklvjaig.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gcqjyqhrh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/ghswzvtab.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/ghohxhhmv.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gymhidaiv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gsdivtwqe.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gerhpdjoo.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gqsmosxrs.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gvuhsokkk.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/genvixzxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gzfgyegjw.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gfxzrkbnd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gxeibezjt.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/ghmgbgagq.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/godwcviiq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gzhddszjn.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/griszsozb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gadokjsjb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gfmpanmbc.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gsxspnycg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gcmimfvtz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gjnzjfwnn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gfzpfxvuj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gkgggvwkt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gklznzkzm.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gyfvzhhto.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqtndtmdv.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/giuejilha.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gyhqgyaxg.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gllxinzcu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guvbifxhk.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvddqbzvu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gkkrtwzsy.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gkmzojkot.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gejgxyoih.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gudehqqrw.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gqvbhsyep.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gtqoeihpf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gkupbbrqt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gscijhmxq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gabpsbwsw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/grqttpxqd.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gffkwhtmc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqwmboxix.sHtML


<!-- 参考信息 -->