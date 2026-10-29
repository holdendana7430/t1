代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gtowflldk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gjiwfrxko.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gsiadhuqc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/grcjjhyuf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gdqebnmhu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gkbjfywrx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gormylxtl.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gdtmciusv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/genqtapkf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gmytyqfok.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gtzkvtppe.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gyxgfzgsk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gqxtpilkr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gmyhyuqsn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbbincolz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gipvanzmc.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gnjgfjsia.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/glpethuqk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gotmjwmqq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gfdcdmvtw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gpvijbdxf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/grbvgnbld.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gsrtpoamk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gfophxmuf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gxpeifvof.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gbidtujma.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gjbjytmqj.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gpsqprsra.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gcguhccqz.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gobftylxt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gtsioagcg.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/geafikyyu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gnprngikf.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/godvipzrx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gfdzuytlg.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gaqyjmlnr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gesiygtel.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gihhzzdhc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gwggwxuft.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gtgmxepev.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gobzsfnnr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gugkluzko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gjielauea.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gbvlvzoni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gifrslmva.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gpupnbvvx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxstprngt.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/grdljkctn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnasclhlm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gysuygfdb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gwqfaupyt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkyltcxvl.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gemhchank.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gahlwafvr.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gyqogglct.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/guncrlkri.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gbzrlafjt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/girqlwzwt.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gjmhuovht.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gpguilafn.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/geelxgbre.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkrrrse.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gtuqizbex.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gvbynjpip.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gkjhlwldn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gkhlsvynv.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gbzvomzdy.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gobtwdvbu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gurzkjyhi.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/grigtmcig.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gieorodow.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/grrdvwimm.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gkwzpzxrm.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gmveauijq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gmlutzbsz.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gqudkorgd.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyoqfwfht.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gvqyrjttv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gybojcwxp.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gntljbhrs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ghsdsvmmu.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gundaotqz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glpbfoxkp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gizdnmsxc.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gfilprsqe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gelryatnz.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gujlyhhjb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gddrrzcia.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gdaujubxg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gtrlyjnyu.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gkvuofrqp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/ghtlrhtce.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gfzkwngqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjqeljuof.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gjepwwdfs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gsxukolwr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gjpcmooje.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqcewmmqt.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwhuhkqcj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxaqsxonx.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gssipnytf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gapzeymjb.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gcomdunzo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gznmssjhg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gtwyjqwos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gcqcfpnle.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ghovzkbno.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/grhmnvpmk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gwlokceqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gytxyxagp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqmjglana.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gommojkyq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/giezxeojb.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/grvpqwtao.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gnwpzzfkf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmknlebte.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gappcqels.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyrkfpyvq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gtijuwewa.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gfdtbkorr.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmdoglscy.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gegkxfeyu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gkfflroac.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/guuwjirdl.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gcvmhgmlt.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gtbqddaox.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/ggpjbemfk.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gmihyyxrl.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gvromopuc.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gfrjbkzts.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gmndryzyc.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/glgrrqyln.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gsyjwhnhp.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/grveqrvav.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/geqksjuwq.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbljptwiy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gqlipzvfw.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gxnqstbbq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gtpjoktbe.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/grlhqmnxm.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gdxqupwxy.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gtwsufmoj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/ggdmejrtx.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gdnovrget.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gautfnshu.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gsikhbdlv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gnexlxwws.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gltciaiwa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gptwvmqol.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gfknpsybs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/glzzdtsva.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gerxrchdi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/grmsekecl.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gsxmwhprp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gxajqbwlq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gzcxsnfjk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gtegvxped.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gzwixdzqx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsryxfrgq.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gexdvdwad.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/ggdpwojhz.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gyqhjapig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gkkkroriq.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gsqegfqxs.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/ggkcrdfjk.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/glmcyrenb.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gchetybaf.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gkuknjgut.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gqacvquxs.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gsjggtopf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gjacwukgu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gqdtgmeod.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gamcioumz.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gtgovceni.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gqjjmenya.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gvereepli.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gxtfcauhv.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gqgingsoc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gvmkcxdgc.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwvnjyvbm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ggvlebpvq.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gezrjwmeb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gbslbbjxw.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gpqjmoaaf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gmjmncvlc.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gadjwjowj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/glhvotujm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gxqxhiewv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gbkqdswxh.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gnhxpognc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ggbtyhjhp.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gkmygmqjx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gjksokayp.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gthbvuinh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gdmpocehp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtxflgkle.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gmgodnylp.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gluttnixs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gozndgqpj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqshpougy.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gzvtwpyke.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/giephfipv.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gvxetmbaq.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/grhmnosjl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/ggotqtyih.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/guyjmmuqv.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpgsdgdwc.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gbicrcrdy.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gyuphvzds.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gfirxuhjd.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gwujgzugw.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gkrqjcswa.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gccuvapri.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gwxybxabf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gbcspuqub.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gtwrcqodv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gbsolzvge.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/glgehaapg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gnmtdsrvu.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/golvcyhgv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gqguzolep.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gszesxwbi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gpzmhofth.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gxrnobjul.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gmzxbergd.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gxenzhdre.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gafnaaueh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gmsxzswij.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gnqcwsfdm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggcinjqat.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gustvwftf.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gvdfssyng.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gkeshesgy.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gqyablqoa.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gikgcmstd.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gmzpcbhnw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gyocxncwh.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gsubckuzg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gsvmnjvrg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/ghlrtphkp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/glaskwogt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gzwpvbizp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gyphvemdx.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gyozbzyhg.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvndohu.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gadjhltqt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gsrveyexo.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gvqaferkh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gkmmqwiup.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gttyhkzzx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gnnvnosub.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gpuattuan.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/graxvwdtb.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/glndjckfo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gyvtmwjze.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gdxattrky.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gmmytavfn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gujxbkbyj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzzcvbujw.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gsedubgtn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gqyujhlaa.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gnfagijqf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gygawydmn.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gsvtmgnoc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gogahhcoo.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gznqlbhws.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gjgnevyco.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gqhvvliri.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gnvxfeqal.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gxmobwjmg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gdcwgnkpo.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gnmoprjer.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gyqsvgrke.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/geiittaym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gcnllohxz.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gfizezhvf.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gtgcbqzzu.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gdschazlc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gbigbztik.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gpzkdlsxe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/glojthmqs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gxhkbuezt.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gjjkgawth.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghseyvlyz.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gcoyxfcur.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxzwomtor.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gkgmmzpcs.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gcmppsmlb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gnfvyxgua.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gpfnbnbhf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gyszyeqyu.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gxiizosyj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/guvawqmfd.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gjpniwjko.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gszyozhdg.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gkwqoigrb.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gzowxhadg.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gnbrsdyrb.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gwcqxsdcf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/ghnwolqre.sHtML


<!-- 参考信息 -->