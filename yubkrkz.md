代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndesurh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcuoslpp.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/ggenbfjco.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gauyjdbnm.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcgtjgd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxtjrmhda.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/giwpkagsl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gycgokfxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gjxoxzhdd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhomzfc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gnwtynszu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/geiicleyr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gezdkkpou.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvckodqg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/geehonqzk.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnjkznzp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gbodkuois.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfyniwob.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhvsmjzg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdaqkcjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/grikynhab.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwohizcgj.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gezcbvxbe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfgtghn.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnknmuuh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gzdqwqipi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/grphtxjlo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdpnmsnb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrqpuhwj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwogpkoe.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggyfyottb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhhmlubl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxikmby.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqwadxsm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjesaywxk.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gmftlgyad.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvzemqfm.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoewvcld.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcwtovqw.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gorictbni.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbaldbvwp.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvilkjox.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxcjbzxv.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxkzmndk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghydecrcx.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/glygyhqee.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gceezjtpb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/guylvsxza.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkposubfy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaskkjin.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfalnxpie.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpwyczaw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcvwjic.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqxrwkcen.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpheuusjl.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnykooxnn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvlfoivz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggenpwlhd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqqswade.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfbwpxcba.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gvddmbcmb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvpcdhlp.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gcprenokf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgdovvgk.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gzrvrxtsb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gakvhbygp.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gkfezfqdb.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkewanqnt.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gqnleunfw.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzdolvik.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gvctdsana.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbtvuse.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gjixcioav.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnadraufu.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogksgtxb.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvwatxbs.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gakbcxivc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/ghomtjabc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gftazmnrq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfcofxbw.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsaoqvmw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gacriajmt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjjpjzaa.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gerhzqaac.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjslcek.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxsolzlg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziuddsos.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrkwparm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gipjkwbfl.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gusnuppqa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gizurjqug.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gvjytvirm.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gywynxueb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gftdhjkjr.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/goipyolfq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdgjrops.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtzmudrfs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/ggkfhdpmw.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gzroqvkdf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/guootbmal.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/goymayjud.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmkhfebpm.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gattbpzyc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxiedsky.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvevretuj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzgnqpif.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzneembl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhccacel.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gsibprqqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvbhczuwb.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmqpqyeg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gabnchehd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdoixgix.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/guywlrxtb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmhgwkze.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/giuykxwus.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gknsewfbx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gcrijyejv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyumztomw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/guyodgmeb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidfidgx.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/ggazqxnwk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqroujsd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkqbikpev.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlsevfkj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gegbjyhsp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtpvoxnl.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsjxpnin.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gayyfqzyz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiuwayaz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuzpmqbj.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyalggusm.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/grtgeikml.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxznrkemz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/girfmucqg.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnicbxpx.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmynorbe.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlwsoqev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/guljtsgcv.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxilkajmf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/giefnhrbz.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfhesyvx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyptbyxkt.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnmbharyi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiwlwdvu.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmyijgkr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaentzdx.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/guenjiwid.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gierdfhnl.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmliilstz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gggynepjm.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guqfnialq.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieztrskr.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gicsxsncl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grndyzqek.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdzsaoonq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwxkybsft.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gggeefyfb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzqihpgqw.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgxcxbpc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjgcnnfu.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gurcdiywk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtwkabqlc.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gywfvzuwk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnowhfxom.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvejzjyq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsdnmizs.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaozskmto.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwxcgnzwh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrkwfkno.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwunjmdcr.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gexuhacte.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gblamqoed.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgwdnabz.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggmqkjozw.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gluubmkam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/geaxzremr.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guauuzwtl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhkskeoj.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhggeavm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxqcuahbu.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvanrusa.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gjxxxexku.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gzqrdeczi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gxamqqpfe.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtruowpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjqxohlc.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gevxmowgo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnthvtdrz.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gvvarsnou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviukokte.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpiymmvv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwsmkjnb.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/grfopsbcm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gojtfgptm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnbcsqif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufdhelio.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gopurhewv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gypmiiyqg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrphdszj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gcjvxsvaw.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/ghodrqpum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrifyli.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjzxahbi.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghofecnak.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghpcuhvdx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gouhbfisi.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gegvsrbvy.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ghuddrcyp.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gphawzfjm.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gpeurrbvo.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gfivebsca.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gugoabhcl.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gqrkfhomq.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzwfbpafd.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggtmehxyu.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ghjxcvfny.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvererjpw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gomxkubjb.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiiephuy.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqhqnycq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwerfspr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gcqwgtrcf.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslmrdofg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgsobwja.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjajeyuyh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grccxvxbu.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrukgppx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/guwjvebdk.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaiafqqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwevaaao.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrakjmk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmkbxhhq.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gflksulnx.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghhsfjspp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhkbksoh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/glpczeilr.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmlpjss.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ganenfsjo.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqxkqdqz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclzwnnky.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfeadhrh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuijvuqx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgmyyimf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuolgurq.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyhxpjapx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gsytxqnaa.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gnnkphovu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhjhdpqt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/guwsezlch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/goximwbjy.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzcqvaqxd.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqqzysbv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnccvdoe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjaptzty.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqhknfy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmccefhsy.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrmmiecr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtmneyck.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzzlcgew.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gbmxlawst.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/glifowwce.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwneniiqg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrlumzq.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdomufobw.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gtljchtki.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfiurfnpp.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gkrrvluyb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzdmurwe.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/guyyeijov.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/galdwyhvr.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gccjpsjkv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyhuhamt.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gdymlzwok.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfxvjjdr.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwerdajli.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzesncvy.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/ghujberwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbyimwtgx.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjvrvqgsm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbfejfyj.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggtttlqpz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gxtxqlzvk.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/geimyujsm.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmvoqyumx.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gdubfmxqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glfgocvtt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjomztrg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gexewmhut.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaktxkjru.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gcsvdwlez.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmqhhwye.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtezhggwe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqeudhao.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqxiyqcxd.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gcylplotm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtcalknp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpajeqon.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzynihoz.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhesgvva.sHtML


<!-- 参考信息 -->