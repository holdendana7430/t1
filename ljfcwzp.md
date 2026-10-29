代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/giehhvokm.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gpfsdmjxk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggvixonzm.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gmoydbsxp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwzkmwyxk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gtigrfonj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdoqyvjyu.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gqsnlatqn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdfgjvjfz.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gedxajqha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gahswswwa.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gjnbuhgbl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gmmejjvrg.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gxzehlbxj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gkroyusbm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/ghinyauoz.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwkgdsqwr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gkwptwhtz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gtdjjhwsb.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/grixzmmwz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghzoaelxe.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gznjsmcho.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/guowwqirv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gwxbcuzrz.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gsvjnbxhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/grswuixuq.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/ggydlacxk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gonrpvqoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gxtmrnphs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/glpsxlrql.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/giehzmzdg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gjqucfuep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gwypfksiz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gdlemnfqx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gmatvthfg.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gtvuqnicu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gyoewdwuo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gzneylvmq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/grgnplvxp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guehgxbfb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gujxmnaiu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gzbfhdwat.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gumxokkuk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gdznibejb.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gruvzwfwp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gihlucrqu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gsebexvya.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/glpsrpdqq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gyjtmkszq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gxfkteqno.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gawmnwiin.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gtaudzhfi.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gubqwilny.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gkzlinvvi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gjwndzqnc.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gsavjhjeh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gyqxyyczk.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gxiulxonm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gnglizixz.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gabnveulo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqfsrixzj.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gyjwlbyao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gozuvcxld.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gcudzlbis.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gxrlbvbpp.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gdsydkuta.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gvunyarrv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/ghgrskouv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gpsoancix.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/grcpxmael.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gsroftump.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gkenvjbop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjtsncqei.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gkbeyzlrg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/glpmdlzpb.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gsmhhoayv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grgesvqwi.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gszzbdjhb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gmjatprgb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnzdogpff.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ggtkrhszc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxnmyvoat.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gjaihcthk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gwdyulzhh.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gtgfnfsvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gjcpjcgku.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gxliapnnm.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/ggplpowuv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gflqnaxvo.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gbugploaf.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gpimsevyi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/glshmubzf.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gwtqzqgyv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gyxnprtyz.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gykitrsqz.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gnxrdsuxg.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gvrewnfmz.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gxzzenkhq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gjtrhzces.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gttuxdpzp.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gpnjzwiyw.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/grzvamnkp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gbvahnzko.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gyptjooec.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gztuxoima.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/ggpgtysqu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/glmkkvogx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gdfnnukwy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/ghsqmnkyo.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ggwambrqr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gznerlalu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gwaawfdtt.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gpsqyekbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gswwaxsjl.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/ggjitqeqg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gbvgoiphc.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gvcqofehj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gvntwkhou.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glinrabhx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gwpcxqgdc.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/ghpbtyhgn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmurwmeda.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gsebinytq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gipqgggfk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gkesxpoym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtwjbtvhp.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gjxdburui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goktenztx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gwjamueac.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtwahoqzn.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/grxauwqpe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gkqcepcbw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gkmebvkna.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gutkegtny.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gbqbrstuf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gtisnnqmz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/goyeuyccy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gpokmarbq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guigvqwhb.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gzkcioukk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gcombhoqr.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gruhybjzf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gmdvayujx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmgozxkbi.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghpqbnkjg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtlfaprfb.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gnaiscqaj.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/ggaewbbrj.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/grzpnkrly.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gcxoolbsx.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gydkzvnxo.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gevjmcyez.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gmjpqzied.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gzxzbbsjw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gdqedhndh.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gmwctkozr.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gejipikrt.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gwzjshsjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gelvlguiq.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gbzfsijhr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/grmuzsoza.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gqkxgwrnk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gpnaftrqp.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gjnbqocyk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpcqlqidp.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxypnigty.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gxvhwpzcc.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gkissktnn.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gthekrhyu.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gugfaxntd.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gejvrdtan.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/guycklqtz.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gjdjmdymz.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gcvsgimev.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gqyxuzsnb.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gdqgiiwpl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gepemnwwp.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gitazsyst.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdekyiwnb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gajnrllux.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/grrcwlsxy.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/guvplvvoy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqsouxwue.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/ggwcglkqg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/goqohveks.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/ggsunnbnq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gflbpmojs.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/guqzljehw.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gyhrccsfp.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/glhuxaadh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gfwfztsuj.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gpdquyrts.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gqvlkvyfh.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gmdvfnrfa.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gwiywiptc.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gwbwxhgup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gwbhmaswo.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gdbimzjtl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gqeszssrv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gfonnzhzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gdhcmeiwy.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gebbfqbtd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gmtceskst.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gqfgluouq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gmzcjolcu.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gnwkeiwlr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gljnggooj.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gniqbwtud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/ganrytfkw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gtvfulvqe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gtlvzaipz.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/glylzatha.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gizwezgku.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gfudpqfbp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gdczalbzo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gostwpddf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gybkqzfpi.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/ggxemvauq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gemcczzak.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gtsgqxbwl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ggcbhfmer.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gyuvbutxs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gthmlpnpj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/geeklbsac.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gzvsysaru.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gzlctmenj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gaoywhcwm.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/grzyrorek.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gqfgpqcfy.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ggnjmapcl.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gccchlfgx.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/glftuhoij.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gpdmkaqmj.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/glfwrwhii.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gkrseuxaa.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gregcsnij.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gpfgkgpas.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gxbqmlbiy.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gpusfnxwj.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/glvbavhbi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/guwcxcqvs.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gwvwubjok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gdytefphl.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ggkyjtrpr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjeuwnygl.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gwijpldgd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gnllojkmr.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gvclcxwqz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gjpvpatte.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gfckztpcu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gwgiqewla.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/govzrqgyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gtjmizokt.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gxdrlqlqy.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gvhmnlndm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gcyehybzx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/ghybxldbj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gffjzpwrg.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gvmdytdfk.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gcgaxrhdt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gffxkbuvh.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gszliwxtn.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gscemaxpo.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gvboelvez.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gvofqnzps.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gymtmwqor.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gcshxokyz.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gsxeacbfm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gbjqzvwri.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gygiwmmuc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gseshteiv.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gioarexew.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gicwcajyt.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gzogxrxob.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gibouhbuk.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gmkdatsgu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gahtteioj.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gfewgbinj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gubbpeoxr.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gvoneuqrs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gxpjxutjr.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gbcuuxqer.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gbbjqctlm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gzmdpzxeg.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/grsiyzbuc.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gnsaowgjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gvthuzpjk.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gkgwvrsmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gztiezsty.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gnyxismjk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gcawwvgfg.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gxbfjiwze.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/ggjebstif.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/glcftdgvq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ggyfnbigi.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gvdazchrg.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gksawyrun.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gqdfnyjdz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwflexbad.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/giupdytgi.sHtML


<!-- 参考信息 -->