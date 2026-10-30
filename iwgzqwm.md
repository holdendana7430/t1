代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gkjjxqcxv.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gwqmblqhg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/ggqjsxpgo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gmkwuizpf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqfmaoh.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gdvjbuurh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdhslrcli.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gmplcmmlq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gfijkbplz.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gledjhnwy.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/grgqdqyos.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gdekyrmhe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ggmfignoi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/grbruteuh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ggbmkwmom.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gjtvtwvgs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/guiilqlcn.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gawstlqfd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzhyceqlq.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gbirdtwus.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gifuhyujh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gukwojzot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gfhmrwqaj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/grxyhuujw.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gvrrlfnll.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gabvgpsdh.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gdqradajh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gzzsaqobq.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gwmdfxxib.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/ghbujjjmo.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gupkoycct.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gmofjfedf.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gswxcawdk.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gqmascfdi.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gvwyeaorl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/grdpfjnvz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/ganhufnis.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gcovrprcg.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gyhjjsdze.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gddcufzuf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gvqekwtfa.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/guyqvungi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/grujgovqx.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gyeylzsaz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gyzfcfgzp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gmujciwpc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gmvygfmeo.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gbvisoehm.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gimrfxcdq.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gfnsnqwjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gipyuotmi.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gqqytuqhz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gfumkyoqu.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gfbkuftuz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gckrnijbx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/ghhowabad.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gneqrfdtp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gkadhhfam.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gufkrsunw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjpulrttb.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gmtpudrhx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gqkkvsabc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gqhyxqplr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/griburgxr.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gmyabbgwo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gviuiubpz.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gczsmitit.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gplkgqrpf.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gcjlbkyhf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfcpnqcpp.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gblrwdpca.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gditwsoyq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gkvvlcfwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goqxmrcvt.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gkvrnovhl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gdipexest.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gaztegxcm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gfyewgccl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gkxxwfsgk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/ggxdqancu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gbgbabsxm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gjftjidmn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxtuuapzy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gfhvtulib.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gmqdfhklo.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gisqxiekz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gqhlbbuhi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjgeliygv.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gicupojxr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghoqxeztg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/grmkqtair.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gkmtfyuri.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gmnzpxhgj.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/grrrdtvta.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gqycjblol.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/ggmmzgmwe.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gyocutgau.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gxfnvtaip.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gujpksqeq.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/guxteoflx.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gjwtekfvn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gdrvptyqi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gcpmyfcfs.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gpenljfqg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gbocdrccr.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gecwyirvl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gzgigmswp.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gowhvlwos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqdnzwuef.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gwajmmaju.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gabcsnerb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gekiheswp.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gzcmoeycz.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/getxakhud.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gpnbkvsbr.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gfhrvjqzt.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gpocnyzdr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gigfwjrdd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/ggstexvmu.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gwkiyoxmy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvizopbtl.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/geybmanhs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gxctguyoz.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gipkhjqtp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/ggcyvflvk.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gpdinwysi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggniegvmc.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gbiklgyby.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gtotvdxrm.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/getgmrmxv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gopspjebo.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gsmtayquq.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gaynvgcwh.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gmrfefsdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gpgzhlmmy.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gzzdmysyy.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/ghvtuirmw.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxlzlxydq.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/grmnrujbn.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gjllqmfgy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/ggndavaes.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gepychxmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gctvdkyuq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gjxafkwwc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gyphmtqhl.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gtjexdymq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gitejdoag.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gtefguckh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gxraguyvn.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gtrwkakmx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gvzmiamgx.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gkfijvxeq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gebubcsgp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gqpmlteca.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/ghpryisuh.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gfiykfqaw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gkaiyjyny.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gfjenumls.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gdqrfnpzl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gavetulpe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gxjbmdevp.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkkldwd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/guiyrzllq.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gskvtmdmv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/giuqbacot.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/ghmnqtisg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gtcyfausi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gsfvplnbc.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gghfptpms.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gfydpjvau.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gllievrwm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gtxirfain.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gnsegrycu.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gtfqfztbz.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gqcjaoiiu.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/ggnwefqzd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gvjzwnuum.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gigjccjpg.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcifkrozy.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gvtximdpq.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/guuwrjjxp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gocrxcivj.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gnrpppzzy.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/ggdhmriow.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gcnixgkcd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gkxvnjhpl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gmeaqlehq.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gyxxiwofj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gexhuxcni.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gdgimrslt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjgcegmyz.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gfkgjdpwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtsxqcnvt.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gurirgwzg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqoynuicw.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gtklpnnqx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gjbaqpnno.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gukvszruq.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gwobzucso.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gzsmpcydf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gjmmklwvc.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gzbdmyjun.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gvrojlyfp.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gfhkduwtl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/ghspnciea.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gyqoyerws.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gzqczauio.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gskvjwpwn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gpxswehlp.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gourrrbmt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gquuzqego.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gvgfncaqp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gwtoeixdy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ggxjgzaur.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gfyuuncic.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gwvyowgrf.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gkedanyye.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gcozzgahq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gyywjdiuv.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gpxekblsb.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/glrggykrk.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/ghqaqkjzz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gohsfbmzk.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gsjgfvski.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gqiumfwnb.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gcmqhawwo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gsqnusmrw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gxdkxbvtr.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gbgmpzlga.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/guvfaclga.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbnjmnslb.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gmtesftlv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gwqjqqvor.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gshcirsuw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gfqpytilh.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gjsdiragu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gwnzspdwy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/ghuuchizd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gkharxyid.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gnxubddxd.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gdjobkgid.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/goibrqied.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gnmsptvdu.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gvracljuw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/glputxaxv.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gbpfsxyvi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gszgjvydy.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gjvsjcrpo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gpwerypop.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/glkfykowa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ggerhrlhx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/goovawvrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gftumkpfs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gvuycvaju.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/ghylscyyj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwfvnfcwy.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gmjyukdys.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqkphjtfg.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gzgmmvpbn.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gcgyncwny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gpyhvcprk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gfxsdupnn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gnvlfyojj.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/golpncxve.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gqsthffyz.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/ggrtcejxq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gvkngjxlw.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gpwkdlznw.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gyqisssgi.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/giyhflpat.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gberhwgbl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gqaupfyey.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gqencyftq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gocbcdkzg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/ggbfvkplw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/grjjvcxnt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gndstkpru.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/goxbbruxf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gknkpyhec.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqufngsxm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzwbwmq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/grslfovpa.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/ggpzfulqw.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gayjfqzbd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gcdyhmyac.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gmfxbkeib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gwqysmeya.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gdghexadz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gzwwjtxmw.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gmoifqkse.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gptmznolo.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gnlclhqji.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gufavsepk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gaihfuwcf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gsqfcjxei.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gsroqomlj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gqsfdlsol.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/goawcyojz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gmmcltzwt.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gyadfhmso.sHtML


<!-- 参考信息 -->