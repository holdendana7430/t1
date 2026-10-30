代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkgwklluz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gxgvxtgcw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gvltnoqrf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjvoyuxw.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzkqwvmp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvpmubsb.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gelibpjtk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gbphkiaoc.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gumsccudw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gefkxqqvl.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmyrdvdm.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbyxlsyi.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gflbsmicy.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gxltzytoe.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gbednblwk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqdgvxgs.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehawwwqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvznbowd.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gcwbhqxvj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunbikmyk.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/glytxmzda.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvuzdexq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjfguife.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gogxkpepb.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqtzmjlwv.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gnlaxgclu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gyacoxdap.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmuamhec.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwswoelkk.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gmhtbtoea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gbvbquvlz.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxvehxik.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtclayiwu.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmdymfwlr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gellfjpol.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/grrapznck.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjqcffih.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgznedmv.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvvccucn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gisljyqiu.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeepfsxp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gnuyywqev.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqqbungw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoggyaog.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/guwvkqhby.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjmdavnv.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmhghsdup.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gajdepogb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glqpmzhfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmnqdiejv.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxtnoooy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxnjedyc.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjntlxge.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/galuzrusb.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gisflwgpx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/glmzpcuby.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gjlinvilt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gjuevcpjf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpkmwqyaj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/glomenvaj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gltgilhgv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsdcyryr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvjofzbi.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewztkawa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gouxspthd.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxicskvvp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbrwfxcj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmznxzqh.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscjdsgjc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsbmojed.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gcttjubtw.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gjqwjmgou.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gnakswapl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqplyvjrb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgxrbexj.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gevpgqjlq.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gvadwflfw.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxgoasap.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gowkyskwj.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdifbcoy.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzzqwrbdg.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gumbqikuw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixisyiav.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggtpleszs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtphhmno.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/griqllskd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjubvyfc.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gaodexbsg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtztjivxw.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmxikjut.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/golbzatyo.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabbcqviv.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gzpywvvek.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grvbokook.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyojvovq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemnvwoha.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeffrscd.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gktueaegd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxuezdfz.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gljviguqp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhdzahx.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gvenzdrcy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkueyappk.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggehkrtbq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfkqwjyer.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypotpabm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyfukqub.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gogonqhwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhkwuvjq.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gbrffdknf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfjyuhmgu.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvjtkzzi.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnolfsnfy.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gynkvdtgd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxcdbonkv.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmklyyuxt.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqfawgsg.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/goleetkxw.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkgnhhbtt.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtkaopwea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtibarefp.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gikrtrzex.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshvitqdw.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/guoxobzrq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjjfffrnk.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnrujqyn.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gyrnxgxul.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gttfirrhh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajxtklb.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gcstelidz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gseqgrptk.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbgklubzn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibpanvgi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkliinhst.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfiyxyjl.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpdfqwgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goqxwybkt.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvvecglc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxkqgaus.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnwljgz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gslyaetfv.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gkktvxgja.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gxndsvmex.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuwncfvb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gobihglvc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gkycgkuhd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gsluajveb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmmiyqro.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmxmnuss.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gfiyhqgos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuldcldn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpkhsxuc.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gnemfkfml.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltaxlkok.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfeldmxj.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gyppduevf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gulslxhyd.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/grgzzjbet.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glrxoswuf.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkdugus.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gkpsyjltk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqyzypwt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmdvplov.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqpfzpi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gcppcxhuw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gbptfwrht.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsdnsvyu.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqptggvxm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giaunscwv.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gizakpwtj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbpmxita.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiytnpvm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbkijuu.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gcoyhaxdj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewnrmto.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gihhuxsxj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjqqyrs.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvjjzowf.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjhduqwr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmdawti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ghzbigdlf.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gykmbklhn.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvjiqpxxz.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gstaqdopj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gsuurzdbf.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyfrdron.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxnituwf.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjwcyvif.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnmmmdwdz.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkagnyr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcgmqkrn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxedfhdz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/giagpwxpi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gawrxiktw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gqsvcxkyx.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gckmqnfoa.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/glitojhpj.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzecfnqzx.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gnkckdoqb.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/guivffjel.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gwijuhpqq.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwppznfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gihnyhvsy.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/grwaxrowg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdprrcbs.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfnncfpu.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhqsmzaa.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdibnhapo.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gijkrmidl.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrmrusa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvanykxeh.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/ghyyfxetg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtbfmrts.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gifgbhvoa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkjtiwjp.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gokibtwky.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/guoutetpl.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gmteotsac.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzhvciwe.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmmnhjsqh.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gasnybgru.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gombuuvff.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glxuqjiml.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptzdsbmt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoujgaom.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuqdaxpr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gayvnrapo.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gwkwtpjzl.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gxepujtgy.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdvxzura.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoomcwck.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlqnmhvo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gariqhycg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/garhladhz.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gkjjexfei.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxblslth.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gxubbwwmm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghkrrnahw.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrltwyaj.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzqadblz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpjmctid.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggjvxzcia.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjwvhtsi.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaxfnswt.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/geefepkio.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gmbgvglqs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/girvorpnm.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkehctvn.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsltizcqu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpgbpmwb.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/grzlvuasv.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggstmdzfb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzumixfcd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gfquwehsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyjxzkbu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqgpkljh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwjiruw.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gvbwkscxg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiihvvan.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwluxoqsm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/giutrokui.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrfirjbm.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkwdtzub.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddjaxmft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gcifbekjv.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/grnibxidh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gofrgscta.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbwpnzesv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkgqtafp.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmarqurzn.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtczibbv.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdranbdgo.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgkalvnn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gzqwlhoxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvlyghjh.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/giksjspbm.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlbzhmvo.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcgnzbyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gygacviwl.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/girpdjjir.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gjfqrawty.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gxxviqgqm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsgsyizv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgmsmqho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghznvtipl.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfmmizzf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmnswyn.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmuifwstd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtmdpmye.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtvtxpbh.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gdgtfjikl.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gnjdaader.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaupxatv.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/ggijkaqts.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmtkvbiqb.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gphoqnxyw.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/guyxcwhgw.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaazfuiy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsbaqzra.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxujigar.sHtML


<!-- 参考信息 -->