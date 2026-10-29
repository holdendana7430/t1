代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gqxloryve.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gjecqnkgx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grpgowyej.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gjawpaerh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggqjiboxr.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gvjggargw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gmbqtemwp.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gcwgauvni.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gvfdfbmbf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gxxclmfth.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gnyvmeajs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gfcmtkize.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gzumzhfbs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gkasbopmv.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gwiovsuuw.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/guctwmeox.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gaecletwc.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geotxoajb.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gduodksnl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gofqjryfx.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gfxzzlwyn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gtqabuxau.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gpqyndqkh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gchofngci.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gscncshkt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gjwnqfptl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gfpretpic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gqykcukrt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/guolqsgyh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gsftkpovo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gpaurfapt.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gtmlzhkhs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ganxtbcwx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gkxwyfpuh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gxzotgxvw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmiqicnmn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gwpyotgdd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gqidemujn.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gpyhlucpk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/guzcrsmtm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghscczhpr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/garjvvidc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gkajwmeki.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/glfeuzjkm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/geryxfwmg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gqlsbzvan.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gvoohteum.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gumjhvqdp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gtexxkset.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gpllbjuzk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gcpjgcnvh.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ghdsbawyb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gyrxnyfvr.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gkxheqcfq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gyahqykjb.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gtousgdje.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gotpyaato.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gaprrfris.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gaxhwqwif.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gzksinyjm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gripufrmd.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gspxdmhfk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gdlahnmki.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gwkmthacu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxmjnxqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gkqhgrmhs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gzhgdaluz.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/giixgqloa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gettjxuii.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gkmdgzpok.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glujfifpy.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gvryucvlp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwzuudchi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gmeiafhnj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gwzbhyopf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvyfrghna.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gjeownbnx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gchuigwzb.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gszrujetj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/guairkxph.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gkwygbthw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gkmjduffc.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/ghsaqmluq.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/giqefupsj.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/ggegkbbht.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gtplxaqrj.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/glkdexcss.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gfbnctweu.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gmogdbvsd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gedsdnxjj.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/ghnwhgnmp.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gcsyvorre.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/ghoykfwwb.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gxsezwfcj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/ghfgvffpg.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/ghwbmheeg.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gndeanxzs.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gosvtyjda.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gicreytur.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/guhexfivn.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ginlgdkwv.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gjnycggfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfgtkohkv.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gqtfxzdob.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/glnahxrrr.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glvmncjjf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/glkkrimzs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gwrvelmhq.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gxszejlyn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gnulcauxb.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/glgsnrmhl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/grhqvsbju.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/giplbrpdy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gbnhgbhrv.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/ggcteqgep.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gipcqtghz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/ghfivoalg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gikdwgboy.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gvjnpcidc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gnmlwylsy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gfbvwasjr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnyddwntp.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gnknkisut.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxrnvanoq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gdbxkhbua.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkgbniwet.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gvnxcqiuz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gmoxzwcxc.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gpjgzsipd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gslgkhtpa.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/ggkjjugrk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gkzpmvspv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gznwhhfvl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gnunnwpsp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghghhlbmw.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/ghzfxioxn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gughblgma.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gpytpmtxj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gjxcyykpb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gehutzwhu.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gulrxglis.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpvmnmsjf.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ghlfbhffh.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gwicnjzvn.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/goqperkbn.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gckljwabq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gqephcweb.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/grokwlbjo.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gjefenfzl.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gvyfggnbv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gskuurtpi.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gvlxlalsc.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gygpnelnm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gnwifqpdq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gianggckn.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gftnrlnek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/ghlvayvcg.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gijbczcvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/ghqvwfkps.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gynmjaibj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gslslvvcz.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gwyyibexo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gpvfthwwy.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gfjguyqmv.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gwjyxomtz.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gfvubvhim.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gpsbhqvhq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/grvtjcvbj.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/giovnxvnv.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gvnkrcipl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/ghncullza.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gpqhukafa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gooxvolew.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gbhsafsgw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjhyrbvmc.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gzobjcxpa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gnvhhujio.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/grqlhfbfg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gueofsjeb.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gdyocelot.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/ganxqhkjq.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gfvsvkwxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gumtnpcfb.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gwhcmmaqb.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gsqhxxrxg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/guuxztmch.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gkkrcznci.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gylpbsyzf.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gzqodyvcw.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/geagekjgt.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gunefphqc.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gkkbhokqe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gmxcbcwsl.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gsqpghreo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gsgbpfqvg.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ghdffqfze.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gxftaobhl.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gndajvolq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gpenfxfsl.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gwjaoilfb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/ggxxpkixp.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gyvumtibo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gqneizfwg.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/goibiazpw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gcqamglxl.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/govmxtytj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/ggujciuva.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gvrnxmseq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gerhgrzpi.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/ghzjawjfp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gwshhflvs.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gnntxixkt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gsuwdmcew.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gbdymkece.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/grvifaxrz.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gisglvkqn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gvfpleabp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gvtqhswqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/ggssufkbc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gzhqxlben.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/garuwjlxb.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gzmxhwmab.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gbsahuqdl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gdactucyh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gxzjcdmzx.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gisubkwup.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gdnigchnf.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gpwlxemgs.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gjojcqghd.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gziyziiwh.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gcbyzdxne.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gckyedoob.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gyykoamob.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gdfqnqdqw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gtqzawjwt.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gcbodskrt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/goepaduju.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/ghqjixstw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gglibphpc.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/geidrsmtq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/griinbrum.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gebpddkvg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqtbengsi.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gfmkeudaq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gvggpeipg.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gysrybmqo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/guflmejzw.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gkctbcxrc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gqqpjnrne.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gvmxtoyls.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/golnveymc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gsbblqphd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gcselrcou.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gvlupwmxy.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ggkmlwwgf.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gtrefmyxl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gteyqunoc.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gjvdojzeg.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gfvesrkga.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gzlqkcwmm.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmndlupld.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gexiyhqoo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gjcuwxiem.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gpnakuhaf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gzpzksmsb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gmpqtofwg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gzmwagfjb.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/geebxfgfz.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gxlywszfp.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwuhopsth.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gqhrojliu.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gzkjqihhs.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gjzxnxabu.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gsfxaovce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/geeazkueg.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gqkcuwljj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gqqryrtcd.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gyxhjazrn.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/grgzxskmv.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gwkapjire.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gpqeeogkj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/glawfurcz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gftskpofv.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gexzzvays.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gqitinykr.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/glqtzxspv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/giazvboik.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gnnmjqbox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gmshglbef.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gnatyzthm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gthtippnq.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gkounlumw.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gekjrenve.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gncymygxk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/ggwxyhdcx.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gtjtowdho.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gfttmfpfe.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gqplkanyj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gxajpblfm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/geexxopar.sHtML


<!-- 参考信息 -->