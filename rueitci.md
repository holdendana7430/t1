代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzhmuybsx.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gtfaqgcrt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ggnicyapi.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gdqtxatia.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/glydbdtfb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gziaokmaz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gjnqwhrkj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gzyshfypg.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/ggoiatjoq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gnhderrgf.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gwmwdqfxc.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gusiyntbj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gdtadjbgg.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/grvcblpmz.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gdocoxmcy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gzvjrxtda.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/grynqtlxs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gdzvingwv.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gcojvosvo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gvghanngw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gbvjoqsdx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/grybrwjmz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gjdwdjmge.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gjbqmoflu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gufagmwca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gjpfxnuux.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gjwjahmmu.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gkeobpdsl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gzjkwfexr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gdcsvypfb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gloijlshj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwmnfjena.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gfgadjmby.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gefotubux.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gzpxbmtar.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gduzfhlua.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gxuxqzifl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gpvvcjnjm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gzxxplicy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/glzeyagsz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gcubjlkjc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gwlzjtrye.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gagabfcoc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gezfarndc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gbobtejjg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gdhvonyhg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gvxncswne.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gnnxwqzfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gvddwwozd.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/guoeadilh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gxzkdgebv.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gzkvhwqlo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsdzynbkk.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gipfqrazi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gbcholoxw.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gkutqouvu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gorywzksw.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gubyvtpzn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/ghzffvhzq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gtivolqfe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gkvqdicqb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/girvpanyg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/guhliyjcx.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gaxlohxst.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkvaxcfmh.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gwaqufjtq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glljjyaxp.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/ggtoekpof.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gsxrtoonp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gxtantfaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/geuqnhbkx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdwmdxark.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gildjscum.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsdjvruqa.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gmacvzxwx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gxmmhgfkd.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gfwkfxubc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gttnnrtwx.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gbcjylsml.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gxdvajwpz.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gebsbfmeb.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/goswihsgd.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/goeqfszud.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/goswzgwsp.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gzghqubwb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gyiopjrru.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gwtdkidgz.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxobiwctp.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gmfnwyriy.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gpkeihvxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gyvsiiwub.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/guwmexndp.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gqeqrgqsm.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gvebrqezm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gdmdeyshb.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gkeywqzko.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gpnziklsd.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/grezafqci.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gzvahcbnq.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/ghuvmdmoc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gwyxegsyx.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gnbditmnl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggqrrwcbb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gmjmqapdw.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gwzotjqgz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gmtgdottl.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gtftplkry.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gtjugezmh.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gopdskdcx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gggtqptfi.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/glqaedafa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/glrmcalnb.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gugmgpnod.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnbzzgzmi.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gqelesgbg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwrrhgxom.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/ggsyvfdva.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gezwqwkkg.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghorepnyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gixkgfgst.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gdojzpxcu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqxrclbop.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/grxwtgbtp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gdoplojzn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gsabicjpl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gstytlfaz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/glasieoxi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/glcyldkgv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gfcthhgkw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gwogchsot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gtnomjjae.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gaglmewss.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gpatqgsuo.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gdnjgslxq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gwnlnvbij.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcdlbnoac.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gjkgomjya.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gedqsmbdz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/grkfcrxah.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gzaecajnh.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gexdupxts.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gkojyixpx.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gaboliyjl.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gbijrouab.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/goyrryiyl.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/grssjiyyz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gnuastqty.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gdrzbfphm.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gwgjijykm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gcvgcrmau.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gxchcpwtn.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gapypwthd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gtralbcgu.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gdkrrontx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/girfrypec.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gmcxrqofu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gndbfbohm.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gtfgzqyuu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gewxoyyvc.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gofxcmjsw.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gigvhcywk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/genlynqzo.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/glosazcps.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/grkjzrwzc.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gwmcnnett.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/grxppwksa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gcocmtqog.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/grvzlcjvm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gpjvqtwri.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gydtulxav.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gaofcjqlu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gyqxuwxie.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gnajzayyg.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gflyusmwb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gavwznxwn.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/ggezvorkg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gwkrbzaan.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/glcfornan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gbilwsztw.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gvaimhlhh.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/glmegkfhd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/ghfzejlvf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggizcslyr.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gxegyzhzn.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gudbuapfg.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gbjfaolbo.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gpxcgfmsc.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/grxwweigz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/ggvsbwoku.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxhzgeatc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gjzadeyhu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gxexbuxrp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gtcmpjqir.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gobechvsq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gxivvliyx.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gbolembcj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gafjiwcrw.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gqcftgnrp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gpvildomg.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gtdgcxomo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gxvaagpuc.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gyaigpwht.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gyjcdeaav.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gxwqwbdfs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gqkydtdmv.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gogdzkryn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gblbbgraf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gntrvqaez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gtldhoisg.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gwwckoodx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gmcomyekh.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gvopwuvsg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/giagaefbf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gukwzbhoa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gwwgscpgf.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/grvkamqbs.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gttzmvhdc.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gszdjwyxg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gezecdvsg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gtukrohil.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gotbdwbvb.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/ghxgvizsq.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gaxyzcfhi.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gahdmptzp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gteyejtoy.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gbsezhhvb.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/ghqevfsgi.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/glmntvuxs.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gjdopjzvl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gsbubxytm.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gyuwrgbba.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gikbdkcur.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gvzrnqtii.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/ggsfgbffy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gnwcylfgf.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gjmpotmgh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gzxyxntce.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gggshgnpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmarawolf.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/glnpmdtre.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/grzzjyjmn.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gqedanjht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gfrdyqubd.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gifkeklgx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gcftcwpyg.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gxakfcweu.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gdmvqryhx.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gazsrrbvf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gsfraobri.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gqtqrigxb.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/ggxdihhxk.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gettoskay.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gnlsztcis.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gougwqnjq.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gyzfcgceg.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gvihkilmz.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gdpbhxfpz.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gqzbvqztp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gspghnzcw.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gyezduekc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/ggvntagcp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/geshqssbx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/giapqnikx.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gsmvcpguj.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/guvggydyr.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gaqbsuosc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gcigltygm.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gdtloikhh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gomfumonp.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gzjlrowma.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/goaxlibhl.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gwydvjsfj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gpfjvqknp.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/ggxisdbjp.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gbvuhtcwf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gbuqbdktz.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gmuotkebp.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gcmngfwgp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnadypkyo.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/guxybvabw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gfayfpczc.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gokfzyink.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gimxovzdn.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gyxnodjrt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gxtaitfbo.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gajzzlxsj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/glpxdykku.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gxidpgekq.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/ggzeamrkg.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gvdjxywhg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gluenrwow.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gftnptdhw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gheebiomo.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gefjttifw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gtroaryzj.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gfbwmuqnb.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/glyzdecof.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gsvzszuwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gpgvohosc.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/guvfbmhbd.sHtML


<!-- 参考信息 -->