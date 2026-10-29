代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gzztvvggh.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gnyfbcpke.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gtyiwnfvb.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gqbjssiox.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gaoadmjaf.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/ghazszhqq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gzyvezrif.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gebcxldvw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkvpqtlmb.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gibbiskzo.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gsqonkzmf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gjdwhzvym.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gzxdtnbwz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gybyvzftn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gnowukhjn.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gfegxmcxj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gyroijigv.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gjnxtnzzo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnpchberi.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/grqrinqme.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gucmtexyc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/guhexvkzm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gkkhvervt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ganieebsn.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gmkevdifb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpfqfqaau.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gzrfxrqvk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gnzbbjdjl.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gajuuzbtl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/germnwnxp.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gchyjbdnv.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gdwbyvwih.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gkoytggjx.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/govpqxpbe.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gpswbqyhr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gycrssnsu.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gpukdhkhi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gqeswdnzj.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gjdphwkkm.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/ggrfsadxq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/geatxiofq.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gdcaghzjt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gbgbgvavi.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/grvquyxik.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gcjywdfyy.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gdzfxpkom.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/giornkabw.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/ghkiguutc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjaqlsdgt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gndbvyjgi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gulnswrrd.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gxnfgysoy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gnphcdkth.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtdicrrqu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ggdepejwv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gcyvqzbje.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gltjaxbrr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gzuuxysbm.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gkbdzbvvt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gvhzfrudv.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gwmciuzkl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gzzemozkm.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gluxffdom.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/getpxztsm.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gqspgefqe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdmikewvt.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gwrnbtrbt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcoqpuvla.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gjgcxebii.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gshciepmq.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gbkgqmlev.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grmrclmnj.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gfomdtslm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxvracltu.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gznzqxgeq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/grlttdfrt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gjrytuyxh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gfmalqlpr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gsasjfirj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gwgctoenh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/ghuedhlnt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gmubknvag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggfgrcfxs.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/garalqszm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/galqawewe.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/grghmimih.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gztmmphce.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbevcjktx.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gcktsnsku.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grhmqugok.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gnafqpshg.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gahxyazaa.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ghduizaua.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gabyptxnu.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gdotptsvb.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gftrbttzh.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/ghpibthne.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gxffshxps.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gkelwzihg.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gntczyrhz.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/grgjzqgal.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwtjpcxgr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gcsbwcjxh.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gwqcsoqjb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gwuyyoioh.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gnkbkttpe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/grxebylfw.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ghbvocvwk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/guisnxkjt.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gemrwykjl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvpxldzbo.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gbzsefgqz.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/geaerwqnh.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gasnbayxq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/grjpjponi.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/giuxirsuf.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gxqyhqumc.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gqmzmzwll.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/grkgsjpbx.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gkztmbebz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ggowoymco.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gmsphjcrn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gxmebuccs.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxudafzec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gctukmopg.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/glnrgodmh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gabdklwga.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/grdbvwyhb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gmcljmuez.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gwcwzhamt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gtcjkxtvi.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gliioapnx.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gulyojhqs.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gxihexuvb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gchlqjsxf.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gcndfssoz.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gkzwgtnjt.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/geujdigwe.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/glckilphb.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/ggjsnelar.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/glcxwuspd.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grybbojio.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/grfialgkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gksavxdyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gomfijvyf.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gsvxrlqxg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/glskwslsx.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/giwbnupao.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggbxcdizq.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gatmfflar.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gesgaumbw.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gvpsnjgmu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/ghozyvbva.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gfaicntqz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gqrvmedex.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gayjrycoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gqahbivpt.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gyvekzcuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gwjldsgpm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gbdzlxjlx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gciiuxtkc.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gelkwnvnt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gwakahsnj.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gzhmitkrs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gqemfigcp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gccbssiby.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/govrpmjmu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gnevtgzgy.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gioppjhqo.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/ghrhvybxi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gdkqgcezj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gjzlpizfd.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gyyxcqoaw.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/geaseltqp.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/ggwisoect.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/garpckvqv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gfshkvjal.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/grrzjlwrp.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gmzmxlohh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gbprwfege.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/glxcedcrm.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/ggixodjzd.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grhmenzno.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gnfkpquog.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/guqxbvqmq.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gwvmjgsgl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/ggooaijiz.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gnvqwfybq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gixftrrtw.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gevqhhdaw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpgiggzed.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gysqlopig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gijwxdcbw.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/ggihwgslg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvuiqvdqx.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/getvyvxtu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gzjengwos.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gipuqmwcb.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gnttjkmtq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/grsnmpdxp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ggsxvpfin.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gxtbkptyf.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/ghttevuiq.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gpqzbbbke.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gjqnzzwoe.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gpnsilbwl.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/grfbnkfmz.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gygcynqwf.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gnmnhosap.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gdjkoqdip.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gerlaofck.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gdnekucld.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gbardszzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gacpdrfqi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gbxqzpzhf.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/glyiimvih.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/ghmmngqmo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gxesbuzon.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gbssjdjew.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gopkzyfei.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/grkknonru.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/guykttuji.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/guffveype.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gigspdhft.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/geedwfowc.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gweuvyejg.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gbuhinjyr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/grtggxtrr.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gcrisjtqe.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gxnxqsaba.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gacimphan.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gtygxsgrk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbdpamx.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gxdjhmuhd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/guyeldrit.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxexsyjvi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gnwggijuw.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gbjcmrxlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gmtecbmfm.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/grrkhinyt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gkyupwxgd.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gnddxgcli.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtwxenefp.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gcpvbocbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/grlajffaz.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/glcjvwahi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gtgtgkffx.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gromdapgi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/ghwzknhek.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gprobuymx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gmwpgroqd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/ggunganbk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gzigmrlud.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gzqetjppp.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/glltjfrtx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggedaemie.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gaqbuplrn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjvuhjywv.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxmeltyvr.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gvzymruzc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gztmldxys.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/ggvltapra.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gkisfbaey.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gbuhkmrbv.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gjyvgyoqj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gioyqshou.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/ghflflvne.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/grlilbvxx.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gvulssyvj.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnfxqosuh.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gijbhbzvc.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/geyumlush.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gputdupxz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gtrjgyokn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/ganlmqhqn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gmpzduyzp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gribjyhjd.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/guavxiwum.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gaqsfdafp.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gyecnreng.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gkwnefepp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gfljyvhqt.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/glvwlqecz.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gxmmnhuxm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvayyfgri.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gpiuzydyj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gwjsqvarb.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfepbfzbp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gefonyfzr.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/goinofotr.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gbgsxuhaz.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gddnzznzr.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwflfglk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gnosxnvkh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqimekdi.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxekutgqw.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gujnnrpgc.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gchlymrzw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gngmlfiin.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gqodjbgtz.sHtML


<!-- 参考信息 -->