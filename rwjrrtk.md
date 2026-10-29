代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gridcizvv.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gzpyyomwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjfrztzut.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gsdiajvsw.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/glfmsfbta.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gjgvwrvyr.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gavxqzuly.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gcryupker.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gaqpmnoqe.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwxedgaal.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gsabeldvp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/guhzytvvm.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gzceortzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gfuliterd.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gdmdojokf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/ggruqtxrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gbxfgussw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/goksdcvsh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gvpjskbmt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gynpkcncg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gkledtyqc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gulinxdtn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gueybuphj.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gqlmzxuvc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gwvcyfhnb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gjcwyhcho.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ggzwkiyhy.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gtggrbkjw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gpgphzdsf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gzihprhvr.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gdqhimbfk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gosrzmeys.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gfmokqieg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gztldrrtc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfdrbihvw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gdrpbdtbr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gnewbyunk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gosugsmub.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gemtonbvr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gdwmmhwmw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gizqmmazx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/geavwjrti.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gyuuthxgp.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gtnexiqdh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gunyghtst.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gchyvwgzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gerbyasgh.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gbofngtzj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbuzheoip.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gmtkmtuxt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/godfydeok.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gthucaayg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gdgigeiml.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/guqrgzfmg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gyiwsustw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gnvquflci.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/ggplcknok.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gfbxsvuxs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gkkzwaatk.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gzncpdbfr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/goxnrfkxc.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/guedrrkmo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/geevhoxzi.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gijqgchfx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gyrnbeuir.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gllnblkxj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gwutarosi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtifjpcpr.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gwdhinnsj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmkpsysef.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gqbkzkvyy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gupuwlmvh.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gceksypmq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/grbkxxfvz.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gfejyybjl.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gqpnipien.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gundhirmw.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gwtxwxpry.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gkknsuiqk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/grcivivfe.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gzhokfoaq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gkzrnviqt.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gehsbucfz.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gzvubicux.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gjljppuhv.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/goacjvdtw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/geanfqmas.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gnyzegisz.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gyzgrtrjf.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gxepxtzxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gopedjfbi.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ggtskthfd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/glsnawqmi.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/grhajreef.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gxpxnxutz.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gzfaityka.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gjavkbjaq.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/ghbrujonj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvusjbijk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gyyokijek.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/glvgtkhgz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gmkdhirpp.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gxcbilkzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/greaxyhgv.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gwughzyiq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gyacssetm.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/guflesicn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gflcslayu.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gzucoigcl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnwrmiegn.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gyfjjvqio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gljttscyt.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gydgmkvxu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkrwqnxov.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ganiluglj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gvpitxibg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gresntakd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpnrbousp.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gaqmprvca.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gpfzzkmfu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gumygprcc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/glttusapy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gagnrmmsh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gdpnxyeye.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gspjgnnms.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gibhixgmd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glknvjxhc.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gdfvbrvkj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gmclwidda.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gdwqaoeak.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gzdzxdtdf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdmmrzjfu.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gqliqcyvw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmnzusyea.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gemofnash.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gvpabkgrw.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/grquwhmct.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/ggmnaahdl.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gnqgmlxwp.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/glpbfauzo.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gpmgiqpnp.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gyggfgryy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gwdixjvzn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gtdotvxsq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gakqdlftb.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gieetxjqo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gpuwvbrrd.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gxqafgxxa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gtukemfce.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gpqyrsioz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gugvsmkii.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gbmtpqlld.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gjsntcgdl.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gxwqcgetn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gehngasid.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gribkfnab.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gbodqghqx.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/ginlrbvnw.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/glexoecxr.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gxnixbtpt.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gteeffnyy.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gnnzvwefh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/glodqzbdp.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gwtdrsreu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/guwsaeqif.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gkyxbvvie.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gydwjzzaa.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gitphzkaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpnowkqbp.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gratbgasi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/griduuvqr.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gceqatxas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gjcjzqikc.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gwennszio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gwiaestrd.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gdljtgyww.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gyyfevosf.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gvxbmzbif.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gkzpjsbev.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gjwssxxtj.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gobccgiqx.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gcnhinugi.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvqykxqrl.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gcwodkftl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/guuayknkg.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/ghsqnqtoy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gfhzswpqm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gsposyyel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/giqgqudqa.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gkrrwgpic.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gtrdyzddx.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gzqbhhcdm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gusvyhrjx.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gryttizmx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gmthwktcd.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gcehomndd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gviqwrylh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gbahwtbjh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gvgqkzppg.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gtvpqdnhc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gckodgwwu.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/ghukenpqy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxvmgptbu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/ghspeyuxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/goyygyaqy.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gnmebcrtd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/glyelqeua.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gwtrdxnvl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gkyctchai.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gisqufyqd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gyonggpoy.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gvjjlixaa.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gwtceqgib.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/giumvuxbq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gctsnsszg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gysuuqjir.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/ggimtgexg.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gvurmdwkk.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gkdwewklp.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gkcedsbuj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/giseiphby.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/ggciidlqa.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gercbggsp.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gjeckznuk.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gwipngdvc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gvolcpvmm.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gjsbcrssa.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/ggsogbbud.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/ghmmaborn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gxelztndn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gtyyzywyu.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/ggrnxnolk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gctnbsnqs.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gzwurfwyx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggklasrft.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/guiayvrds.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gsvlrmmfv.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gbicwlyxe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfylwkftr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gpumibwnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gebjxrapx.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gfxsenzkv.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gniaskzac.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/guqbfbcyn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gvqlpkmvu.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gktpfcopz.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gefbhukme.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gxjjdjalb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gtwfqvdke.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/ghjhnquyk.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gzfquonkf.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gizedfatw.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gjyjerriq.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gkmdfooct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/goobcpeet.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gfjsyfijw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gkqrazqar.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/glnkvkytm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gzgvcgbzd.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/giotxvllb.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/giykrbmnf.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gnccomeru.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/ghuqryrbp.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gacabyldj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gkpjgmekx.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gudzxemde.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gzwpfoevz.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gxxkkjtut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gbnsyofcp.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gsmdnxmrf.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gldabsqih.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gcpensmaw.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/glaszsyuu.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/grnqzqecm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gdyhadlse.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/ggmbbrfve.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gyuidlmvc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gcgqbnshe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gbibxnclq.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gdzpjqmcv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/grftfiuyk.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gzgezfwuo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gbwcnzmhn.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gvxbomxwr.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gqkxrwnqi.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gncnalzlc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gnjlkukdl.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gzzuvqoew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/grmzdmjhe.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gyyagyymt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gpyebgdpe.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/grneoluwg.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/guelqqgga.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gbhrcrbda.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/grcpjkdfq.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/ggmnpgkes.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gkirnoepo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gwdjspfpt.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gstbzbqof.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbcrxtdvh.sHtML


<!-- 参考信息 -->