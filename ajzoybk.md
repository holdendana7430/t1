代发 wailian999

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gihpiwsgm.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gmiejfjyo.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gshuuqtmm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskvjklqm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/ggruvidbt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gusupyaum.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gxabzphwx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/greejofwk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyqurgdp.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqwqdnua.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/ghwcjdmwi.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzxnvomi.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/godnlfjwp.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gfhxpnazh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gxdicxoyt.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkcyfcqp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwsqqbjw.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfbeelqm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqalnubxd.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gkzvnimlv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbawetfm.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gahvypnri.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxisasg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggljnumcr.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/grhklnzdu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwsgdtoz.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxszdbkz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gxscedcbg.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfdlbotq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/goxikvqma.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gedmssjkw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gkojdemmj.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/glygppadr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmdrxiqvh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatmgkxdp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsktrbzo.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzhvqxcom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gorziihwl.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gccovacqj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfeipmolu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/glotuaiot.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbynehlbv.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnuuwsc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gepipxawm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnpknbqp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gkpnixvuh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjorpoi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzqrjelu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfxqyacp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/guktrjvvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdrwvuop.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gesfycpbl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvbuyhvy.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gqxfewgza.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjxlhjiz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxldawekk.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjoxpbvp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvltrlodq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gloeyywfh.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfnwyft.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpqewpcv.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfwafhgs.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkogtzxvu.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gosgethhx.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gefbtjjug.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdwdhidlr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gavljqgaa.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqmkyiyy.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/grcodeana.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gyethyrus.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggvuflvrm.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdqbfjeiy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjlzxwjs.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gcowktjrd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gstefodmw.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpwpiogz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gatwwmdor.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghcqnnxcr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gagghmkpm.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/goiwcttsr.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gqltobkjn.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbijsayrw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gywnfcpsz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxqaktnz.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gybdomije.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/geqphzfxd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtulczmzo.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gcqootmoj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/goqxvkzgw.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gdhlghsmv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glpwdopup.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxquodis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojmgjiy.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwimwpngo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbqsdqmfu.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/guktfpspa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glvxkxnfv.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gtolbriqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnrdkxjb.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gabpekaja.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdzuwnfm.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbpmitz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtfsqpsj.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gexpuiasz.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grcejstea.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerpztpqy.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gryedrxrf.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/garrlelwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqputtd.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjcgsfsi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkfqoekj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gazzjbjrt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcbhmsyd.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxyhmhssv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnunkzed.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucihjlxx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gcjqlnymv.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgsjmiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gvnxgzlaq.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnpzouoay.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkiirkpj.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gytvgnsly.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gieyxpxbx.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glcjexyah.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgcouzqe.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gmctlhdvl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqquoxiek.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkginfqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfroetmi.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gdxaosrph.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzppmxegw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcspkuub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/godfokeak.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/guvwwwhzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gdggxcpsn.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glavlrmba.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdvywqje.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcjqqkbn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gghssgjhd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/grgsgspcn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvyikyrp.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gignaooca.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixfakjov.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijhonpn.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gozarupzu.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbyfsuca.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfafrtnt.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gphbsqbri.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpobltcz.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gsumlzmqv.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpwubrqsw.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/grdpmkzhu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzorsgii.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjubgprfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gzqkuolve.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvltcvzwp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guqaweqmv.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbpmqtrqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gooftyyhw.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvzlegavz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplhnwyqr.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwxntuu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gitkrqqxv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkiezpvq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gugoaiuws.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gqbhtqkkq.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkawnhdcs.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbwrxkto.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdjfvxnz.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdigouycy.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeperlca.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gacngezrr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/geusdbzxh.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/giizjatcw.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmxjjiue.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxyjunej.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaniwxqv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhpigbri.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxdqmzq.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/grkegsgsd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gcmlvadip.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmehxgdhr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfwixqsa.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpexksjgw.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzghhocln.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduebwvud.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gxyicdynn.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnyocwypw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gzyaztbot.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweexvmgk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpxiiewl.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmjwbdcec.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gcgqakrdi.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gevmqrfpd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojmeldyd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gobemhnnz.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfwglqdh.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gdhofpvix.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grpnkhogc.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqzgdopg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gipyvcdaa.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gtejoqzhv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gbqdlhjkt.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzppbkjxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gylipvkab.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjacyowi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghgiiqqsu.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gygzcgddx.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwcwzcwd.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbicqjol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuexyhjv.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grromblew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtylgnieq.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/glceufcwx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gryjpgbfb.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/grxieysnz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gognqdqjz.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gsztqajyv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giacqandh.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gffnroiwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfpalsnwd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlnveeys.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpcccvjo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gluhatark.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gxehavtya.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzwhxnls.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvztifnx.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gomzokwsh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcakuzgcf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gciqhjwcg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/glmhxivtx.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzjhllbb.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/guandblrj.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gkiqsbyez.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gidodbyhe.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glckmsxns.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcejivkvq.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guhayaztu.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/grlejqkuu.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/grsomzemm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gllhauvva.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gcughsqfw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghapcuoqe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gjtgznjdy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/glfnynwut.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbapbpevm.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyzcuonn.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhpxqmsb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gghtvjbfl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gypvvkwza.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqresgvq.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqikibrow.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpfdqbvpk.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gagdpfjml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdloriev.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsteqhsn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnkiwbau.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqtmbugl.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gswrnvxiv.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/ggplhovby.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtunuolbg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqqrnvgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gvaegfszm.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyolvcuv.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzvpytev.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gknwcuzhk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlgveuqg.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gytuzsffd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlnuomfc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzpeanvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gvlucjghd.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvjzotdec.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxutlvowm.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gtnbgerfj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwecfurrj.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gqhudsvlx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/guhwczwbi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvplrcglr.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqdhitxr.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnyqsosq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gypmaktzd.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwmvjpcnj.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajfvvfbc.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxklulwvf.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvztofzv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjygjvobv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvbzkrhy.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gztfebrcg.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnrcokgc.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gdllgzhyy.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gmriytgfm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidifzvvn.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gteivgeai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grngjxquz.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grqalgndv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxexgmfvu.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gluzzdevg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmprzljdh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gzyhutuei.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsyceinc.sHtML


<!-- 参考信息 -->