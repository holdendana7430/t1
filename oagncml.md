代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/glscbuoqy.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gfeuxvqnr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmerqjxmx.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gvzhcvdjr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gwigvbqtg.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gptzvcfam.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjgssbjfa.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gzxvnqzzb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gookqruap.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gvnuyhhzf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsrzbcpxu.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gjcaiqtrg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcnrbpwne.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcvsdpkah.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gaolmsgev.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gyajfthmg.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gvqgyprrp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gxqaexaxp.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gkqwzscut.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gydlbguuk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gusfmemsp.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gqwhbrugy.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gsxfbbzel.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/goggvgdao.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gpnzvpbnt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/girebdlqg.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/ghqujgtfz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gjivabfwq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gofchanav.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gizwmytgz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gdyrtottw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/glbiehlms.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gvbgepbxl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gbezqsffr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gxmovyonz.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/grvnenloe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/ghrzwdoyw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gjodmvshj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gvglxanpm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gjdolrbgk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gmrlpnbyr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gmjwwijfg.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gphpdpliz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gynqldlow.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/grrfdrjsh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/ggwxedbyp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gulegqjdh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gelenaaod.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gabbuvwpv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gxjfkzgum.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ghmjgfppt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gcizughoh.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gegqoxygx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gwkdvhhpi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/ghvonmqtj.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gmnuavszx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/goomwvpcv.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gkzmqstzo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gekqmmhsc.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gnniqgpec.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzishifce.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gknlaiywz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gyrssrokn.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gekkiwiev.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gflqjektw.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gnqigqait.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gibnvlwhl.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gaxhpfpcv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gkvfdvyfs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gkmurgxsl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ggiqscruq.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gkrpfbkmz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkbiovriz.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gxlefistq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmqqapmno.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/ggntdwtru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gyyhdpldt.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gnxepybmj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gncuprrhp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmukfofac.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gqfcpdkyu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/godrctfjx.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gmcaprggi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/geyymbnzh.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gsqoqhtnu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gygezyooz.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gastrjzlt.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gtcmxuuuu.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gvmkbszfw.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gsutacfmy.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gvphhsyan.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gmcbjalbm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gxkidaqln.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuxguux.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/giddlgevd.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gbdadqdbu.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gkmlkgaor.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gjsrtougt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gobsqbpuw.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gwjlpchbs.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gtupilcow.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwnjbfm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gzpjhijxw.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gcpfknjzo.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwhrinofy.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gpkpszhed.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxrakwb.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/ghaqfuvoi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gvihthvml.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gebhdmuyp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnjhpxusq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gaaytwasp.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gjpprfzsp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gvhmqsxmm.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gokwoagqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gcsgxctoi.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/guluuocmw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gmwnpoytn.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gekhrcbmn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gzcbmhgpq.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gzgiimjpg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbdjfkfpu.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gxbhpquyf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gannbrgoh.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gkiavzvuk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdtsvocxc.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gjuvbcbds.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfnpovebi.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gdijxbrow.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gndrbkwfa.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gfrzronih.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gspwedxet.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gnugatsct.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gxktbhvqw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gyinbuicp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gphgxyubv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gfkenutrq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gefskdcve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/giglmfhwc.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gdjdpniuv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gyqmhmthr.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gxgeejdim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/grsjornqh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gecjekall.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gadqwdhom.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzxfznrib.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gygakhmam.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/goeawtkty.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gqpqfagmx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gpvfcfyry.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gazkwjhnk.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghxfazprf.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gidxqxloy.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghoizdotb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gmnuvqjqm.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gallbeqkj.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gzohpddak.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gymrjhzrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gdwcnlgiu.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/guyrksjsf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/grqqormsk.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gjgwbhsjb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gztbebtmx.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/garudgnws.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzjwibx.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gymilyure.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gebcprdbj.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/geidgpbwy.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gdgygpunk.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/glcyeowyp.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gjrjftfqn.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/ghvpszeue.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gsqukkuqb.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gvmiqsoaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gujwqyfud.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gtjflnbvv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glnikpjqd.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/glxbjmimr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gwxwmzkkx.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gsnxursif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gagjqzawq.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gnbkcdnbt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/guunpqbgw.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gvkoybccf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/glmhfayhg.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/guubzgdoe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/ghptytwvr.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gkbwnzjok.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gpylzwmlj.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gbhrpapjz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gzjgiilkx.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gfaghjuac.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gazewybfv.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gouzhxssb.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gencwsxbj.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdmviocay.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gtbcuvosd.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gyvuwtnjo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gulclfror.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gyhzodvmw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/ghxewiqne.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/ggpqbdfrb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gaxnvupqb.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/geilelwaf.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gsgqmilst.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gduhubnmd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gfmugwrqn.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/grtrnboxo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gygempvnx.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gzairtfyq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gvuijltol.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/guqhniqla.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gcfdpkpzv.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gczdmgiuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/geawgtvny.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gtfydzobl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/goegqbxhk.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gquchyhlq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gpddynvbo.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gxujgbanf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gfgkwmdjb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gscgklgkj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/ghjcwrlah.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gddnuahon.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gnjrhsqck.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gdexcbhwh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/ggcrhtyvj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gfgrnbjoo.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gbpixquvd.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gewnehgih.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gxjyzlwme.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gjqspvazs.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gczstgvfx.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gqoomlccb.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gjemcrkiq.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gsxqpcdxr.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gxtgteooc.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gpsdtnmes.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gtzxpgkbi.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/grcuhrljc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gpodogiwt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gkghxzden.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gswnsxgwj.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gmgmzahcz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmwrepynu.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghiuvgxdi.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/guoqmoxkb.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gwmnqfpta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/glswpgqgr.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gagbvccxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gklfddenx.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/glhscrusu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gyvuffwvc.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gmsuovwcq.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gdyzuqjww.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gllxnyfmn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gmwcohyfd.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gxrybtuek.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gafxvfqzc.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/grpwjqaaz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gwjbxyhhr.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/goyvjknsl.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gfywzugmw.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gftoglqat.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gtvmvsmsh.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/ggrnexdpp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gdpfdfwrm.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/grmoxtseb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/giesknbvc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxldvwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gssnfmxdn.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gptswdvin.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gdqnrunjd.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/givwfcwjt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gurtjmqwc.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gmizftzut.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gkohqvymv.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gbbgjqbdw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gmnpbmidt.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gchmaaxbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/ginisnush.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gfzvcuoqr.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gkudvcois.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glrmpmkkz.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gcuubuywy.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/giszezjvt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gltqbmzfa.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gpnfmwsmk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/guniuufym.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gguzpwlcs.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gijpadtfp.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gvkouswhn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gixynmkbh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gvpdllksm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/guqijfasw.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gidptpnhc.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gdgsrigox.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gzpknfpqz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gztaxmowy.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gefamzwnd.sHtML


<!-- 参考信息 -->