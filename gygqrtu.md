代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzdefbwt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcrzzvts.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyhrfqgb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzukegzz.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxvolaxp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaawrnrcx.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gnahasnnr.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkpvuikm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxxygrih.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grkoxxkgu.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdxsrucw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gqnifsivy.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gciowkjhy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gtdqbkpvs.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gakwfxgth.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwdwcyys.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/ganxkcgcz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gizaajrmj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhutduuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxkobqhv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gypytfdqx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviaccsxr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswwyaeu.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gduokqfng.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdzbesxx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusfegtzm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/giytjymvu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyuiluwx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gxidwntua.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzussqmo.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylfvkqtq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gfbgjjryo.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwfwtov.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glijfowpz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdryaex.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryqqnyyj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gakblfqev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gjectrngo.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqonevwa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/grqdqmepi.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbulkzcp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmhadufq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglulyafp.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gdgiqonte.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkewhiiew.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gtydobnos.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbsaklva.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gvwcldzqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/guoudljdj.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvgvimh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrajyklc.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gcvetepyf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrfuedle.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtpqehvk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweqsfwmz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxkhptr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/grfkkdidf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcmdbhib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gujxwxzuv.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gogjsdwbd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gijkbwtcl.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtqbfvhhu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzafqauct.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsnrzohx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhhzgrna.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoymhgqr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsxrjway.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwacodie.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgquuyxf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtpefzyqz.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gdqwfgsgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/grnfteslv.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gycmbtjmg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gqijwnzjc.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxngdmlwp.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gdvjiaswt.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjedqvvbg.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/getgsdthb.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/godukndof.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gnppmfyfc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjznhpzw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnbzrfzf.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxcmgmuj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvcosuei.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthzyrnfe.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gtwwgzbkj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gamwravma.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyoadlen.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnifgppen.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlwtgiyf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/guedphizc.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gborkvxfu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcyczcud.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadwgacuz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gexirbcvh.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfwkdsfb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gsmzjospp.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/goezegzqz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glcuntlrl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxsgzimx.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/glpcuahdr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/glqihgkfm.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/genyfhvty.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqdaaomp.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gfjndxbtu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gpimgawhp.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gykiqwtnw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/glqzeuabp.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/grzrvlvks.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtetsmnfn.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glzyvycig.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdjegeo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfskmtpa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gralajyvk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvllvugz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gshfiidwg.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gayxbpqur.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghomvxppp.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gozwakkzf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gdltuuglj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmjdhhdh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdluijlgc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzraogxj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauibeelk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/goipkaiqt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gbfdupygl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvugbwot.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjckzwlbw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnkwhwbr.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gklykwgad.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzgvnhte.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqudslfhm.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqrzlpjo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gktpsptma.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gpxgzjdre.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghpuzappp.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqtvoogi.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gsefdgotg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqabrmch.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gunesdmht.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwbumnez.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkzrvuenu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gofwbwmed.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ggyqkvkua.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaqwpwwh.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghqaojxms.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcabydxhe.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjfzxajwj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqxycpbr.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkayllruw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkkgkcnrl.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdhvakyux.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grjcuwmxv.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvflcazo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guzlwecqs.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gtyzjryve.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewbslqll.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gyfiwsijd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzomyekbh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdngysfk.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoixmbob.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyormawkm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghuhparmi.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gedmfreom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/givrbvduy.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrtimvio.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpeefucip.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqlswenry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqevnuko.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqdfgdjr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtnscbdf.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gehjpotvu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnhnaxaq.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gulmfsetr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzlofwyp.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gomviertb.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdaohhkf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtulsniom.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/geemrvtnu.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkjiwaii.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gshskbpgh.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwttjoes.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gredubsmz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gaqmghvua.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glyyddgrf.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzygepzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnplnlths.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gexibqduy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggxtbnlaj.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxodlizc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggneuwozl.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtymvupp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gdxyqpaol.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gylnwmteo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/guwnzzjuh.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/guaaasjhf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwsddmqdb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybbyveja.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gyqemavpw.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdplcuxcw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpvxyvhf.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/geppdyaez.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlwermj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmxptrmd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gwppyfjul.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/grxndkllo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknlqoupe.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsckcxso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gtalzwnar.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtferdpmc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaqiwufg.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gekjlexsh.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvdoljdcd.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghprivcle.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyacfeanh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gpxcciler.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksulhiit.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/getfcmoxw.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gucshcufa.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gulagirqg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtojmtbqs.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/goittyvir.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvjolqqz.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gedkzuptx.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gybrptynm.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gkzibvgwx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdgshhql.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gurxtlgly.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrqpxyea.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/grglxellu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gjseyvdly.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmwbkmccy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghqfxrjfv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdfebltu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqglarmwi.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnnpsepew.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/geslutplx.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmblxuqk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giacsfkxy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehhhwasg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtavtrnl.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/glhlgogvn.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmpdmlvx.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/goadmwnsf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gueppcnpg.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnhhzyyvc.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjrigroj.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gfypqlydf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoezofci.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcbotqinm.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gejtlxpfl.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ganbozkvw.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gootqtdal.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlwjzfaw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gkzqvqxwm.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/grlkqmnad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljrfxwe.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gcxsiijvx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfobzmdy.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpikexpvk.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbboeqips.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gatartdrf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwztvvrl.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/glpategvp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/geunpfyni.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gaagyucsq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnejnquh.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gocukdsjf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gbajgbtbj.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyyrzdzv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqqyefnl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gamlwnweo.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxbnqkx.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gylxwpwby.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoqorsuc.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmjndulx.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gnlvjsorf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghslhvnfh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gfissbamy.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcjogqsok.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gdkfhulse.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwirchwrf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gltvaawtn.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjbmhnkp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcaicupt.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gahqzsano.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpsoqzfug.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbzmtjoac.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gictpuizg.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzttczfv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghfhpohgs.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmhigrnn.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzystpmk.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gxxikfkzn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grmslnaxt.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grbvdmqdg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gugljfjuk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gazvwykch.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/ggauzpxyl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glilzeqzm.sHtML


<!-- 参考信息 -->