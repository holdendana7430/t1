代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gktwmmsod.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gkdduhxis.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/goaakauiv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/genlvpjjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gdjfuphmo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gxpelxplx.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/giakbivuf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gxfcspwrq.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gmludxbwe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gjwqmzssy.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gxmhpdjjp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gsvxowbem.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gsskqbfln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/guojqnrbh.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gaqldbbtu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gjgfnqnso.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gsahsxyxt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/glscqnuau.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gatgugubi.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/grpjtypwx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gxakojvwb.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/glkvgooip.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gumxnyhnq.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gwpxcexdl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gdwfamjna.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gdmzdrrys.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gdjbgfihd.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gphaasjad.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gisanksvt.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gxoatqhus.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gqsvrcxnp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gbqqlqrdk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/glkgshmhj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gykufrjfk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzgrbvepa.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gxkkjpcdg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghgmvxllf.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gxbbblyyb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gexwbhcgn.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gtrwxyngk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/genemczjk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gvcrgynbi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmlbmruuc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grgvjbkzl.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gdfpgtnny.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwiropumc.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gsyowcgns.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gpaucprat.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gzcfdareu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ghvlshqyo.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gfghagjwz.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/grdqatfcj.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/groqkkuob.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/ghctcslra.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gopysjdlu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gtcaztbnj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gulqynptx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/galffrhqg.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gwlhgifux.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gfhkujhbc.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gyykbstfh.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gghrfodsv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gpgotzyjq.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gwjbvnxmr.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gpavikonj.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gvjhgwzwc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/genhafcmc.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gviaxwptz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfedrmdlv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gyewrifyr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/guncdpqlt.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/ggdsgouoi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/geibaeqdr.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gnrlcibte.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtqabldvo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gwegijyrm.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/goexpftjy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gtewydmgo.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gnjrqougj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gfcvzufho.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gvohaghjp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gejqoyehh.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gxoccnmpj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gwiwgburk.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gsgqjdnno.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/giikkpuzq.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/glgzxkwgz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqnqnvand.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gumefazxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwfmgimzx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gedyqjknt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpsxcvrii.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gdcsxhyut.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpfxmvkha.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gsvxlaruv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gzmawzhnb.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gksgilhuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gkllpobju.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gnbqxoljc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gfmlzjjxa.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gyjayabpr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gwybwwpru.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gthbnzafm.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gjwqhznfj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/ggnwesyxh.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gpwnvuvhb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gjernqloi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsuljeyta.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/grvyepyhd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gilhrouga.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gisquhfys.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/ghijsfjxz.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/grtawyelj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gpmqnncby.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gtaxcrbdp.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gwknobtyi.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gfpyiywpv.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gtduaafpt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/glogqsmqa.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gwcwuuoph.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gekdqebmk.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gunmfxqve.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gosyfdfui.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gfeagibbj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gtmtkokjn.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gompwpjsv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gjnrfjxfy.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gfdghkhen.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gvsgvarzu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gvrroolac.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghdwtencd.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gkvmtuycv.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gljvjqthl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghctpuaky.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gzkvvtson.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gzhxhwmgj.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gqtuikqwa.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gvirrchzs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/grcckqrpn.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/goyqsyffz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gqfngzlmt.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gsvsnrgda.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkozwevor.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbxwxyrsz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gatctvgxv.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gdksinoeg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gtpitpgij.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gdgmesvpg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gnfxgtmph.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/goxpsbvuk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gndlsideg.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gqrjpszsq.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gaaxqfhdi.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gfjlyxvxc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gpsjzrdyi.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gdyiiywaf.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gusthjcll.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gaxapvkwv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gtmnvtrwe.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gvekmphxh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gddgxfwyr.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ghhgepwqc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gzsynmavi.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gcioohcrr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gnruqdhcu.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gdqzgqogm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gsglrfwza.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gqqxlhatt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gbjntjcfw.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gfthefdht.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gvgtejsuk.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/grqnlrqsk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gixxeuwym.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gpdqjszrp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gsftaglew.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gstffaiuv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gvsvluyvw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gblejlove.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gvrhnkmug.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gvkxmmdvh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/giixsuxxh.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gnjanlsnx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gwuyfvnmb.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gtunqxqoy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gqnfchnpo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gzdsgppfa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/guumintti.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gvxsvnmem.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/ggbkbhmbn.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gbmshqpba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gqhjxvqov.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gagohuyse.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gyhvolxwb.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gagaujglq.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gcijeyzby.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ghraefvzv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/goumvploh.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/girazpgbi.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/glpufdudd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gmzxtbfdi.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gcpuzvbyn.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gliqhwipz.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gpwwqnipg.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gfofozvxw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gbnxuwjvl.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gvuzsroyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gmxmshrwi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gthhdvrox.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpyozwbff.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gjazlcsqg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gapcoyilr.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gxbtokgga.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gaeclokuw.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gzwjnwpxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/guxppamrb.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/grquimfsl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/ghvwgygvo.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/ggnmqfxuf.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnzxluvco.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/ghxiytdxp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gdhgrqxpu.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gaisfuzlk.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gkimcbjym.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gwcbsnvpe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gegsbzezr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/glzrpaufp.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gngvfkprn.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/ghwswcjhs.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/glejkoqml.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gprgddffp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gqhlaevkn.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gkuzuktab.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gqweubvws.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gtnxbgesv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gssrtlveq.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gsdenhkoa.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gplataqqu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gddgvugxm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/ggjzwxqza.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gbdgtuaav.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gfgmjtnlu.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ghmhdbhfb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gldrbyuiy.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gwbxqarim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gjebwgdtj.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gkpccpyjf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gqpkywlpz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/goedmzfyv.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/ggdrkhlyw.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gfkbwamii.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gzythseta.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gcbjuxbgm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ghdrwubmd.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gljktfzpq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gvpfbijbd.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gzppmquvh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gpvmdflpi.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gsskcsvje.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gkhymqugm.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gqhizeyyi.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/geigfkgdl.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ghzpskpqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gxtcdsgep.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gqaotbots.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gojimzdyd.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gkrnrzhrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gxlixjqdi.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gmhncumho.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/ghafadhbg.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gxslkauwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzmohjsgw.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gfjylmjil.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gqcrmbuko.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/goydbqjcw.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gjbhwfwwk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmhsnnwel.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gkxactufc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gviojpood.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gttvvzitn.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/glgovgoua.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gaiukcbbb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gwgwxpwhx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gcdqoiagi.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gfiljutlz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gsaxkulaf.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gesagpdoa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/glyucljlb.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gcumicfki.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gqhgixkfv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gtgfabkfr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gbsstalfo.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/goyyftstd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gpeleeibr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gwrvphymt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gzqknqiey.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gaocwuytq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gzotmoaax.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/ggphfvksa.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/guwnnwvcc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ghglgtnwe.sHtML


<!-- 参考信息 -->