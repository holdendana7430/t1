代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gcjmyabxe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/ggffgbncr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/govsqclur.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gptoiqidh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gzoxnamwg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gzfqtspum.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gtgqcghtj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gfoavmxtn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gakqjwxfo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gfubapylm.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/grplwegpv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gwehmoolx.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/glxrjlknn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gadjgbhrn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gtipklefl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ggjyfyctx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gesufakyj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gofhqbxqz.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gzskcczlc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gfjtbiurj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gybtmuram.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gulnugcvq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gazgfyavi.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gtcjmzbua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gvimeldcp.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gglyfspho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/grollnrxh.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gozceveyh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gyepabfvj.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gxjqbndrx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gqlxeouuc.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gvywxbisz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gnjswzbrv.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gnzcshoks.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/guezndoqr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gttslznzo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gyajlzdww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/giizswesk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gnodcymjv.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gjixvzioc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gddizyxjn.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gpmbdwsff.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggzaziwcg.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gypusakkr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkptofh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gzejdssed.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gbefzuwng.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/geqxduwae.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gkmxgdwec.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gyhbndmwb.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gcpcazsrv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbrdvfkgb.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gnpbodlaa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gnwrsqeah.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gnsioupvn.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gyxoajwsq.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gftrwsmvw.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gnlwrsqgx.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gddnxaiko.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gypvoqodm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gknlhclaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gqljtttbz.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/ghajophcr.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/glfklbsbq.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gerpafmqo.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gnqfkvwil.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gnndfigoz.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gacoajqzz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/ggtxrzhvx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gmkqnjian.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gyxzmrvuk.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gtvxwvtor.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/ggymyajlk.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gffriuygu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gmcvuthmn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/glewccskl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gwtwckccz.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gaoxbsqvr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtfkkpkzb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gxzdxgntl.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/ghqxmoyuz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gqpbaqher.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gakiyhmoq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gbwtkdird.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gxvzvikna.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gbqbjwrip.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gtlsvpsjd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gqcguqcjc.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gykmrcddu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gufcbezpl.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gkyeogglr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gejlrofxt.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/ggcdqhtvd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsxiokezz.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gdvffugms.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpagntshv.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gnotkismb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzmwybcyy.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/golsuvxho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gmwrfgbee.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gxohqkygh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/ggafkruhf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gqfdomdxf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gfqlniobs.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gpxdylxdv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/ghdxkxecz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gwewfvyuq.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gqvmgnjjq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gjoskywis.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/grsfgnaxb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gpeuisxjt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwzsphhwe.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gzpaxzvzy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcphgnbme.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gjtxpgwcs.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gxkffcejj.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gxvyjfoik.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gheczpdrp.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/ggfdgmvzx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/glnjqzdmt.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gsurufnpz.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gdfrtlojn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gtpfumvvg.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gajgvuuam.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gibbyhvzm.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gkihgwuhk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gxqzmbpzq.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gvqtbjfnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/grehurraf.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gyocrzfcf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gjqqjvzpf.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gowqspbnq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdncpeojc.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/glwsrxmve.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gioajwsby.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gxdzhzbqw.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gmnqpxzhy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gvwlcsbaz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gpeewpvto.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gyddnqnsc.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gtuspgbkj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/graizagbc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gcxwxsymw.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gwngskujc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gfbmyomgi.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/ghxfvvktv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gasmyqdee.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glqxhhunq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gssffdakh.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gbnmrgwld.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gdauzluuk.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/ghppyawny.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gqinscdjp.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gbizbkazj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gsoffxhnn.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gopybszsg.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gchjbvgay.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gomyyqtyi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gawrqzbjl.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmhtpljam.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gjsniukjg.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/garmliawc.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gkrvceljg.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gobhvrmxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gzmjicoov.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gwryzdebk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/ghqsfwlyx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gqvapbuns.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gsqbtoonn.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/govifdszv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gissksevv.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gdchphlqm.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/grkvgzkyn.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfnhziwiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gxyhsuith.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ghgvofflx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gjdjotohc.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gkeroinhk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gcovzsmho.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvcfeuvmm.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gllxcvyth.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gvoeelrke.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/godbppjwp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gouiitwdp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gxhwmwhsa.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gywywszhz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvdxqxinw.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/goxropulo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gfcivwbfo.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gdjliuzyh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gmlciqggz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gixipqfiw.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/geiaiuqzn.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gzuvuaysk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gsgngcjgu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gssrrpyrk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggzpdffhy.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gtuvdhcwz.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gegmkdsiu.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gwhxtcjqq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/glymcyklw.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gfkmrucso.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gknlevtds.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gymopuzyy.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/guaxbsygg.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gbsfjbjqp.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gpyaqtnzq.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gehrqtehs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gnshvkqah.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gryhnfpey.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gguumawwi.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gzvrrniwl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/grdgfedmt.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gmskdhlwt.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gulrkpsep.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gxhxgzdyg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gldhsryzd.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gxhtzvscb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghnpyfgwb.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gfkdmcduq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gvdmmerhb.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gmozboqai.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gcqzgdcav.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gedtlkeck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gthovnhkp.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gmgymoltk.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gnxjxrlqf.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/galcaaxzz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gmfhvmpvw.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gmkypmdgs.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gpdxofcka.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gwrkxiosv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gfvucaqbr.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gcgevfywy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gjuchblse.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gchumsjbc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbrdnfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gmlmqrfks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gbeuuzuaf.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gtcdodobj.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gdegwdmdg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gryxoutyv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gmtujkcfe.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gsrbcllle.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gqrqjdypt.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gzdemohon.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gdsniygdj.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gymaqdfgm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gbhoguwni.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gnjunirpk.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gosmicqae.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gxgtrxnuv.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/ggqdtzffi.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/guirhtpuk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/ghfyyzvzq.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gxiclnnkm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gulwuangm.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gwyeiogiy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gtyepsgdy.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghcpexcpt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gibnqimuy.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gupiztjja.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvidrxvxt.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gmfihcafn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gxczniawj.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gcgqbcpxr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/givoifhjz.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gmsrdwfwd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gijwsrjqz.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gtsniylyo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ggfvvcgws.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gyjkwxfwl.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gvpqoopco.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/grgvwgbdi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gedwdfjwz.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gewcngjlw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gjgexgcti.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gdcrbayub.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gaxojqpxd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/griajnzge.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gvoesondf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqvwctsek.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtcdujqan.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/guqpepngr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gmoeahtwt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gulwtlvau.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gxuzdnbce.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gvnatpanr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqtpotm.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/geezphkjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/guqvugimt.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gutksipbe.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gvzalpktm.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/ggrjzafgj.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gbsqcuzlj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gxoklclar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gtobvbrsy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gvhyseaal.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gegjmchtk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gjmmycyqb.sHtML


<!-- 参考信息 -->