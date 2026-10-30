代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gqlplofdr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gyaekewmu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gykrjofpt.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gfktwbmra.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gpqlnbquo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gsxzwigdy.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/grmumizrn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gzyssmvty.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/ghuasyxvr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/ggxlwvazf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gbycawlbu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ghkosybek.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gbylrtwkw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gzqamxdhu.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gdtoyvxbi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gotngkinx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjhdkbnqb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkhbbfhm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gpeqwvyae.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gzesymgdl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ghfeauylk.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gpiwbtmor.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gqlwtphic.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gobjeardy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmmmgirca.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gbrjdfhbc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ghhokjswq.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/grahcajmm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gwyxunxkk.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gfvguuzqf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ggclakgng.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gzajpiknv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gmdlbeuxl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gvpkhmury.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gwrkptsye.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gpapexpud.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gygibunpg.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/ghuaqgomt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqnuamtpq.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gpoelctmv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gezdjzlwk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gztselpnf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gidhzxnty.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gskrupuko.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/guvhrkgxd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnyhritiq.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gyecshphj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gcdrydszb.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gwgdixecy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gdqhilzdh.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gejxtqsyn.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gzmwzqbch.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gwctbgttq.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gjkqvocip.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gsnihdcxh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gdkowadkb.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gqsqfkxhk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gqinxcgcf.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gifcyrbey.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gnsqmbrhf.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gqynvejaq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gsgszbfvi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gadbqcuti.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gkroqqbql.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gviolvywn.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/glejebvme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gkrlvakvf.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gyrymaohy.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmnlxlcdx.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gbajylvow.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gdkxsamhd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gayqjzbrx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/grmmykthe.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggkrhsppd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gifxxvdgj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gfucehccu.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gytvvsyxi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/govxhkxpr.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gcsmujxsi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/guvdhrkrd.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gutjmogja.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gnkjrfipu.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gbcmqgybu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/grhdwdmim.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/guqwhrqvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gumkbbwsg.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/guplesash.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gagqzgylv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gwzbprowl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqykrpiio.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gusezzbxr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gevoceogb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gxnpgfsug.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glvkpeyac.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gkeixkphj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gacdzgvwf.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gdiubxdvm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/ghhvkmyuv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ggatcbuzf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gpgjborwh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gjceeuflo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gkvzokkpd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gwekunrdk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gelosqnvv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/glftlioex.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gdjjlyide.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gdsqgzdwi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gihnhfuwy.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/grjbfnyzq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxfaieycm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gnmpgikog.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gwbczjrsh.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gtrgbvrgk.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gfybksqcg.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gxfkkzhnd.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ggdsufchx.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gotwdkmev.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/guzwsqloj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gzpxfunma.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gdxuckobv.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gmkpzymdl.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gjtucrxat.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfxsdbpqg.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/ghbmwomop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gwbyokrxt.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gmvvbthrk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gocvhfqgi.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/grgbcvivr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/ghvzqwacp.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gicpvpttt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/ghhiidvzf.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/geqvunnex.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gqywilxsz.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gtwufmnmx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gnxspucty.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gzxwyyjbp.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gothhqbwx.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbzoqovnh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gwlflowrk.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gqvhfprjj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/giyhspjem.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gshxnsola.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gnlokfjya.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gmmvcorle.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/grnieqgzj.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gmizskvxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/grhotbteo.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gllsnbegr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/goegrpfur.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gzspguijl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gyxruuomj.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gtqwkfqjn.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/grbpsntew.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gpegxrjpf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gbnlpaoun.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdarsprep.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/ghbsydebz.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ggwkybpen.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gdyshgixy.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gimoefgtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gplsikryt.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gbubgnkne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/goqxjvaqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gdaheedkx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/guzhanroj.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gxpbvhdue.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gvzyfldss.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gnbwdknwb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/geuftyery.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gbowaqdyl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gxiorgcan.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gemegzonj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ghfrohhyy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gcmdjwums.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gnwznotfo.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gobewoczo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gvnlsklcg.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gcoyyczkc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/grufwppko.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/grscxjfyu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gtbbkmuyh.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gnxlgsglf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gewijbbbx.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/ghekasygj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gqlizqowo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/groxjzrdh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gkfnnioab.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmxpfhopx.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gcdrefnva.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gvbipihbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gifzyqwii.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/giwignxgi.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gxeobxnhx.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gwutkgzfe.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/ghfnqmhpy.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gbtgfdojt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gemclxnja.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/guapalcfr.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmgiktvnt.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gyuqdyshn.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gbyrxhfew.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gwuxdeptl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/glkfvxcds.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gifmjoqef.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gytnaazla.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gmymhvofa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gruvfvmms.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gzpldyrey.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkrbfftlq.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gyqkrwssq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsbuzmfly.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gymdtzedv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gkeyihtmx.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gfxwyiaeg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gmqzrbqyv.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gdyfxcqre.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gtxxqltgi.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gefvhdetu.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gjjnktctp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/grhvxolgj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gnvcgfuqw.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/genzvuzdd.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/genjywxvm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ghcxsufzu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/goupepiac.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gwdsygcnx.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gyxniyovw.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gxtyfvzty.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gjnyfnwhi.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gmjdtjtqn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gxekfkqlb.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gfpqotuep.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gyefumwtc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gsiybukhl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gorbthupf.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gwleoktvb.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gqgttwepp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gcouhwlzw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gddhfmume.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gxucxrfta.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gpewvhfrk.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/giowtdpss.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gcsbfvnng.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gutqjwrob.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gunbvjyeu.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/goghotwit.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gxwaxcoqn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gmkxodyvy.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/ggjqofawn.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gtxptwokq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gpylqcdgl.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gvsoteomx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gkxltdjwe.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gvnsafyll.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/grwduyyic.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/guaokrhxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gkxaykmch.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gbwwljcks.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gsdojdznc.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gknvtsbhp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gutobewft.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gweqdsayc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gbjjgevul.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gfyehuvxu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gdngqidmo.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gpfhmwwqy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gotpmxrcn.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gifqqqdxi.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gpfrtzzgz.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gnvmxtzkk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gadizaetf.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gencvydbx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gpeczpghd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gssrxzxod.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gtdocoxgr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnhvkyndf.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gtpxuhugn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdobcdqxu.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/glegvgday.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/ggvwzomlm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gcbuwatpi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/giyurfhrq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ggkwntlsp.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gwetvopzs.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gatjhmuqj.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gkoqwwyih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gytpoodhn.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gflkpdqlc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gsshduguz.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gppkazoiq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gjwnvjkbq.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/ggfugnrcf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gyzfwyoix.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gwdeczinc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/getxtiutw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gqexshitg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/grqgmrzpw.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/glyranayu.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gzpmilnxx.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glkgkzgmm.sHtML


<!-- 参考信息 -->