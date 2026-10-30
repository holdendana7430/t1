代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gyhwswhpp.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjegyqijl.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gzmqdsuvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxhfogyo.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gmujthdky.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjxmltrj.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtycurugl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiitfeqz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrugqxri.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpfjnjvw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gpxkffqbo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztjvsvsd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gntgrsgyc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gusxnmpid.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqwmyuvi.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfmzkplu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgofnhyv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqmymqxe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlguprhm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwkuudo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhkurznn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazkmiiao.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuswrjpx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdlzizda.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gysziazju.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gnvqailhc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsipkdawx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/glxukwisu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrlbqwfo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygdwlsur.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gjclmlaiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/ggmulxxrh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggjtfhkql.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/ggjlafjyn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrrqvulg.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwafobcya.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnpbgbp.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfxwcoxi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfzdfgmb.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmpeqyum.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsatpzswa.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdhkhfil.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gopfkzlmn.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrujcxcj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gudsopfae.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcilxxp.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gjuihjmyr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqythluw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gtlncearz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gicyemjys.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ghihzqkhe.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gowcojayn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gimjttjih.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxffvzmax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/galemqhnt.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gmdbenbgz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqczgsen.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufhxtnuj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsromabwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqudwfduq.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/ghhvucabx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghprffmtj.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslscuhuf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gifeedffo.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgcthaqb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/guamnacql.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpdibtbs.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/grcjqbdzz.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gjdhbqzmb.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gysbnwcgl.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuqgqyqj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/glyemtvls.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gequzczdw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gbqymjwcn.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpsyhviv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrgnhbwo.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gkltqkfhl.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdxaqnkn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gddpfibhi.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gwarnlagm.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdpcbex.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlvqvozo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gesoeqjah.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gjnofujbx.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwloxzjbb.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnhbzjck.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvdelfni.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxwawfl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqqmtcu.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndlctvwu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gplgkepwp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gtktxrocj.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gtrckbubt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrqvwbnd.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpjtoavm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gleaaackf.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoctwznc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gcdflxfuu.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gyifsayyl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gzxiqjpuj.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/grulxkrus.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gikycnxqg.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwpsdcqez.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxjnmrge.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gosfpxhmz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkwrmoae.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gphbmazlk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuvcdwnw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gredwiayt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvxdxcpx.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gnkyaklyv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gxwoujmhc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaapdtprw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gctkhokqw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnakekpae.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gdhbiwssc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyrmwdbxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchxmfgic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnuhirlci.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gihbgjpch.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gjzxzvjew.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsenyvhe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwgnwlnw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdpomdkdp.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gigshqxsr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnfjlyvf.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuguaifh.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghdptjpbm.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gnthsolzu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpohfhbr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqvurcwf.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeecchpd.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gqblggclu.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gapkkkhvj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gobmvhumg.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gokxhgorm.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsonuwvgj.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/ghibxutjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxzhsxtrt.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqxzxbpk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gksgurepz.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gahxxyhbx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlmxymad.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gisakhfwn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaftrrli.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gshbupvqp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvduugnlr.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gdolpptmv.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/giaethlcb.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdvvswnw.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwwytmg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guvpwbitk.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/glihhresr.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmnjjtuna.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggqwrgqyf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcuzjfbw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gllsstlhb.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gksgwcorr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqodrzzi.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwibheun.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsdzocnsb.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grxluobyp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsknjafy.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/glvazuczs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmztdtvd.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/grdwqttha.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyyvfcz.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdyghyqe.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimuopat.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gnfqbojxh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/guivrsemh.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqncukam.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/glyrnbswj.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrucjeo.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcgldfez.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnjjckoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gljlyyjfs.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gckbkoraq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwnuiatvg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbdkolmg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcafiayay.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/geuxkpirb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmubtuqdx.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gpyueiquc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwtwhnil.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gpippjand.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gpuetldfv.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvzrurzgx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnqdzshs.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbjwybkfw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfmoikkm.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbemhbmdo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksnlrmvu.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gaesciovq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpdrawnhp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqbyeowj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gehbafeiw.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gdxhcbsvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gfnownxxw.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gqmwvoity.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gulyncsbs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdowatcvc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/grfihhhlt.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpywdoxc.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytrwvlyl.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gefbxhuev.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdwvsqopu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmdifevg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnwvjhdf.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpsdhqqcr.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/glfgazyjk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvfibarn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnecyqdl.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gljmponpg.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrxrzcow.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/grzndytdc.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdjgvtoh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcvqalic.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvpnjizy.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdyqjdihm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhuvvuly.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbxfznzy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbzpmcqd.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzdxhtbmb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpnizylku.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgydqirp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjsdhfqf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnyqvbvfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpsbamup.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhnkycny.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgshnho.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ggkyfsfdl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtexjmen.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrzcopq.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvkzsvsej.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdmncdjy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/guzryuygo.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdrcizfq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbyzdxaw.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gynmplnvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimggaorz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxixemiv.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzosqtui.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gonbbqknz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhqspqrm.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmavguxrb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gxgsfmlyq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrfiqnjv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxdsyipha.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrwnnkyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpvwates.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwdivgcf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gkguheijj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkdrgpkgw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfygerzbf.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/goawqrfwg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gvsyikccg.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlnofrp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/glakjszid.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gfgnanpaj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/guuvlohwp.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdniojiq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmppsqzaf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdsgbsrx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gtlxstpbf.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gjhygbeij.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gghwnoszi.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnxlqlh.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gmzinqsbl.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gdtlzfpui.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/guxjglyxt.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnpznehqv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwebgyvf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqljslsb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqmpolwq.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwsbdaga.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gajhtvtuj.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gquvsugij.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gekjnlwes.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesxrzomp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyactgodq.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqaonuga.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftpfjdqb.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gueirwmfr.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfynpajv.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gckgmmzvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgctsbjs.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gfmbogsgw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzxkiefap.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gghucxzic.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gllsbduco.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpexhrbmg.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gqindleuy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqpcgdoqz.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gavzefdmk.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlwmdfcr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gihufbiba.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsaeakns.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggcngayuz.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsyrqqxs.sHtML


<!-- 参考信息 -->