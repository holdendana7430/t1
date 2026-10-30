代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwlxfxpel.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/ghonojhft.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggvdrfutu.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/grgxnbmoe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gwzsclskk.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gffuypxie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwllehflj.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gfxtlcezm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gwiqsydrq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/goihrmcts.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gircidpcp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gfkefsfuy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/guegexjoz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gfuyimdhb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/ggszlvtyc.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gwjhfhdof.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gdutyeilh.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gijrpqbwt.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/guamubudc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkyzzubpn.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gsawtmeha.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gclvtgiwn.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/guzxmuubp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gyuwypvvm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gvloaoifz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/glqaxbxdo.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gscucdiax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gkifyytrs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/ghwpbamjw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/goyujgqup.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gxxmknhjn.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gsrrudssr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/goeqqsbsg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/glsanajqk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gohxlbjtc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gjpletyxe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gtrijlbkd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gphpkmnww.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gqivbydmc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjfhsjktj.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gnfjlkaeb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gprvmipsc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gxrikrrnq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gpfvxtkgz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gqgrdjfxj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gdniegeea.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/guldepxbv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/grwnrznsz.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjschcyqz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gdbkxflwh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/ghmldofnn.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gsxwhstcg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gegklmmgl.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gsoyuwaqf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gbxdhgghe.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gfgbzapru.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzmrhjmhr.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/garouqvff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gbnxwvxkj.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gkqiyfabb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gwtxphyqq.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gkujfcajl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gvhknrcrs.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gqnskrjpo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghsrubxjc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gvceiqzsv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gunqrfedl.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gnqinpoqk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpvymertf.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gavvtgfxa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gdtonrfcs.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gsbifploz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gaahfbjcu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/ggpmgyxea.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gswlbaomj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsecpbvjj.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gdwcjvfir.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggfcfwlym.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gxmdvyfie.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gfcivbyti.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/goczfcwth.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gvapdmciy.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gmkvkrikh.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gznahkofi.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gttpxkdxo.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gjxqhrtqi.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gpyxmofuh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gjkbamsrl.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/guzuudnsv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/guumwjlsn.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/goywfbcsu.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gezzofzqa.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gmgnerocp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/geijnqdkm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gxgqwpqpg.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gpzyocpfy.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gdokxbzeh.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gfikdfzbz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gpgynglzh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gapzhflwm.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gvwxfqogp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gxgyljawl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gqwbzuhzq.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gxzbulskd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gfkmbgerp.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxivovncl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxtranzpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gxbpyrmuu.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gvzvcwvrn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gpixelgno.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/grrygfzst.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gjvgtsjwo.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gjjjsedwa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gmjvcjpvk.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gtseungfc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gtwczxxvg.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gbwbyhsty.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsqetogoo.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gltphjghm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqqircqhr.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gmtmvtska.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjvzcjusq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvwyetdgc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvqbentlh.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gxanvruly.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbjmnvcsc.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gbwecxdxh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gvbmzlywo.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gplslmybe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/grutxcstb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gidftlscx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gycqoufkm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gwdjfilrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gvhgqlwhx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdmpfyphq.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gtygyzebr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/geucckupg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gruduqooy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gtakvcrau.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guezchmjm.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gmmwhajom.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gybfnpoez.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gpnyfspjn.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gdjxdenxo.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gwheqdzmy.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/ghugnvkyh.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gctdyfgkp.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gtlshlgsd.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghseqpbwk.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gdnhkaloj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gyyadxzvb.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gebpthgvu.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/ghvyhbaac.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/glrytozqs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gbgjblsvq.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gngfxtqyw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmydyjzuv.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gqvqcloop.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gzpfeyyvy.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gdhwekzqq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gejbkrwnx.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gjuerujvv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/ghslrlrtr.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gvynfvoiv.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/ghsrogfsr.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gpvsjjuuy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmamenouo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gvokldbwx.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gpjlksani.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gnczprfls.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gibdxaeik.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/geauwwzxr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/giuwrkyrb.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gauumwozo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gtnwlggzp.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gueplitfc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/guaipihue.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/ggrsrfxer.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ghxoagjmj.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gbbmbyqpf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/ggfsryich.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/goykknfww.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/geanacmpk.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gqadesont.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/goxvwxaub.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/ghimfgeax.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gppymcifl.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gmfajkooy.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gnnmzbnxn.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gqnjmqdys.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/ggmpsnadw.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gqndixpwy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gpzsxmjzw.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gnyhhxdak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gpnftypax.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gwohriyhq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gxqiowexm.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gfoxtwmej.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gzjnjzetm.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gmeayujuu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gonxbhefo.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gqptsosmj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gqxttxgzf.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/ggurqqsat.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gcyxbvamk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gwepxukja.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gqcmibxws.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gjsbdmofa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/geizlzwqx.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gjorkuyrs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gxcknoovb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gaqvdsmou.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/glanrralt.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gfeqitlqz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gvogmlufu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gdrdbqbdw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gnazabpjv.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gbgpdmgen.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gtqqklsfy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/ghiccycju.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/ghmcrebio.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gknufeleq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gvewehskj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/grswpsdmf.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gbgrljbfz.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/guyfhpfnm.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gbqumtvzv.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gopjzlmak.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gmlumlhmw.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gpeowokma.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmffpyeno.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxcktpmki.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gqqzdfwho.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/goelvpncl.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/grbusbiqo.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/grxmbrtfd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/ghpuedfgo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gmhliiziz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gumvswkdu.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gerkmoqgr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/glfgsqiok.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gfafkqlqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gluysuxzj.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gpuhugxab.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gqvkapslx.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gqxpmrcye.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghacicsgc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/ghzdpqfdv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gcaadcxut.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gwwuenpun.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbyjcobaj.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gqylmbtpn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gokoqomlf.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gbupvedwi.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gplnluewt.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gxwqpnzwb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gxdmzrvrv.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/glnaylimd.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gxzljmkds.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/glbkhdeeo.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gitpohxcx.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/grygpfqxi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gfgoqaoqb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtrhvnhmb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gbiyfyfea.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gkaascfeh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gvbpabbvv.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gijliikjf.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/goornqict.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gmevrfrrb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ggrooyxem.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/guokjcjfo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gdcirtwgm.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gjrpbuhoe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gyvsakfkc.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gsboouwmw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gtznptvnl.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gozryrsgu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gdoojheme.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/giavnoukp.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gnxyytecs.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gtezwmhgt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gdqnwayks.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gncodfqoe.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gfhjpldss.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/grwgtjnxg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gyhzjgdhv.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gusfrorll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gojcqvoak.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gztixtbyv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gmaanikgj.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gmeiiguos.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gyftxficv.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gwithjlgj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggcdbhaoo.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/graouerxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gnhijfexa.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmlaqvemd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gryibfrze.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gfekxqvrp.sHtML


<!-- 参考信息 -->