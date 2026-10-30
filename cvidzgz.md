代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gdfaiazkc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gancrogrs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gkauvbhpe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/grfisubmg.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ggduxtlem.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gmhsmmbfw.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gzcunrcao.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gwuftqqqw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gpzicolcx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdpboehag.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gzrmdlnza.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbtrpqdnq.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gfbkxemjv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gkqbzklvi.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/geyvfmlke.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gkygiszee.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gxwwxpowl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gjgfmwmaf.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gbsqgbzxm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gaskqyalj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gjotbswqz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/geztmxozz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gjmzcvafw.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gipajhzgh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gyewnghrc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/grchmwwnu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/grkyelpjq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gouuoavmz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gkznxnkan.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gosgggnpm.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ghrwatieo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/guaekxzvm.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gnupdljfx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gxaxemxnc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gvdybpqhj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gvqvqoifw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gacopaxok.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gibfsgcbh.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gmtvmvnef.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gsnmfisna.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gdtxofbix.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gtpegdufh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gcewtjjgr.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/goezafgtg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gaqayqvfx.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gndlonjiv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gtazwcqip.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gjcqsmgsx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkonfdsrn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gptulylxm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkdyygplg.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/ggiltqzou.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gcafnlsnp.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gzuebakjh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/ghjdpvhdx.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gspvprhzd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gieuvwosq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gtrxciosp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/galpedywc.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gofgwysni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghcuuheuw.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/grzwxxhvp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpiwwudor.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gipvsgplr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzydrypj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/galmuqzpm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gywblphlm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzvbvgehb.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gyvpjdbkn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/giqhafdgu.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gtbqifykh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjjseyptu.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gkrgghkow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gewfvuvhz.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gytypkqkt.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gmtcfnhhz.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gqnyxombf.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gertmbjek.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gttleeftz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gyajetdlm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gsajnuwjc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gcxfnfoel.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gvebvmjjz.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/ganyxgnvj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gvnxikedx.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gdapxyqod.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gralmzelz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gvrojenjx.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gwozouogu.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gksptylfa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/giwpdwgix.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gsxmqpbbq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gahytsuqx.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gmgajskqn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gnupaplpf.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gasjglecs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gtzobgqer.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gtcdmywno.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvhkixvyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/grwrzzwwp.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gwahzxfwq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gkwqrxdfp.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/glcvisnuj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gtkugcwap.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gfdsxpnyt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gjzxiowqf.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gqgxhzzhd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gmbyiboun.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gbwqkddqo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gheyeuovd.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/geuclywlh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gwapkfdvn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gwfljuztv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gartvlmtw.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gzxsessrx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/guyecqvei.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ggdirmwir.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnbiokuxb.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gpmxysigz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gmzxvhqft.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gpildntcd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gikvxmfrn.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gwewodyhr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gbkgbeqdq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gtziptkyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gnpqhcafo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gwnfvqaoe.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjjuihrwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/glouawgbm.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gmylduxqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gnqfixzbn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvnozazwz.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/grffuvbam.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbvpoekca.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gnerwaiva.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gfvajvhxg.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gqankperm.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/guvfrnmqv.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gebhrduco.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gchnkrzqv.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gsquwuyqi.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/guyuiqguj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gwrwvxgdh.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gcvbglaoc.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gyfwtjibp.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gduwtqzvs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcrhxdwpj.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gcbsaubkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gtgqdsfmb.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbjzugleu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gchofvtey.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ggzhkseoc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gfjozmsss.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gzabqxqzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gctpjsvqq.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gadlucuge.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gkkwptraa.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gxhkksbtt.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gzcoxinrk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gbustwcgx.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gzrpmqbrq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjckzygfx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/guneudaio.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/grkgwovpg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gmaaqpdoc.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gubuiuxtf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtmfmntaj.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmeacahsv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdgasebfy.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gezfenpxj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gozlmexej.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/glrhlvhtn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gdvqvtfbd.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gkkdkjlhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gdbkjelwa.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfakkzvuc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gstxhugib.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gudjwlfuq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/giixydfrr.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gvthgzhqy.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gzrrbpxdr.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gbbvuipwd.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gadmiexwy.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/guyswvgnk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gudlhnwig.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gjepievfx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gvuketxdx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gagdvkqhe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gjpqhewnn.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gazscqwcg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/ghhhemuqw.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gccmswlgl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggphjrqjp.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gemjfjlgw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gmzcvxiek.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gaayegiee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gdpmmwdun.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gvhluhmaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/ggnqjwutf.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gpcdkczlt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/ggntzqdak.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gcannneol.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gfwadduqz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/giukzzpfh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/guoqziqtq.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gnarzyyrm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gwuxnkoxz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gplwhmlas.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gvamghigx.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gonzdgmfn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gzknmdmxb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gqlyuytan.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gaemmpqyf.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gmjcymnkm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gdvryroee.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gwrtsajma.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/grpjwdooi.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ghwevyofs.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/ggdbjfrtd.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gupajtlzn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gcdrvsyqk.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gwxntkojl.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gcilktsxu.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gnosaatke.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gjsepozks.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gjhfdahak.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gczzuzpzi.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/glinpmqnk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gggudlkvt.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gbnuiadfm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gfrpejhwz.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/glmwglcjo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbkkqsplu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gciwflgak.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwauintde.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gilcbmiup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gflmxmzvg.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gufbhujua.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gaqjzunlc.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gpunslohr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gihjeusei.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gdkeotmec.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gdmetifur.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ghzrfixdy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gnzdnyhre.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/ghesbiobs.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gfehmqjxw.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gwpxrnhwx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gjjmoexgb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gfblphbey.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gruydlqsb.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/grzlgsprn.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gywmtacwb.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gaikggdhf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gsejcbujd.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/goobgfjcr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gxyfdpihu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gesdgmawm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/govpwsije.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gjjuernkc.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gnozeclen.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/goqwtnwms.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gtuzvqexi.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gyjlobgka.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gjgnazqse.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gexghxrwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/guuvturvy.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gkojnvivu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/ggkgseota.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gigegftae.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gfdllcfnx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gcrffssuo.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gkzjjzqqb.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/ggmiedjsp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gumtliplz.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gbldjijer.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gvtnzyqky.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gjyorjzhs.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gjjijukws.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gikoyreqg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gganlsycz.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gopqnuzis.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gfjowolye.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/giyenjiac.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gobduinsn.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ghbmtvdtk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/ghotopopo.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gbittxzkw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gfbpzuekb.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gqtktbocs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gaxpwcpyu.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gbymzjtqt.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmamqie.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gbkaqyepq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwdubrsjg.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/guxmkdbkq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gmiehdhvx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/ggpgulnnf.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gztsolcjh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbietovkw.sHtML


<!-- 参考信息 -->