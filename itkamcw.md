代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlpsdgjk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gwlfhdgjh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkwxsmme.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvtqctma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfuemfbn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gslymxjyy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbokjihyp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzculexjz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gyylfjped.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsslaiqq.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjaglxvf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gracheahx.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gexayxozi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpckqxenw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grhkozvkq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghovxhpkp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/ggiyejfdx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gdecfhwyc.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmuxjjyzp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gccymogee.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyaqkmds.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gythadcab.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmuqgcch.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuirpenc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gdcybisff.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gehbqbevt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/givllvbik.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gxhelxygb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gnltumavn.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gchroeyui.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjlomfbv.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuirfmjh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfrtyjc.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhcxwazf.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/ggukctkno.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gleanwjxm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/grhozhnrp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnreytrcg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcfyuftq.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/ghllnugop.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiowzygj.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnsjvnvuv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzjeqdfi.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gsstdurmf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjqgxhlpw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grvjqbpyx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkspptvcf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grfpkkkst.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhzhycap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grstwcmhl.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gfmbbhofo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvvdgxtw.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/ggskgdhbw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gvskltcqm.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/ghtssfzvs.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwexoyrc.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvkcobin.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gkuxmveim.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghgdyiybd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmhzhfzr.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gchaywqbo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/godkkgehc.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxywrajby.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtefffbsk.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/geupyweqn.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvfbntdu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotezqrbo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxswsppu.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/grxdcbaus.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gxfqphwat.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gedoroyil.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmznjwkvl.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvkfqyjoc.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjezejujn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsqckvtw.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/guoaluwzi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkknfxad.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmbpfbkb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgeycyxy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gndvspmnk.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gkbatabog.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gdjvguiwu.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdswacol.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbepvodxe.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gojkagfcr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwnlfjsa.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjejrfvm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gsnnzfxjy.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsxojun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjowxxggt.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/geyhhhwug.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gslgzqjqs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyewhksdt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpkuxhte.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsspzvzi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhsoelms.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/geehpsirp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfhdkkdj.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxocyiuze.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzehddqo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhfkswty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjscelzk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmstrlsf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gylwftqku.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmncrphq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gcequagvb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdzabyol.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpkuizfyk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgogemob.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/ghweanxhi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesmujbxs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpfpdhwwf.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzanqjoyo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxfocyrl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpvxgded.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuaszsvx.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gvplmesfp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmzencbr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxentibo.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxpingjd.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzqioer.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqrdlirp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gtnrlhwlo.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/geebimmtu.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gplfwwaqp.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjeisprbd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcoohuai.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdxqyyos.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcxstxyt.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcjijfrj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmroxanbu.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiigwzzy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ggbcylzhx.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpamwtbp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxfruuwlm.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gabklxoxr.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gderjzbjx.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gltytbeik.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpuhrbzg.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtxmioqm.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqnztnv.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gesjzxlzy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkurmhsbo.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqbyjmqyu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gynvbahge.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gcsamshks.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/greitmcnq.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiiulyqi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaumuxwy.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyyriivpz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqljojcyv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrajukbe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbqowmzko.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/glcnmvtfo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gligokyza.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gisbacrvs.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpkpovhtl.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhcarkec.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrzoijrx.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbbejikqs.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbitionx.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gvggjzrfo.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gddnqimcj.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghknpsfwm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyuthskn.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwhcnqo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfeumyax.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzjvjjsn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdfexyzat.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glcjmxlpj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyvghcqp.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gtjbximci.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpxchaas.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeydfquw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gvvhlrlhr.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghotqgzfc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzmlvzfmm.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gplnkzwqy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmslxqxdp.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwkafyan.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkbxhxsp.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqffbgath.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmapvmws.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvdywjga.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphloxrsf.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gshvdeskh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gssjauspr.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gelkfxomv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gipjeenwr.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxwclymwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gshkozooj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/guhztgepw.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxlbrxuq.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gpgshozya.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/giifvnmux.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gpevhpeol.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gliwscdsr.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihdaczwv.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/guhtsupzp.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrismbpv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkstkurzi.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcbpulxg.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfxbaeub.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gupdcdynd.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gyriokadz.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/godfsejrc.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grfpxyttt.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxonluleq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gucizsjos.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqlksflg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwttfiorg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guryezdov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzubkdijr.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoycairs.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdunjvp.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/geuauauwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gjuvfubep.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwztmaosf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geaxbkmco.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gaykhxmsi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkljupzp.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgyfira.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvczyvbnf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gpsryjyfp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtewgpyo.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwubaspu.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhkqjdk.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gsdsmxzdw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gmmspgndt.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxllrilmd.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjmqjqjl.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gpefouytx.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/guhehvsoo.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzqthhhls.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwkastwc.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gakxadsfz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/guhnnjgyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsodapiim.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxjwzwdqg.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfcyrisp.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gsswfpczr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyspihhw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gfjrugzeu.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girgacpoo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaelxypx.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgnewjhe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gfgezfvkq.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/glewoggva.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/glddwbibv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggquipcyz.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmmmaqpsy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyorqnry.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gajknsoxj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzefoimzz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzhvkwfkn.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyxdwsot.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/glxhujcls.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrlamfne.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gmoacqmoq.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawnavmj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gzuyjjaop.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjyqlnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdabyhxrz.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmeycuec.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gfvvegoqu.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyrbierk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glbckbhut.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjcpnjob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gmajbyqfp.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giqkxrxya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbntddfj.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuklvjql.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdootxedv.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gqsqnqfsc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzrdmjlb.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gobnyohzo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gopiaywud.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjitnlict.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gmirsnzyx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnzyafgs.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gtkbjivjn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpirgffni.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsopdjwgv.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqatrabj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gppkugwrd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gxspkuziq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmvsgcnb.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqscvli.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gxyzbaewa.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gzcdddvqr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guljzvqsp.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwyrgsdo.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpmoshjtq.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqxrsdg.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gvdpblelo.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwzgdtxyv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/glgvuseeb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gqkanpeal.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gwmojmqsh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gujlruxdg.sHtML


<!-- 参考信息 -->