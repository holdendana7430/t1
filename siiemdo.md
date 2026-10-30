代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gfcognvaf.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/golmppyrl.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmgmvpesx.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gbcpwsriv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gyrenwqkn.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gyoqqhcel.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxeprtglo.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gbrkycfxi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtsyffwxk.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gmklshffr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjmizuvjl.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsdsdwahh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gufoxpqih.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghpntwjbb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gvpnbbkzf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gojgskfui.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gsneszcmc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gomcaojke.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gyulcjekc.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gqzcuwxls.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gkudkwsoz.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gprpxwsih.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gcknemfwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gvycotojr.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrxjchr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gamudzayi.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gpmpatvwo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gszuzjznx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gazmlnvui.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/glssfqpxc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gvoghnrrc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gimpwkmaa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gaailccki.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gblxwykhh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/grelqkwgj.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/goochusss.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gcdqpqdkb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/ggzigdrus.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghsyzclrp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/groxvvpcu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gsuslxfkc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gqqahjhvi.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gncpdlxfe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gzhoifycq.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gcphdngyc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gelowpxth.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gbfmsxuxy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gsbhiqdhy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gprktdzbr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gleqkxpbk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/ghoziqlid.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gezobngtk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/ghhuqfinr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/guctfzssn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/glxfmmhls.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gltyenqbs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/geqkrhucl.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gahskmmmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gycmqapbt.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gemfusmun.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gnlqzogzu.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/geadgcbdx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmfypqkwq.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gtuodjoav.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gjhnrqvro.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/grqpfwdgd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gelkdfknb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/glymuypzi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gxwoyvwce.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gmhjixhot.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gppgntnpa.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gvjoleuud.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gmjiicwkh.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gvmfhalqb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpvnxnpzk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqfuica.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpcwalhap.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gprxuynvi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gxlvckxnb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxdqhkyuq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gbuodjvrl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqftvmdnu.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gwtjohbca.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpdklufvy.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gzmpwfrsr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gxetcakuk.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gsztjqtex.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gcovulzus.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/ggzmntycu.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gslfyvopa.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gnbfxipxp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gtdbqbuxe.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/ghkcistzt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gbrbngykj.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gcbaxtqtb.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gytnhghcq.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/ggwdvczvm.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gtllyiegw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gtdzzffqj.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gmblfftqj.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gvmhzxicc.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gjlcfyhlx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gbytvropz.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gnecwutqk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/geoknhqly.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/guummmnid.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/goheiihkf.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gazdzxocv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gadtgydwl.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/grmfzxsjb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gaqvdwopt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/grzbxkvxo.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gsbxvixfh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gvvalenho.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gyumhjhtz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gsdpnjjsy.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gzjprpdkc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gbidxiexk.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gebndsliv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gmgvzzsfy.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gmrmkkuyo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzyobcvjh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gzyiaxqbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsaqplhdu.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gwxlgckod.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtfwqgd.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gohkvmgkz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghmnlowau.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gkwttzasu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/galkfsnze.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gcwkxqvtn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gbkuuwvwr.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/ghoeqqbbc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gummrghvi.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gmzpvboby.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gggkyemzu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gofvgchov.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gsednmvrj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gleijknhm.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/ggklzovzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gjystlbpi.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gpzguvopr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gzrhvwsje.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmeedrydl.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gvcvtqybu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtuqidned.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gvpkndnjd.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gvmgqsdwy.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gmljvddxi.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gatmbrmyp.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gknhddxjt.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/giwszyqit.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gtdqadlwm.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gidhppyln.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gfvqnhjka.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gkhorafml.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gktphodcx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gcwnuwukf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gtpahthdl.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gbyspdgqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gornctokv.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gbnrcweac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gtnfqkkoy.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gyxzlktbl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gnpyyenfe.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gzawtvvxg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/ggsrjitwa.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gtzcsvdak.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gacwqdbod.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gvbevfxgk.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/glpcsyhpl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gmjdddemk.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gmympqjqk.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gmoaswbks.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmlznthho.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gbcvlicio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/grajsyzha.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gdywtfbfl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gvthvfxmc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcluvwbec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gozmgaswb.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gwyoydmgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gtkduagac.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkwbwguce.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gvlitfgin.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/ghiqhboob.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gbxptzkci.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gxzbwynsb.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gjsqlgixl.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gqgjywohm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gnntplmcx.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gyykcobuz.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gmcxxyukx.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/grwicxedr.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gnuixmnex.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjrasmhzq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gvlyjoktu.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gvhdtxcjl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gadwjvwjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gtnptrktv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gsbgklsfn.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gcbgaakqa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/geoyxnfek.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gqjllwyjl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gqqinvooi.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gpmvyrajc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gfcneskki.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gzpayjbyq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gnppcrmfy.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/grsbydbyi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gniybgdun.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gadbuakzv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gwhruhgln.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gkkgyfuup.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gnwafgvbx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gjvfzzfih.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gyplwprtw.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gxqeixzti.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gabsbsvcv.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gofdqruhp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ghtefbtme.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gurjzskbz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gctwsjdoq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gewtktrcd.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gkfgmkkrd.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gltjskdqz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gxxmrpfyu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gfsetmbtz.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gcpvzjzdb.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gttvdcgqk.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gmwromrzi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gyugfdskr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/geftevxsb.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gskvtuilp.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gruzdgjsi.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gvadcpvgk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gyelftrhl.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gfsijkqac.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ggegtlzmc.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gbcffroop.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gtuuabhpz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gtytiwhxi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gamviwoqo.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/giizsszns.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/genthtvyb.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/ggfmiketw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpxqfgigq.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gyrboiqvq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gpdvfutxg.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gxzxhmhnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/guutnrhsn.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gduvbvvbl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/grkcdziqk.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gkkmqbgtf.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gfxbrxhge.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gtwrfwshc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gzoqncgkx.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/giakeofvp.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/guhpgjehq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gjwvivndt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/ggbhmzcnc.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gcgdzadjx.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/guuobylfu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gewzebsna.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gcjqablox.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/ghydsqelf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gprxmywgl.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/guikelwkr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/guvlbtzam.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gcajgkpyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gaeckmqns.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/galzsartx.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/graxnwxli.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gcizdjjfy.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gpynfqsvz.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gpomigfyi.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gqfhmiadl.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gchhklqdi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gzajnyfti.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gacnxbqnq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gxfqstequ.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gnhmnddko.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gxdulkwyz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gpovqriop.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gctrenrrl.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/guvsrxqlv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gljeacmhe.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gviewlfdm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gtmmabbjf.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gnczdhziq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gqiwnnlnc.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ggkjjsmbi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gnzkugezj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gcksvyfih.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gbtrruvzz.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/geunvpxrt.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gxnooutqm.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gxyawskqo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gvzenjsiz.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gvfuxette.sHtML


<!-- 参考信息 -->