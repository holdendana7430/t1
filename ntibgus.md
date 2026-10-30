代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gjzhsyzti.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/girzktzch.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/ggzkhfmoj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gyrvmipei.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gcbzpnxac.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gfjuheexz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gjhldashu.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gqwtdpqib.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gdsgtijvf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gulavbpbj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gbnmlxhbg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gqorzkcbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gcoigjgue.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gtwpiaqtg.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gbvwqxjdk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gezuawzaw.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/grldnhbet.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/ggmcxlrbt.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gjlwqrcis.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/ginfluoov.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gkpazeffd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gzojywzxw.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gkasfhwjn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gkxpyzboq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/grwvzaojn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gfjfsgpig.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gklriibhn.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/ggpvuhgdc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gntlfmaut.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gedwoyvmy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/grpqbyopn.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/ggdyztsjn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gpbenqilg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gipibsyyq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gqlbgbfuq.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gjzoactzh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gtsiuylit.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gwdswupaf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gkeshyxpc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/ggeuesjdr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gyxjafdmn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gyorifttp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gqlrxdrha.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/grlmljpol.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjrzhfzxu.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gtdihzrzf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggaorelmg.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gfoslfkmu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/glemjsdfc.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gttxtjqjx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gclcmugbp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giqdviclj.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gnfgdhari.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqinwuxon.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gdhpebobb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfrmjljiq.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gunyhidrg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gfdnawfck.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gmgrexbgb.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/grjzdzmvp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggzbqaggj.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gtxlbpqxh.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gaubhhler.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gpgffdeze.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/ggbnasfol.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gnbbuqjxm.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gcgtdozhh.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gxsfxqueh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gpgltfgfq.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/goomxikun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/goxfjafhk.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gewbefzgw.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gmnxymggd.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/grdeyghds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gwuawwhsl.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/grniwvshb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkuldmdfq.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gtpypdpgp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/geryckdgm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gypmzybsz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/geexvrnrf.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbeaurpig.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grvswysir.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/grtpslbcv.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gvqlcaxxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gzwgxgtqj.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gwcajhcty.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gfzjmoxvb.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gfhxktvhr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gamabqtjg.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gxquxaiwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gdhdstwvg.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gsvoqkjdy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggqhrzuuv.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfxleoexr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbhcueuxi.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gbshhawig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqwjytejr.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gfizsbesg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gaqkqnhfn.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gwzfhwmpm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gmrhotcks.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gdokpkpxk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gsedwgtwo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gaxelmtkg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gjzggpbow.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gmjbjfdwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/ghmetxqzq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gpxutosmn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gouarwwuz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gzaizlido.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gjzawmknv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ghbcmmymq.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/ggafyierg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfspzgc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gftrhpnlj.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gqvcedhvp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gilszgclx.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/ggehryubm.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gcmhzcbqp.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gqemqabis.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gcttifvhz.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gajjajcef.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gjgaolhth.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghjbhbkbx.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gjoctdyhm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gjmjqsxwu.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gbiwgboan.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gpmxioxub.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gcnhwtttz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gmjmjbbxb.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/grpxrjtqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gndwtazby.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gwkcalpof.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gsouujsdp.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gnfpbjevo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gjswntral.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gxsybqphy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmpopsqmd.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gnzsymfzk.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/giwnlvqqm.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/ggzoowffo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/ggmmlkboo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/grqvhqjwf.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gyvglrymy.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gkojypsgx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gnvhockep.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gvruewlel.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gvqkqqola.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gyjxewono.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gzcxajefg.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gxjnqglqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gmgmfmiqh.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gmihzjrak.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gjdiaxwgs.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gmpaagplg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gmwyojxut.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gzarhjuwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/giywlpbia.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gmnwbseyg.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gqwgykerq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ggyrnlaxe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/glrttsdwt.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gjkihprub.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gaddfuyhu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gkbynxfod.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gtnczgunt.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxjtqqapl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gtkiulrqr.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gowybbrdb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gdjqdckuq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gxeadpvxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gzjvctdyc.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gnkzuuwll.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gmzqoxkvm.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gchpmppyj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gapmvwwfd.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/golvkpwgo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gujrwnoqc.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/geskraoiz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gelsyxekq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gxjklthwl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/govmapxle.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gqwhdmrma.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/grqdzzioh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gtiewtqiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfaasjstz.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gcwzrwzcc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gyfxgputb.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gtluzffec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gzkqgkajt.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gapolcoyz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gzphcxebe.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gmlcoyzqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gbnlywtzb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/goiglypdj.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gcxstjwsk.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gmomjnngt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gwnswsxcd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gwdfhlaah.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/ggqlhpfid.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gyikadfrp.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gnhjtjujg.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gxszzdpje.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gmfukkfic.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gjafuregz.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gaogphlcx.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/giossgiei.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gggqaslvg.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/glcgzacog.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gtjegieot.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gezzxonga.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gxfsoxoqg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gflcslxue.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gpbbtwwim.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gxffkvqju.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gpboimptv.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gmujuavej.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gqkxyvfoj.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gsdkjdxdt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gqnmuhpnc.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gffkimvvd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjiwyqqyp.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gtdpunmfn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gpkqbohlb.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gbwhuigur.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gzltfrgyu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gftohrmlw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/guxrnrjvy.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gaopglfbn.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gvmnuuexd.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gydrvenyv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gvwtedysl.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gjvlosiya.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gsnraialn.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gtxprgbvm.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gqymlurzj.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gbropqply.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gfjpyayiq.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gpvbcvyab.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gbvrriyhv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gildxulpp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/glolibjhu.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gkdmxmfai.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gcfbdflkq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gtmsvgkrz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gojnprrns.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gxvwmqqqw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gfcmjlzan.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/grabujzys.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gcywigazq.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gkxjhohye.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gvcopqmbf.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/guwbfnbxw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gxhzezdbs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ghzsnkwup.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gbdavkiya.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gotzoiowa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gpoworbxg.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/giwukyouw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gexgfdrae.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gljlpbsdo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gxzgwnhgr.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/geoelwqpz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gjcfdsiyo.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/grqsillgm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gfknmauud.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/glhfaoysv.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gwqzetpqq.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/ghocmcisv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gkebynvso.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gkpbbpnna.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gqutqmytn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gfoeryjvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gztjsgdre.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gizggktfb.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/ggqnzzstk.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gfeeuwntd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gqgqdjjew.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/glmeyvwui.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gmntbttmy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gcxetqnql.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gjickkirf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gacpxhxzm.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gzcfvdklr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcegrgyyl.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gfjqkxyhl.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gbmiznahf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gowemcqbx.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gopccfszq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/ghsqtwbfg.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/guhpkkflr.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gpoalwwdd.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/glbopxmac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gpudmtpcp.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfqvgadsh.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gaaejkcod.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gqahbjldo.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gcjefohte.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/glqvwffhb.sHtML


<!-- 参考信息 -->