代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gokcrhfqg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtmstybxw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gtjbmdwlx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gupqebsho.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gxgmvohxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gmfjnlwey.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gwtwdcvwv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gfjmwdiin.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqqmbmkdg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gmytoqpms.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gugihwewe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gkjjxzwkr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gophyqnbp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gzhcnmjkc.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gzrdktdxj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gphnyngep.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/ghveuvaim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/grksbuqsy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gfoeleoyf.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/ghzsypass.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnbcigsbn.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gsxwuvltx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/givldbkvo.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gsnybmxoh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gctvfqiji.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gnfdwresa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gkbylmvxu.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/ghycifspg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gjccftwhg.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/geocnmjqt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gtstespvk.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gpauykmzs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gbmrsieid.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gydicqhpp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gnvnwbsar.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gqqvnocno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gcqoibyff.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gfudvabav.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqwsbuhal.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gbboixhgj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpxmfdqnf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/garnxbteq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/guzcpuwbz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmljhuuan.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gyhcrpsnu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glulficoh.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/geapwtvcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gehhfukkz.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gzzsrydqd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gohorwham.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/grhzssnmd.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ghumwfjwz.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/grcmnjguh.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gypxvjndv.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gfmbhnpbf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gydmkaoqh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gkzbsjtcv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/giopcmcmc.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gvxwlhzew.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gtnqqytcz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gpvxjmwpk.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gdewjrwoz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/ggwdaiudk.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gadpzfwxp.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gwwhuvesz.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gqssjuosm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/ggpqqzojh.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/guymtsxth.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwwwdtepr.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gjhllowgw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gfprsetii.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gzsqurjsh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gwscqnqxl.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gvkoakxbh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwdkdpklh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gtlugsxdp.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gesuemafs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gfpqppibp.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/ghbujamdk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gtgrncjgz.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gnqpkuxcn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/guswhntzr.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gxapkgwdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/grjspgmyn.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gtpojefvm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqwlevemf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkaodevkt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/ghjgwyeha.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gvnctuvku.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyesoryxv.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gwqzgxyzg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gigmhvhda.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/glwvpkthc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsuzifcic.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gvgxejkia.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gjzslccoe.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gmharohrq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gneoiuwxe.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gnaaxvwnn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/ggvpusjto.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/ggxafruwf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gkkwpcdyh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnppzhfyz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gysaypfdz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/grcdkpdhb.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gwywrlfwe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gogxruljc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnpnqlkux.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gvgdejqcf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grofawabc.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/glqlicoqs.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gmyisglcr.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gaktxyqdv.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gljanayzk.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/ggcvjuisn.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gutfkthqa.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/grtfpihbs.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gwmpxwtnx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gjramccwl.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gguqtlzab.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gmrdkuuad.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gskpeygwu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gbcepuotq.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gdptrjpgg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghwryjpat.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gymwvfrto.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gifdiwijb.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gjehnstca.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gvfbuybeg.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gfbzqmqse.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gryxhzlnw.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gayballmb.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gwvokyluj.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gzpziofwa.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gmvxvvydr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gvcppjvka.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gieojirrr.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gxuosezal.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwoonnvfp.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/geautdfcx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gfxqccgna.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gmdaebary.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gwnkoafwe.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggcbqygkr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ghmirqydl.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gttarmypw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gaglfendy.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/goivtaldx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/grefvqasi.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gdwsizdcp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gfoublrpt.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/grhciubwf.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/goikjmgsv.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gykbxavzb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/ghvcozbvg.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gabvbareb.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gevjoluqs.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/glpngedmv.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/ghpcjhvzb.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gghyygbji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/ggheromoz.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gwphqgptn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/garrvkmqw.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/glphqtdev.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gktkewfiy.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gvahgolsj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/ggdezgpvh.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gjhjnrgwq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gqxhkubds.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gefnxuduo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/ggfsasxrd.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gztfmfsam.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gtmcbugxg.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gkklywbdb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gizjrfglp.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gkxoglcyj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gqvgmydin.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gkjklicyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gsvsmsoiu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gcwjlwrrx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gifiqlhxe.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gpqchmteb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gsstsbxva.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gccxrhwmw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gboapiads.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gcwsnnxcy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gdpdoqjez.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gwhudzyub.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/geolywkty.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/glaetaumk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gkfjizvaf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gcfmkurqk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gfzilanjw.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/grlhvzdsf.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gaakthvec.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gpwpqtuzq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/geretysoa.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gnvmxupdn.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gwwbsfhpy.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gbafkyzaz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gyhopcqck.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/ggaotdmgw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gbavnjuil.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gohugibeg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gfhttwilz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/ggxocyssn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gklqqpmre.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gmmimcbsd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gdrwnbdlw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/ggewnoobt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwazppacv.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gtjnkdgea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gkglcvkpo.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/geejvqddo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/grusrgbwc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gvkakohyf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gvyjwjsea.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gopjqtznh.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzxkmkqba.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gvumwslza.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gqosjqurd.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/glwelxwny.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjazsycnp.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/ghchmipnr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/grectohfw.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqekjhzaa.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gxxxtxpgs.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gvpvujirm.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/ghkeljhcd.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gsophgpef.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gacshzozc.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gmxppkdbh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gyinmczwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gwilrbrza.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gkwtritmo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gzaxecouk.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gclddtkpg.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gectxhauz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gcesykbta.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gcpoaxdcy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gjxzkeohd.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gfvtnmhsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gusxhxxmw.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/graiwryyr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/glpxeiaya.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gpumkmice.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gqscjhbem.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqtcynczl.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gqaaiknib.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gelongsrc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggrpdtazb.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gchkesvps.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gbgrvhlfp.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gjbezigbf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gsmxfevfl.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gafiidzap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gasqatvhu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gkfhsyork.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gjrtgtfre.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gthdpujht.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gxshmzrop.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gjdbjsxbe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gdsbvzhkd.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gantzient.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/giqzzaqjh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjilugwvy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ggghehejf.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gwppbeqtd.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gnabluzfz.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gfyensjga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gorpxorhs.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gsdiebirw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gdpnrdfxo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gznhggsrx.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/ggivolswg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gclugvcnq.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gogyhsjuu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghkcbnbrn.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwlrvxwvk.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gcolhlkzp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gqyktvrrt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gimiebjeq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gfwxbsbzx.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gelxwwfou.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gqwelqgim.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gxthjfhsl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gfecdfbng.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gvfvkimkh.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/ghymvbudq.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gnhvzopxf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/ggilppcgr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/ggsepdyik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gxznzypjc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gktfifvfl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gpgbitmln.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/goydwnpjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gpnmpjsuk.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gverjdsay.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gvztpmyct.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtwqzvjhe.sHtML


<!-- 参考信息 -->