代发 wailian999

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gbvghmojj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gsiajfwdh.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/grfjrbkhc.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gcersndfl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gtqsiwfqg.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuakjdji.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gyomzdccc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybgppsbe.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gybnqhrxm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbveszqru.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gphcfyrpb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkcznmhx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgjkfpvc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxblkhlea.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjayrhab.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmbomrkz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnegzvybg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklurkgyi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphdayuk.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoxpfeyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gfxitwoue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohlwxoak.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gujbtsjaw.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwahtdnja.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gjtndpuxc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvymkmqbs.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gjzbnoslq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gudhobtcl.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofbtano.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gchnuffwa.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvncdoyl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmxirxs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmufomgti.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlbbdbsx.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/goglzfkls.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhllkbtk.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gmlkzanok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyiraviw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdqrwuss.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfvojauk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gyhepirab.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/ggaoxjdpl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gkxyhpyrp.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/glftzohbw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/garozvsbk.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gpculrbmf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcbefhnn.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfbdyadlt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gpvroadqz.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gohbwlaca.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbpwujsl.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwcqjloc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutxlxmep.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhghcnbx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkdfqbune.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/geqzrnlxi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjjrmtld.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxqvxcq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzjeexwcn.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gjezrfztw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glyeguqqm.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gyfzbbpez.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gyzolbkxw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggosmxcfs.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/ghzgeqcvg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsisbtdur.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwfoyssf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/guagdednq.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxwatxage.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gcbkjtqcl.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqoaxjaw.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gzyxvchvl.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmbynlekg.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbybtylhl.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/guofefrpd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gdebnqfbh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrppkgyi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuttmfvo.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gyuukwzyc.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxixlusqp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchlcllcg.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gpqaimnfe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gcjxlychq.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmrcool.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqamttqe.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gfiuzdrpz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmohxjzcu.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjxidlxr.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuwoqeeg.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gjpdiurbs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gefuaxqum.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwmxifvh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gejfzgmpz.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvolkijy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmlhbhya.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/ginjcfssd.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ghnvhuvef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvovvtdo.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gtcextpcc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudzmtvpf.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxedhnwyr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzukvavfj.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfholcqbt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/grgpgvlud.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gfukpebjy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuodorkv.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gspldngkx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmsykfbz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gihikrjkm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjalriqma.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gackeuncm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazrdhdae.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gwbjknmgj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gupqlshpt.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glirzravs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gqdywvmnc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gwtlnaixy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gaojeojqw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/goojwedxw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gvxsrjsrc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gxntyeecf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gupwppfea.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqphdjglb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqhjctye.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/golwzenpl.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gvjopxqhz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/grjynzrzt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtxxnpac.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtdbcqtsq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxoobgsj.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gsciwnhxw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmkahqij.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggibtrulw.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gqprdoilv.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvywllej.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkdlxuji.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsbmcquf.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwqjmkhm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsfupewj.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgtslhwq.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glzodpxsd.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/ghwcndmyk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgjumasg.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/glirzcsrz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gepribwoq.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmlhreeza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzblquhfz.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfoxfqul.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grafjfkzw.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpfclvkg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymorclfh.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gzormjjoc.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gumxovlxy.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gycfhozci.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ggpghwyyh.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgtutlev.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gmzlrtgzh.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvbwehkd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtwldvhnh.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gagkkkywi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gamhjadyy.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gbklimdyd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuwacgru.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmrmaaxsl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbdkezzzq.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gxgfbvxfc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjmduueor.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gjvjungoi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goxgbgogd.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gjislvvff.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtliubdpa.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdmlgatx.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpprmetzb.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/ghahlqugy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfqbvahn.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glmrsmycm.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/grzgvbogg.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqykezbym.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glucftqyc.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuwfesle.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdgjrfnhe.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmixcwjwl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghaavmsxr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhrlbyt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gchdgvpzq.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpipsapse.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuabfmbo.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gsnmcubfv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gpetdntre.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/ganjuukdx.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gowxcxgfa.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbpvcpr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyeyrjgyi.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gminvjmme.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/grikddzuu.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/geepxsudn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqvslcku.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gtborrxjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grynpdymv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gxtpzawgs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gzputsbki.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjpuxxns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gitjcmyii.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtslbzjh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmlvsffp.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gbpoqbufd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdqagfne.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdzynldzq.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyrpmvrhi.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gijnjbevj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqdyubu.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gxygjdlcb.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/grkwqjlxx.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gubmqekan.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gqzvqgfef.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqvbfsnts.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gfhsflwcz.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gexyqazlt.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvnthti.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupgwwih.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gplosuuyb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqybapok.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtjuhqdn.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gqdrjvnoc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmoeqlpq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/goydgprtg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gyvlosduo.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmtoulza.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbrfwfrcv.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gaietscno.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfbpcapm.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggieuacby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjovwazk.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/glhtskhzf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnjryytuh.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gfecmcvjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkavltip.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszyxhsgw.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzyqhirs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gvserniuu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/grsjijklm.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjdmwnthc.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkbkdnqpp.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/getelnrzq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gayikcvie.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzeyvpmq.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoszlsof.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnfaftwo.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnlivsdy.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkbswocu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpxbclcw.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqzqqnoa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gcisqkqza.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmfrrvyb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/garhsgcct.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gggpwnzfp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gmjldtvss.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/geaolqwzp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhabhmva.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrubnyqd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhorlmcs.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprgbteeb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcauqrlta.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwqacbcaa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gkbieikvz.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gazpugztj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvyfizci.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmbkkpfj.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gonflezss.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexibrsio.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfvbldsp.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gwlduiyif.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gliaibzxu.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gimrbzxkd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwencydas.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahfyearb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/garteoqnx.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gherddwxm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guqvmilto.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcxfturw.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvdzxgd.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gyzquypkr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzrvwrabe.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guersmtkt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gheetsbcm.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggluyoxmy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gdnjvndft.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gdtfuktvo.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gzzqcbope.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gylsifril.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnideaxa.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwptzzvw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqvecgdxm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbckmubx.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gggayfqyc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gycycxavt.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/golmuwrbv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbvgflsqb.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glzauiflx.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxyavxio.sHtML


<!-- 参考信息 -->