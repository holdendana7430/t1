代发 wailian999

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmyuqzvex.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gujqhnrro.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkvfgrun.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagccalks.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxdpdvpho.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdbebxjr.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gscilvjwu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmftaqpl.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gsguhgfeu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspbsifzg.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gixfhmchd.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gukrfxcyb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwasxpfzo.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gupkhfufd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gxscdylov.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gxfgrottw.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlpvhlvh.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmsyaqqi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gtvpbizko.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gdkwqybli.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphfcjlbr.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gwvkygvia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gpuoqizyh.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvicfqhn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gqxxfceba.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtahddjql.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohqyucn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gklayxcel.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gchpavpee.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpifzeul.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzrknqkm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gpibifpvp.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/guviwqdjl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvtslnim.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuzpxfby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjqmavpw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqurnlob.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzccfnc.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxvagqhgd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubhkagum.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaqruyfj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggmphnwai.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsloklmss.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gywhqchjj.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gkkqulnkp.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gioximtfu.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gvnugjsjp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyadonovv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gtztkgtvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqddtyymf.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxtdhbp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/goyjnhonq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/grsmqbbbs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gobqpgrjy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxclkidnf.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxlhigyxa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gtgfozzoj.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gfjfiumas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhkdmwwr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geavmuhrq.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlagmgrg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvekfib.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqgjumi.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gnlruludt.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjoefjjp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwuewixs.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gstiebktf.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrxjfnxp.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznmcrgzq.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkpynumph.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gcxfxxyix.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtgqgfqx.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxgrsllvg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwydmnwc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmcoazxo.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmzmzofdu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtiagazk.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfwdizgqi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozyvoiuo.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfxhimmz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzkkyuvr.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/grzioewns.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoihuwec.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gxtvuwfbs.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/grnvohrsd.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzsbhwjn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnwcowjd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ggspupksu.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gnhsgzmnf.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjltzcrpa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gokaiepax.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glodiaruv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfiisuay.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlnraizx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gieyryjqc.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmjsyfykd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grfvniheo.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gavttggoy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqkfgwj.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gospvrjwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkmpdaxcs.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gminzkqde.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggwiuptwq.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gibdklshq.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grvlhfjij.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/glajqpafg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbrlgjrq.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/grrxvicuv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/grbuwpxxa.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzgiwjuc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfacjyfy.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfzdckikh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grzkupzwk.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwmmpyxhq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gysjtccxd.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gxiiwymvz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsflvtdr.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/getuvapje.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galmblmkm.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjifkdvlt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnswfrpae.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gazyulcao.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtudcjypq.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkicxbryd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxujstjcq.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gqunsjxfp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwdzvejy.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqiyzot.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glbalcugm.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgweijw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghdvzqxxh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhwipcr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxvwheqj.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gstqfahgi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gzffhrnpw.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/ghskigelt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbvlyrsz.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gwpessuko.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqyyuskh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawmpmlub.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgdhhmjt.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctkjdqkg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhsaesbb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gxubrimya.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnjxapaw.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gcejuawxb.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgjamzwk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnhjuwtc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtnwfjd.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/giwcnyvuh.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gypuzteww.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgyclzod.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gohqktakq.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gpnvumcvl.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfohxgbtm.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gphpzoydn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcutzppm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gempfxmqf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gaupbdslz.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gndnnqgwt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcezglhh.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gknnuxiri.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grzxnhdla.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvhlywdaq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/groqckkej.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbhtmqei.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsdxdxaw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmhguvri.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvugzgyy.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzyzngkn.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxusktbso.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gtnvuchwc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/geogwkqsw.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gixvbtcol.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqloztyqi.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gyduakcly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnqaukdy.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhegmkzs.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ghvqlvhod.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gkogdjgdc.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/grvfiygsx.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghcxycnze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gcgzhxusw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfsdjhel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gasifwyvw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/grioidmdb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gdbendclq.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwunpxjxn.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktquwdrp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcicsstk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gipmgidnm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganaqdyyl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gfxfwmdxm.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkbnohytx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gcuiqengb.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmceaovil.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhhkjbdr.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtseajeqy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaopcjcv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gflupudnh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpveadij.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfszjays.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/goqiqmdap.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxzqvvwx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvvpbuq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqowawcjl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/glylwalxy.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gouwiscai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyhtkecc.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gytunuhap.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guewwsuru.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfuzgjcjp.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/geweryhru.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/grazpqukz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvuopaouh.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwninbezd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/girncihog.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpqnofupc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/guapdttjm.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/guopgszab.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxpjeudze.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gvvnsbael.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmptwhpzj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyptjbwhx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggfarzsqk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/ggvkafrnz.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsrbkjgs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giblqiisc.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/giukkpvqj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfebiwjeb.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnmritelt.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gehoqnmvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gisdcldlc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gymfqoohz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxtecoft.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvqylwok.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gpuylaxna.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/govhlhopc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxajuujcs.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ganconrpx.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyurxqvka.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcppudwny.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrwsfatd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqwnhtqhu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtcvmikt.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gqocjzlky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gogzzjzul.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwupunwmr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/giepfgcxe.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujisdzqb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfrojngc.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpdezoksa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfodrxrq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfztlypvv.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdsorbgq.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdjhvrjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnqokbxs.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhvmhxer.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwckifvz.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghfdipntq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gihmohtnw.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndjomihh.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gffhgiowt.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/govyewbcd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcbcnsle.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxbijzynj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgjtmcju.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gapfuhhbo.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtbatase.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwksdpfut.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gieglkidf.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkpeqxyzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gxklmtyow.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmsajrvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gygriorqu.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjoiikf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqdijthk.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gcnaloffg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvihnuocy.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gprxhxglw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpdqzlxw.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqihbixly.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gfoebxihp.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrswfmbe.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuownyuk.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrfaagkg.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gcerltkij.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grkcfrhaf.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gtmxhhsbm.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzudnkits.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxelohynr.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/glornarda.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gxallqzub.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnazyemmm.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnbcgody.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grzycqhac.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gpfrdcmre.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszonsodn.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gemftehbz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/geeanvquu.sHtML


<!-- 参考信息 -->