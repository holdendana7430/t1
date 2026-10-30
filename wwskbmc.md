代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gicstekyc.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gaxtvptta.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsnjyxrf.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxsimoeq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggucjtdfd.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grxximawr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtmuades.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gvzteepgr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyjwweuy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzbjbmtt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/grdtwbdji.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/ghienjpgm.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gqfmyrlax.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbxlsbww.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gxsavuskb.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnynqsoq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gjrkzfpcu.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gafmdskat.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/geebpeoge.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpftogeg.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjshqpxd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/grcbtpuep.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkscpxglo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsawqfyhz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqcctpbs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gavxgxtld.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/giywxtknb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrglgsnx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkfmqhcl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxfagxgt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkvwgbsm.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gchhvutku.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxctvkctt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehpposp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvanccct.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/glczqdxrn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gkpvbbtbv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gdulfwrot.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyzgksco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gufshfhnj.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gnkcauvye.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngpthjvv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gsrgbnqdk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfdltjdg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gmcshxtmg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gazmvadrc.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggrmgeivn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkgbydy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/giojuicpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyvledfj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkyftrcf.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuzogqqm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvynoxxj.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gsgavhgzl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpvsaqzs.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/grxkvtmav.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvmlrzfo.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzltyddt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlvwoirz.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbcivsw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gxghxhfht.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gtpoefkho.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckmxydj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjgeomjc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjucrdksd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvstfqxn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwwtgcwj.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/ggpyswjmm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpleccupl.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gremyycqz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfemfvutk.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyazbwrk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwunkeans.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrrtmaoi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvlqypbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gyspiqpip.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/grjtmtjih.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/girdctfmv.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gnpnyprsc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/ghkyptjrs.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswoyhvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gbzoddmjb.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gztrmusqf.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/ggryyeslx.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gczgbodhd.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvdtnjw.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gdknckbhk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhidbxvq.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gthrhapdp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeucgecr.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvbxwgei.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gceqgyhtm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigagnrod.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gggnrthlk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gbjcfmnef.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gggkehhxe.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqnzneej.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gccdvofmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gczcvbyke.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgsnrwi.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdftduzdf.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/ghqgasofh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gvbrofevs.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjnqmxyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/giaxxmyuk.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gqgitycbw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxpmlmvb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtesomrrt.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grvhsyudt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gdoyzietp.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gdsobtjqc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gixiiysml.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmmsevhsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gfhbepopw.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gelfhibkf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gvslzonfd.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gywmmzspa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gogfiqsfq.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdqweuohf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymtkpfm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbhgvtzg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gidosujwd.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/giaclecem.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxznqifsn.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrumqyt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsloxwlj.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvqiemzk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhknppln.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgtmahbb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gjdjlznlm.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqrcjrytp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gtueydoix.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjpbxyzt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxqrhtb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjgwqkyy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glythvuap.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngyamwtz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauxtufck.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/ghgtpkcbk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcreghufe.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelsowhf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzlamvwey.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnohpihck.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnemdbbf.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlraktrg.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gztvcqwxy.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/glgvaccph.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxbnsnce.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gyydallrs.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwojtlch.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/grqitfrst.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gsyfakeez.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/grtvjrypx.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gihedtadp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhahmwuc.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geiicgmhx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewhbotis.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvuxmesu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxexhvmj.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginwpftci.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goqdywbfg.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghxaskinb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjgihqrk.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosnvlftq.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxpsqfzk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxzlyaw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkhhrnao.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvxlaibh.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gcvtypyqy.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmyaplpjy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufhmddfv.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gjjpikitf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzigtomyi.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gxafwpqmn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhbzcsdi.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnustmzt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtorbysmx.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtmfefhdo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpjfnqjp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwjkyljb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnyldhayh.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvwaojod.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymyssvoz.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrflnjzb.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilnwcxqs.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbocdtsgz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvbkbpvi.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwvijwsw.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjuycgiuh.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gywzeelns.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnglwlsks.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmifkvupo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmqkmdyie.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gamvuglcv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/glqqmskcl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gwrazjfqw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gagumqmsc.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggxhmsald.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbkaelez.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glczfmlsc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gtsuxkboe.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gjqlxvfsr.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzgendfo.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/guashyqfm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcafbbhri.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxsmwhgiz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbcfewm.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gblybutlk.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyllyzwo.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ghqbqbiag.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gssazzxdn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggswmeiup.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqnulvelc.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/guyobokoq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gexddjnbi.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/ggwzhvrcu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gqssbizis.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/goisuzlql.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gujupprnm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gttufysop.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvztigyoa.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gctvjugfq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpznhsudc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glqsxykkc.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpyyegkr.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gahbrvwsa.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/ghrebudvv.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/galfxhfpc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcoxpmcdf.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gftsflchu.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrooorlu.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gevzdwzpa.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gsjjppmml.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gajssmibc.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdxncynfp.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gicmktajj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gffudwcdj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gqttciabk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnskiiygd.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhhqsruj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giqleonxa.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqywkmvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkxvpeebu.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqppzbnyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/ggqdpgrpy.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkxacqov.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakiftugn.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/glbhauoua.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gvcfdjinf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gnzlzlski.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gckjymvlm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcfvkcgb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glmwfdhlg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galyxgxly.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gizaqvwgz.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwyesjcb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmnqfxxv.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gegxksqzd.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkpjskxa.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gydrnqugb.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvirstsf.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/guyxnzpaz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gcsotgbqb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/guyedfwng.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbczobtnf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfnlwbouf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gccqlnhnn.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmxovufz.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpowuzef.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaklskdhm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtrucwfp.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gofqumphy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkgencub.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/grawadtbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtvyzytp.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnxnihz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gwobnjthi.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkloxlvc.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/guxgcvgbc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gsizpvssn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/giolgfcfq.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzvhfzxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geonizoge.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gayiedyde.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrwbghcn.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/govqzsprt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmyeispf.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvczwjayc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gswdhcxec.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxlcnjlb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkmbhjuvx.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gadhsgsaj.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwonaem.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhbkmmgi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwmdqekn.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gyaqtqpub.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/guitsayrh.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbdqzlfbi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbndbqkhp.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gjqnrqanj.sHtML


<!-- 参考信息 -->