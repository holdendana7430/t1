代发 wailian999

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gjdccvvpi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbacdisyq.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gmiuehmhg.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbztlvjgu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkauwtnpp.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/ghstoblhq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjykokkt.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gvthzbhep.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gstzpgblw.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwzuggdb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gzjphpnnn.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glheevxbc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjbttcxp.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gietrvjfs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gnhpslpvx.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjtotmwc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/grlzhxdoe.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzienuntz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gglunmyff.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyzuqhmu.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gadtdjppq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/ginpihpft.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnatopdef.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gydihacaq.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvzqnqgh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/ggblgelzn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjidyjbjt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gkojetynx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbobiiyh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gazqqgkqk.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtxarauk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gupbyplji.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxguynzq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibjgppmu.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjvqtltf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqwzvmlu.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtbolhth.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guwdbgbfp.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcalgggj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/genobmkea.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacpolnev.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/giujjdmmg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpnuizwmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzacyovb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlcahgvk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gkcohbbus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giydidzxk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsleuymqf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gysxfitbd.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gbzvalqae.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvzxnznh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoqmtcli.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/glynrnuos.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbjjwpze.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gordcrhpl.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvxklylx.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gnptglfjf.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gpirwjsgs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcixnhiv.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoeszfgf.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gunarqkde.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gehuxxvuf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/glevkcayl.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gazicfpnt.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvzpnbrl.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkagwcvsi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocnnxrlz.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhpvslz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwyqcvxz.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfzoubwsz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjblcomxz.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzpdewujj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjjutcux.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/giiqllrwm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gjarqjwbd.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gyozmbqqk.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gkoqidhfq.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxcxexvr.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvmhgums.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetffgwt.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gemmjtzdz.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gakygrquo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekyvnqws.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gecsklitz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyjdvjcy.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvmzxiqf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavjgxwyu.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gybfspruv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzljvbwyu.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjkyafwil.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gspmvxedw.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuxduaqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudqfcknm.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcxaewth.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/groptoqjs.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gypsgrbvv.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdobmvxam.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfluzerm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyopwsyt.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcatqjevh.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gizbbboiu.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gslgbllkq.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnaunkdlu.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvywwoghr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjuebgeeq.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdevhxpn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokzrsly.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyvrzvxi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gulyrqdnn.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsrxmbicy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gqvcdkuxi.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqeqpsbq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtozygc.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvgusoyx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gatcoascf.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwucdwwbr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmusfbmhv.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gozdsysek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapdmnofs.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrofxkpi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiinaqud.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnvuaeqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gomcryilz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuwlbdhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gxumwmvlj.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixnpktrs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgujypku.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvittfcdm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gscunxxvo.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvbhlbgcu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlqecxuy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsbqwznl.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gitjwosxa.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdriskdj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gfdowinfa.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gathpidfk.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gmocpcgng.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzgnkmdyq.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gxxkbtpeh.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxtorwysu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gituxdbft.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxblsjity.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghuyjrhmv.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbzplyova.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbjicvuj.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxnheiwi.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gldckuwfd.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gyxwkxdzy.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirhuyhn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geestvvtv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuhxtpbn.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgobcfxf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcflqytoi.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxppeqpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gycotcavn.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmtxoiijb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/grwsnqlae.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnyhjbvn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxnqaphk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gornjbpor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjghtbslr.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdafrqjt.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grovomaey.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiavhwyf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwfabkn.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkcgglkmm.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqyltbrks.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gwbikansj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpimsnjh.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geatfsydv.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gybrodtmd.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gtegmlffq.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gaberxebx.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmxrrkvoy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwhrkmxt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxwrfqli.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsmxtpjj.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gndqerfkv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gonyaafti.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdznjefpi.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gdjbdlhvv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/glbhufuxn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulrgkbtk.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gixgpihad.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gfkmnfqjl.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbihmtcs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhheenf.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgauwelc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gehrsawjc.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtooedvwm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkahxogb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcfqnolx.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gfnjxdwxj.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjswhxfgw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhsfpzub.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbcwygbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtrbcmi.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtujddwcr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmthurwe.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdlvxsmwd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfanaiink.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdedrqscm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxedfcdou.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxzmjpvy.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gdeuzoygf.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gudscxuhn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gumldqpwp.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gofzdzuaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/geujrovnc.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcshysobg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gflkslacd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/glpoiejzr.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gjqnamlvr.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gevuluwic.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpveracqp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gokzmxzlt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gezgqmltt.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gljhgwxva.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtyxqaki.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmvpplvzh.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmlzuhce.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goxyrbnqi.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gykdjiwgr.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtepsfrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnopkzaf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvudnpgld.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gshoqiyzo.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbntdsnqt.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqoacwhy.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdigeejx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gtskayojj.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/garzoouwk.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gidywczyf.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gobxekadk.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ggudcxkrk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhlzqkav.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gvzsftbpz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gojcvenrm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gmoqycvln.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gtbmkshak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gayduulsd.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gmgejigwz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghciruuhj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjuxfbexr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gbsktcarm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccppzlxm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmhcwvsvl.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnoldqjkz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhdrnvkv.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gebbybbzz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gvebzzotr.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbatjfgg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjyrxioz.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gtnvfeyrb.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmueuhiuz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybuecbf.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqmejwxh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gybvckngi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gblujcxrc.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwsurqhsl.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gqulkqbqu.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gncqsmcxh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqowpbza.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gshbcrtdw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcvwggiz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgavxnbs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/grzufyvqo.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxdtcdej.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gfoueazvf.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkegkamr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtrhzccl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulmdjeht.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqtxmcbr.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gldixdeck.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/grxtegodr.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjiarffk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzbbeqfll.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwaydtpu.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhulunpl.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gojfvvsnc.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhmukagz.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnchvbeaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbelwiqu.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gpdfxuory.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gsupgzskp.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gbcjihgyv.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/grdlfbhyd.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebjsbrf.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gvinrjehv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmfdvtpp.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbdtdruxp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gipvzqnng.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhccxyjp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhxwjxsf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosstqkwz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/givojxpfb.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuwxswru.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gkcqcurlz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gifrjxbft.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmldnibuy.sHtML


<!-- 参考信息 -->