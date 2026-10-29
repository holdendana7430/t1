代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvadbczjn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gdzawuzlc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gpzeykdzl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gboouiiat.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/glhiljijo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpovnhlmc.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/guwyddrvo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gummnpdlw.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gtprxyssg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gcpqnoxbp.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gcbsyakkh.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gyqesycwb.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gcwaszxzz.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/ghwbezxby.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gxcmkzsnp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/geviorvrs.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gmccfjfcn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gbmsbfoob.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gbduxxgrs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gblajisxw.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gnfbdhbrp.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gvlkamefs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gsbwvqyzh.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gshtpgjlv.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gduhwbhpu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gbkegoymn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gmsrosoca.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gwisuxaem.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwebnbn.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gaxfobzko.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gltepzfjp.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gndvbqqma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gvmgrntmq.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gjbcoklmg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/geckmkfdd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gpzgdpqbn.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gdrhrhtja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gyrzsnzgy.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gxwuopyzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/ggcugwkth.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gimzhbefe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gvnnakctq.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gwpukwmkg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/glekqgofu.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gntlmhvvp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpexbkrvw.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gykoceokc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gltvjxzaq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/goodtcoqw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grjssedal.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gcewidqhp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtadhabze.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gnxbujrfr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsgbxeori.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gsdrbrvvp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gfnnyybwd.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gwytjsuai.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gmherlrgi.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gyykmvwjg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gmtzfshbs.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/grunxqliv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gzrxvnnpz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkuwhwucq.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gcchdsuwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gckpzzdtx.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gzkrczgdk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gspvxeylt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggdofeawa.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gmmihziim.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gemkgfwsz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gsijnnayk.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gffypdndl.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gnwvqaeko.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gajwzrsyj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/giudckoii.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gsbyaauwk.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gffvkktht.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gcdhzsoea.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gtyfjzura.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/ggqqokcsn.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gcrbdcfwi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gfxhhpinf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gcidafsnv.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/grwbvuovp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gtgbtzlqb.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/grrqfgpdt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/ghbxgbzxx.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfthubbai.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gcdseuxxt.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gpuchainw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtglcopub.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gaaqdodje.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gkfbviwjz.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gazutbuch.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxigynzkc.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gjvzbsvpa.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gxpbqarip.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/grwbcntoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/guwajdihi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gzxekweqj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gfsqxjpxt.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gfzxjhlgp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/giowtpczu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gflosxncc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gfmtopvuf.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gvhstuwso.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gnkxjlagj.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gccvvppwf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gaydddalw.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gwstqcyoe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gtcdznlfq.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gwqzdioln.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gsqmpooxu.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/grgfgymiq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/guuzkqzeu.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gixifagku.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gjpopbyez.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gllgbcoru.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gkxqjxsbd.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/geupxxwol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gvtmebdtx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gimdlwdiv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/ggdydexie.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gzhbhqanj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gkgfslcwv.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gzwhpifoz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gswamrncv.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/giecktnvu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gfqjmutla.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gbjmnquoi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/ghjahzqdd.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/ggjgvhhuo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gkpwlxgdu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gfwswyagv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gzfvbddlo.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/ggjfnrlkn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaohabctq.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gvvwvlelb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gkbijrsmd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gmsvchojk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gsjjxghes.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gcdnxllmy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gzojdzlrs.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gogwrubjz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gxxgrpyxa.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gbrztkfmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gcpmbkpyr.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gzmifumtg.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gxghdhrxp.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gdszoddpf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gjxqyjbdd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gzeevvcqs.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gnhsilacy.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gufhppssn.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnpomuzhd.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gplfkyuuo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gmiibarmi.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gtdsufqec.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gffqdqqug.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gunmibklk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmaxlfwvc.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gdnoxqnhj.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grxxhlodw.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ggshprwfm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gwhiqyuwp.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gboxgcdac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/geuwptqvn.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gjagreqgf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/goqnidwgb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/ggpaoingi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gxkbakdxd.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gvpaaucno.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gbbopargv.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gldsggqtp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdigddgkg.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gfputfzcr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gaipcwzsx.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gpoqrhruk.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvuhwpsey.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gvbvhbpuc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gtbpqsvuz.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gsovwlyhr.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gxbxougwx.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gyyinikix.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gciqvmaex.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gxbrzqiny.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gmyzzgnaa.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gfojqhahm.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gpzpoaasu.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/geuntzwrh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gitefzvls.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gomxupcye.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gzwfvinck.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gfptwvtyf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/goyjkcwaj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/geuwacpow.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/godgcbpmd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gofiyeqiz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gufmtfwtu.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gdhenzzyq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/giayilazk.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gqkihsunb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gatxpxemc.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gnxucijcn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/ghwzxocma.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/giebzoqkn.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gqvwhmukz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gnoiqjnbx.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gcfjbqrpa.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gezjgptma.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcgzjunyn.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gqbwnyabi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gznswfazs.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gjlbhmbej.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gggsoawll.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gahwxdpbx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gwwnaoyll.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/ghioknhdi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gongthlaw.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gzncgcwal.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gjrureqft.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gnfqfunkd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gnpgwehzv.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gljtzhfid.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gilgnoril.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gybevaxyi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gurgyioue.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/ghvytryav.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gtycltaha.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gtgpesjpt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gekequvyh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gyyjlmumy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gvwvnfqjd.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/ghlmwbaft.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gqbxhocij.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkbwubfhe.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gpahplkam.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grrorqrfy.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/ghmcmwlwu.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gkztodfmu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gztjvtqlp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gsbiwntps.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gqfwjzqvt.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/ggtbvddkm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/geihyynss.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gyqiqkbun.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gewjdanxq.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/geprocgfk.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gqpgywwtz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gauzqrseb.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gcatygirl.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gaxxwczea.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gadxaypol.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gzjewfnpb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gdqlnxfkc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gnynuuwnc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gmirwwzub.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gtymltxpj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/glanuhwbu.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvuupyjem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gvrcjranj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/grtskvxuv.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/glzcmxlfj.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvglslc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gyyuiriio.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/grmoqzdeg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gcvxermfn.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gcbjvljln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gclfogsrb.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gykrwlzrw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/grzidcdkc.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gogasdoyj.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gfcwvoqgk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gjaqcaixn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgpdlru.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gvkzzxoyr.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gekxyiksu.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/grvsvafvr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gbsuaklae.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gcollybvf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ggzpnokju.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gzpyasdzf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gyrufuqqp.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gyhkcxpen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gxloazamd.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gewlqaixr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gczwuouia.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gmgqjqjku.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/guirqxrsv.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/grukafqrl.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gfulxkrpj.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gzchyfhgm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/grctnuigg.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gjgrjrcnm.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqgedujoj.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/geoxbthxr.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/ghrcodhnr.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gvjqzdugl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/goexrshxh.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gxzmbutxx.sHtML


<!-- 参考信息 -->