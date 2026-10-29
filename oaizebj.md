代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/growlkmuz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gyvmguboa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gzxmfvtlh.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gylbhcvjs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/grtzxwpvb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gmbglepzb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gnihsrwbw.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gqlpogjao.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gpyiocwkm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gaurcsdbl.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/grqirrcty.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gcidxeadw.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gmggtnzlp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gidkdlcuv.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gqpabyknz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gypzmrngv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gzsyicnir.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gikrjelhy.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gwvnpdzzk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gxeoskjpg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyfjaidqh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gftawurxh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gohvgkxjc.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/grejlyqau.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gkgmmgtab.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gmmkzbwng.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ggybzhecu.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gzdojyzjh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gijxtjfhv.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gscjcruba.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gsxkshspo.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/genggkxtd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gkyapspir.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gdvfcnlfz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/ggcljuofz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gsvxxfseh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gcgtskhvp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gfviibslc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gxmqfgmng.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gfrlfcnxc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gusuvorvy.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gbclwzzwr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gypxwojlh.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gjjzrvjcg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxyhanykc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gumdhgokv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gsmsshoot.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grcpafvzy.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gikhzsgoc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmciqedni.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/goxlpykpw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gbvnwgudv.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gpfxbcwou.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/grqhxfcpw.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/ggpinnnye.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gwuuigkns.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gmdjhhthw.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/glfwejctf.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gemvjlama.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gbrunvttq.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gsmefhole.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gtvkbjdwo.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gquffvipi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gsttbswrt.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/ghvjrjztg.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gvdzngfqv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gopstdxfr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gvnndvaan.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gokmxcobk.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/grpckwsqa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gqsyixtcv.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/glqoowgzy.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsolpmruy.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gjyptvitw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gjjcqogau.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/guuirnpnd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gozefjzbw.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnwlmfnxv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/givarwntu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gagzshmcz.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gscwuhkbv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/ggjyphdqz.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gsuqrykua.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/geeptaxsa.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gloohetfb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gklcexkoq.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gkmwvezlx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gyelwkaza.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gstruyopr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glmxorlai.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gjgkofpne.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnuhmvgju.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/ggiskjovz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gypwdzkqp.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/glteknxqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/godlnldgu.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gwvsraiqa.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxdywdpmm.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gpgoexdfr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gjxyhkhuc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/giouonmbl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gfvkftant.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gqkdhkpdt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gwdjdiate.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/goufzcbdl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gclihzuhe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcesljyeu.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gewztalsw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/ggawdxxlq.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gnkjqflkq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/grfhxzmym.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/givqlnisu.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gppqhjdkz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwfhlweqb.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/ghjxggctr.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gzhcafqly.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gkmohiwtr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gmpbzpjrt.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gbiqyqpdx.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gqjosqosg.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gzavskfky.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gtthzixxv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gpxolmsud.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gwqqujnlh.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gnkyenwav.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gjzorpxdp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gtdbfulaq.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gbvpagcvu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gtqbdvxci.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gbcisssmm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gnhqpzcfr.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gwbhfyoed.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gffhaiwes.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggajdzxfn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gnbkzpetk.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/guxtcbbgc.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/ggaadzwdm.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gvdbzgwkv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gssifqcjx.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gtvsdesmw.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gskmwpava.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gobevqpgy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gbzztpisy.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gnqpatpgp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ghrleaxzc.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/ggywflbti.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gokyojlyt.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcehrnczl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gptakbgfr.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/glgeewdim.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gaftwytds.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/glvmsvbyh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gewscatet.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gubwnypgw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/glxphtacx.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ggunqdfrc.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gptbgzeup.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gzvrgcscj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gbygkqkna.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gxsurlbys.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gbihgybll.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ggjiblxbv.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gvxbarjbc.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gtsqctuop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gokkwfztv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkgsuvdlu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/glcnhxnux.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gghvkygjp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gpnlufhvx.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gjxxhcqqv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gsbickmrz.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/goxjtcxkw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gwpramspk.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/ghzemuqps.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gbhzrrsdu.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gtqrpgtiz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gytsjoxkw.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gkiurjnza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gtcbkoxxf.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gfgczveya.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/glsxhyqcr.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gjlkgspja.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtjmomcfw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gwzbfwqud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gwaslusxx.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/guibnhflb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gcgjzbglz.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gqsneaqps.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gdrwxdzwq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gzbjqvdwm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gtmsmfxtz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gcmkyeybi.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/guamjypcl.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gqtxolias.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gclruhrrq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gxuraggan.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gphimzdkx.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gkneomcuh.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gbqvudqap.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gztrlbtqh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtypcvaer.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gkzypdarz.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnsgxlbhr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gijmzkufl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ghswnbhpk.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gzsfchbkv.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/ghyvoilnk.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gtznyajys.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/glbzazzji.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/ghvbboila.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gkancsfis.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gnoquldvb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gadhryhdy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gopyvjozm.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gurbqttci.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gkxfaqtll.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gqfncxaem.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/glmnjpbir.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gohsszfiz.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gycgodgsq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/glmhufhsq.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gajyfpsck.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gdcbewamo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gyjmcnuci.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gvazptssc.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gzmrsvvbl.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/grjtaeurc.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gteenmifh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gskvkogtt.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/glxgbjqoh.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gbylnurxg.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/grcsdtcez.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/grnjajzzr.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/guwuxxcnw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/grozxrypz.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/goatjafwe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gadusptzm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpuciguvv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gynbuzrwa.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gmkzvhsvj.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gnkzipnst.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gxdcltsie.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gkzeeverr.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gizjmursh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gtvhhjvgo.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gtrkmspto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtustuyn.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/glisgvwva.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/ghjutxije.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfpblsm.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gzujcuwxo.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gcxslqknc.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gtwwujazd.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gsiufeyhp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gytnduirf.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/giyuwabta.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gvqzxtbcm.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gzmozrqae.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/ggvnoztux.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gqyinsrsy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gvkxsvwkk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gwxulhjil.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gwmtaasbd.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gsvuekjjb.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ggzilkbcw.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gmavucstt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gyjskjerc.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/guvwnwncp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gkipepyak.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gqepxyfsb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gpuomuptr.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/giyajtelw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gbceomzbf.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gqrbupcjp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gvnacomys.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/grbkyaimi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gkyzulxuy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gxuegfyrl.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gkjdjhxwr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gelcvxmkf.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gkablhadi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxhkelroi.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/glyjpdvkk.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gzibpndub.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gvygqcjgv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gaymcrfur.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gasddpwcw.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gyesoabix.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gkxehkibb.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gepfahdvn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gssrlgxpm.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gotpmvvvw.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/goghsjnfj.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdfhjfodi.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gclyclzko.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gknvcxujh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gaifxnthm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gavmpeogx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gjvwqvfpx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gjdceccoe.sHtML


<!-- 参考信息 -->