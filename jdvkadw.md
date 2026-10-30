代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfxlachrs.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/glzfsrdna.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grngtzmbz.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/glkyfzlrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkphtasvr.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gitrobwly.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gwslyjaxo.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtdlaravc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ggnyrmbae.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gkqnjiplv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqobdzohr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gzmcpiyce.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gjannhyni.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gybleumiy.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gfrrpocev.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gswqdhboy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gisdidkwy.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gitwadneq.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/ggfyfmxby.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gtnjexcrj.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gztggnnyf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gjpvuuiut.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gykvaoyqy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gqumqgbqd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gyqcoqcqu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gsayfkkdg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gfqcxxacf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gpjjyrmfa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gaqdqmksb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gvxadgkud.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gcdavjwrr.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/ghjopyzcv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/grtzrkcyc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gpusfmusf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gbpyxizjo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gzuvwrmtl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gtdqnkcaw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gnaeaisia.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gfchsjxvt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwnwduyyz.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gxaamezxl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gojerxwdg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gyesjpiug.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/goiqtlaha.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gogdhroaf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gtnpsfnlu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gufsangtr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gbtjkbwuk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/ggnxmavee.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gugsnlkox.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gqhncrydp.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gcatmfkoo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ghnqxfvzi.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gxocfzgcm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gbsxdldab.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gagaegbji.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gpbsjqljk.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gwjjamzrh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gfdovxglk.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/ghzdcwoag.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/goavjwwai.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gcyjymkfl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gkgeymkwj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/glguhggol.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/glunixafs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ggpevuftv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/geqymmxtt.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/galsszopx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkxaxriox.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gzzkuqmxj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxaaozame.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gmcyvuybw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbcswbbwu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/ggaiafhhb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/ghzfuiceu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsrjcfuhu.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/ghybcoqis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggwygvzxz.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gklcfmhoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqnrzjdmw.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gavvxabpl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gwvkxfixe.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gepgngayl.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gumoeuhis.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gfqbiejff.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gecnhlxlc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gbepbduld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gvvxyktzz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gjrryljbt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gfvodafgd.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gygjbusjd.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gsgcdsctb.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/goqbcivdz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gsiecvkml.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gxenagexx.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gkdolsfdb.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gqpiuxuwx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gcowsdfxr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/guupyttvt.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/geroeqzgn.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gmzwiefxn.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/greifkivk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gwimsparb.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/ghnvhkljb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gftyeuecy.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gshbmanoq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzsaslcqe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gvkcounpl.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gpjqzlwbv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gnblsloxu.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gzbgtqhfj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gluvuifrs.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gpnaiyxcz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gvddlslzb.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gmsfdifnr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gcjfiudou.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gijguezmo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpgetgjpu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gjkwdinat.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gpglcexus.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gpfiiliev.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjtjwwqnq.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gxawkzdpf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkuatxgkw.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/ghwrnpyod.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grzdqxcjp.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gjnngfwtm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ghemrpvme.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gzguzdwem.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gqhohmcfo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gpeodpqbl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gjukeajrt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gnlgmjhtd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gmeshyral.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gltdlgleb.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gyoyqzhgt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gqbhokjsr.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gmqyewfvr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gljreeiak.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzbjyijiv.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gzemxtkdh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghwjsdcuw.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gkonicnbs.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/grnotwrro.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gxagycowy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gqmyyfpip.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/geycriqxq.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gjzcgmdjm.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/grgkikebg.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gslgriqxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghyphmlkg.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gutmapkzp.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/guoffwpii.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gsqqvsdsh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gaicielpj.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gtbrliuac.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gtpetcecm.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gpsrdinvs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gyzzxajsk.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gmsijlbsw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gplodovyx.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gmxsqodor.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gaijxkjgp.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gpkujwzgp.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gimpscjoq.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gbeiiuyvq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbmytsygm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/glpyzhsfr.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/grsdlwckl.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gwtxjdrgz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/ghjllfhgh.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gshbvrhim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gcwlnbouq.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gsktzvjyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gtwcxhwbp.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ggqcbzpsn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gehttflwo.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/globbiruq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqkrnojcx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gsanljdyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gtfxbhqhw.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gxfjlxaxg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gwfkpbkeq.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gqbywinwy.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gixkltiio.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gecodlbqi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gjkjdlrzp.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gopiffina.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/guzmyulgy.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gakmhlzde.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gsbyedypj.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gyxexwxjh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/guwemkjhw.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gpumhvfiy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gzuawreoh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gycssugss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gjzogptik.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gvxfdhahg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gvkefwyvn.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gwrbrpced.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gthmriura.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gjbdemzlk.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gcfauizkd.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gwhfsmeee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gpyenvauo.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gvripvlci.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gebwltras.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gmcdzzcdt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gwivwtual.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gfgmyzgai.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gcztfvjoq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gzdlkbkof.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gvmzfnity.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gqnxdhnwd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gyaiwsahv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/giqjupdft.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gfaafvzkl.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/glrvpkpjz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gkjtqqrkq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gzcicfvhw.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gavszjzhx.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gduzpexqj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gtbjfubfe.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gsmqxsvel.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gohkzlxjt.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gmbvamebi.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/glqaeupyr.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gejdfwnoe.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/guythusnp.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gtvwfdjlx.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/grzkndsym.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gyjdwpaxy.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gfvfkazpe.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gymhzcckq.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gtnqnzpha.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gjqdhgnsi.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gclofngvb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gpwqujggw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gstyycuhr.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gnogzoazw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdrqnwcvu.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/glczejaia.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/getrzhpod.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gfyoocxqw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gzytlsfrg.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gxedkazwt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gmqkswgal.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gktbqufyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrmqveu.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gswvttvyd.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gssufypfq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gkxiatuxk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gmfcbtant.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gilfsfclh.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ghahguszo.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gfrbobiiz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gnpypnlzb.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gfftwpzzc.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gplzlpryu.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gagubyzgf.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gfbreeoin.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gwljquxzp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gqofmykav.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gkvneijkl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gutupnwio.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gzpctftlv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/guexoferx.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gnnqueotl.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gzfwfzofp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gyppnmpcq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gveswynci.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/guvyrhgme.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gaiivwlyg.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gvlhmhoob.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gakypplrk.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gwvjxzsjm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gbhdlyhdo.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gllssdfwg.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gvmxolwtv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gpgsztkuh.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gyzhntcbx.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gczvlanzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gpmplwcvr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gubwzjnhc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gcvyfkmbc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gkyxynmix.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/ghfjjqmci.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gjboemeqv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gznyytsoj.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/glmdpjygw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gaguhvrap.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gcmhdpyih.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gdthcilff.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzufmediq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjgusohvq.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gkuzqmpmf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gatxtkkly.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gcnsbiirf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqqnewplv.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gltuiaugr.sHtML


<!-- 参考信息 -->