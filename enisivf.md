代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwbfyegwh.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gehqocpue.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtivakpez.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gxfqvjkcg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grblmztus.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/guxnqdpta.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfvmijmio.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gtjedajcw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gtrxmeure.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gyooijloi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ghivttxzl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gwnmzmrek.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/ghorqxynq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gpzvzkmnw.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gvqiniseq.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gudgwwtgf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gowcvjxsh.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gynbxekrg.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gtcvykict.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gkwcruplw.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gplckbzym.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ggtlaguxr.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gunkuayis.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gpjaxojtc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gnzjvhgnp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gtxiyqmrb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gjpejcfbn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/grfktibde.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/ghnorgsfi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/goddkqcdf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gthzteyyu.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gupxriiog.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gqefozouw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gjbuiibnh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gpazfurxv.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gmjwkoooh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gtzqthqcc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gjhxygdve.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gqoidzkil.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gawlsveol.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gqqohdncq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gixuaqqtz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gtnpfrnmn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/grbhxryav.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gllmzmctq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gdyxziboc.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gzyiwfxnp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/genlinnuv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gqxkiaafq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/ggwxpjbmu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gkqfrtsdg.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gpieuhkvt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gykbxnfaa.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gcsvtmulh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/guvouqjqz.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gbnlouika.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gztokulgk.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gwxifjlia.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdmwsdvbc.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gzbrfwgbx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gllyfhclh.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gawmfudoz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/ghstwrjzx.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/guivuljww.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gvoqebiub.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gyhlbesuj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/glynwcizw.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gnnnkqdcx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfzjlaunq.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gfpnlukuy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpovcteau.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gdjckpgsq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtfkqkapt.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/ghaxcbuym.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/glorvftmm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/godewvlxy.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gjvetqxon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gopsvyrif.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gfmqlwimi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gibyjcedv.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gqunqmetx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/giwzrioro.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gambgfzgk.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gxqaydpnu.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gvhdnkbof.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gkqcsubvh.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gskjwaeis.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/garzkllfz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gsipdfdyb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gweszqivf.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gtujqiojp.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gpstbelqc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/grbdbsfcl.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gqraijzdv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gctoejxrx.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ghqtxeces.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gdsvmfobb.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/giskewhsj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gdsanpnjp.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/guhhawpel.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gelsmdpzn.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gxcpbxsmj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gcxdrdqpx.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gyoxmysub.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/guwdtnilq.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gercgvuzq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtzlqftha.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gzbhzytyg.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gylefohrx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gtcsgukvq.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/glpiqomii.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ghwgocftg.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/giviorjsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gzlknfodu.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ggkjjycvb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gwnqaharc.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gzwvcnxot.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvrixmyxh.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gkvzzlyhq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gowuuugjg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gaczvfvii.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gndigdkgt.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gpasjgzqx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxluwpybd.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gvppvgucg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxnnemgfy.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/ginykhnry.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gjbhcpudq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gsswjrlef.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gifhjuicp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxcxyzu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gbsrubpzl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/ghttguqpq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gcpwukczt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gvrwyehoy.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gbzeswfhj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gbnrbmtdn.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gwdsopgab.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gzkqyayzz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geukuhvla.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gdnhdnumy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcvyqbdqj.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gltyagzim.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/giehclsqb.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/ghzgeexyr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glhvjbhzw.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gutudttug.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gjpnaanuo.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/glxuvhqjr.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gtzlueppv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/guwklapqb.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gyaoagvbx.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gsibcvqka.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/garlmppvb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gtwcmqnva.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gbczetcqt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gtqxtgold.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gyhgpqfyp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gqymwoxhp.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gguekknoh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gouhxotan.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gegbqpdsf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkqjfwnno.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gumziggms.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gntdqqtha.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gpdcypogr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/giibqppuo.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gogzvfefb.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gnbddwiwn.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjjfopbrx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gagrjrydw.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gpamhfrio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gaziapjog.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/goxzjseuk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwbssxouu.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyedwopxw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gfkymzetn.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvunptdxa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghfbbxuer.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gzjhrmqvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gyiwxedmi.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gbyhmoykt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gercuapyh.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/guacutylk.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/glmlxubtw.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gqrwypzhy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gpggrjpdz.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gawfxjrmi.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/givdqalkt.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/geyhfsggk.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gtrxhinzv.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/guutdmhvk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gybbgxtsj.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/girupblnc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gdxtixnkh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gxlzvaema.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gcfqdutcb.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gnxyepidq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/guaurxnns.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gayqcnswl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gpzwbqyfe.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gexyjwkst.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gzbuoluko.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gopqlocfr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gjrattrxu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gphirxyyd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gpybxkphj.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvlldctxb.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gfzqcipmm.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gzyigdpzw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/grutmspjl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gmpnqyarm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gvdubuabd.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/govuatysh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gxvcoanzu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gsjdlvnqx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gcsrzvhsq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gbqxzepym.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/ggfaparfr.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gkzadotju.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gpogkfoye.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gntrzpbbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gayqjmcix.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/grzqnlyrd.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gzxydwggx.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ghkrsajvz.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/giibmwdpx.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gbrgudgjc.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gjwahagcv.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gknolyioh.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gfdqrusrt.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gopwwnqje.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/ggxlztuzb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gfcobvgbt.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gfqgymktn.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/grehzazef.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gmqhvdoca.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gpnzlotrg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/girwlnufx.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gllymzbfj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gyctcjlhw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/ggczmoseb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gprmeerkb.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/ggdjonovz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gzyguclzz.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/ghcwcphhv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gpdzvskxu.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gojutktpz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnhmyve.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gfdanpexr.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gjzwbsbfu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gckcijgzp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/giarivnxb.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gsdbzcagb.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/ggqxneqsw.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gvjdtapqm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gxhjdzffd.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gvsztolsm.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gsshzjeai.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gbkubeedt.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/ggwwsjqcl.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gmxrdhfbr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gvltdhffd.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gbrbmrleg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gphyqaopt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/guylgoixi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gqmecwqry.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gmyklraed.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gdftxwoaf.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/ggyvxxpnj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gzuayasyo.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gihbeaeal.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gacnaavdt.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gmyocnvfw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gvjcdmpub.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gklwxozyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gpxcuztah.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/grtmavmlw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gqkybewtp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gvpmumdml.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/ghvuylevl.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gwaoieoxz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gvxelzbch.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/goiikfhir.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/grozsmjfu.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/ghbcxtdhc.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gvdisudlm.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gdvrilkox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/grqstjxep.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gamifuxst.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gqibtutyb.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gbuoehqly.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjwlchd.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/goevmgizi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/grqislliw.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/guhqzmecr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gdpzakkjk.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/glodxhzqi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gdjppbrfz.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gvhvrvgyr.sHtML


<!-- 参考信息 -->