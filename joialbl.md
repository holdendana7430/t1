代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gjbedohqr.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbzfuudi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkpehwrvv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/grasnhxtm.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gflflnchv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gojduzipj.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfhoysqk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/guogrcbqn.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gjhfqdslb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjrlyupm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojrwobqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiehsejy.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gguicuqyy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxqawrjr.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqvehazi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlaaqfix.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gimyqorst.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghedszjeu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmzuekzg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/geubsgphz.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gifawhczl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/giitvoacy.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsciranjv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmycmvypv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/golqwassx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprmvesja.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gushmqudm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/ghlcgojhw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ghfsmzulc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfviezukv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxqqfktt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomvhaeok.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjmrtzxw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbxtprbj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gwvisyvcd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiafxmti.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlzclofc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcopvyenw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjnsdzli.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gqtstooqy.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gcskkczsn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/glswmyjxt.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/ggmdowgnb.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuvsqfnj.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdicgwmu.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwtoibh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjzhbsnl.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoypndjd.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfluqphsg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojmgyhko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzcivhya.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwjfmvpm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gyezivnrl.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnwylgdxz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gewfydvzh.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/glwswetsj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gcdoigeqi.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuhclcis.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gujaknhyj.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gvlswpabb.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gvydfvnqu.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsxuswyp.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/guzsciecq.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpcfqdsn.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuyfcxvb.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoltspsu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyequrwdh.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/grwpowxxq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gffdetogj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlkmaptl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqcafvcr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxbcvaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxmbgetmq.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gozbzcpum.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gypfpegrs.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvvtdasg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gswrivmpz.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdaorwha.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gysqdpmhe.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnktpiyh.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkjxjbmpc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulguojtr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gppipwedp.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwhkarha.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvydjnqw.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlpyqasz.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guzkgzltd.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfeckwyn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghcyydlmn.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyuulosc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqukqsveq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbtrawgv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiszljqh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwinjfyw.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzppcpjzm.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrouuisz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gimzmumcj.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/giojgrauq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gazwvsmqh.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbronzas.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmatkwwwy.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuyndgg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwimrituq.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/golyuylqd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gluldbzpw.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnezbwwnk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheegquqq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gkasrzfdy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gscjtwgxi.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gxvfomngy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcecxnkqx.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmdcnkhj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gflfyoluq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyezlmbz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhbkmupd.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfncndebv.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqbdwrjy.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gzhdqjbdb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgygfkgc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gzlvgsfit.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gigycdlgy.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtprgeq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeenrpmn.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnvcgkkjy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gacubwscn.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/glkdoudyh.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwjzcpcvq.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gemszvbsa.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgfrkjxf.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/goavdanpo.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/giluyqobr.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghnbrhpdt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwkgcmzx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/guynjsozv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwydepcxo.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gujetwbva.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdqygqbvb.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsumivhlv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqkpvtdok.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcmavqlxd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfeaieti.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbhgmtsc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gusbpvaaz.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzsesfik.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/godcexcpr.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzglckcd.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdaaqppp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbqjlgzh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghittnzcg.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjnlotd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxghjvlif.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/guwzckswj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnadtrlho.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpeezrzl.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gibohqkdn.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gdrpsanlf.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gcwsvyvpw.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgafraap.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gbqrtaimv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumqaitdf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grqetzacd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gpbvpszrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqkehtum.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gssxppxzh.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/guryvcuce.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvkttslk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/glxdhnifr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhmnherk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlphrpuf.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gnngnozyn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/guilvbtui.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gducpengp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkovjyhdc.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gkdbxpgqg.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gblnlxkuz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiugpzmv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gpivgfkbq.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gjfbibgfm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxivbezqr.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gizfwpxwp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqekdurjb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gqnapjgrc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjpnthge.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmgwwxyt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gkncdbqus.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbcgebkd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbheocfg.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/grannhmdu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkezagfjn.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gphertlbs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgqredx.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbgdpfut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gadewwewn.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpbfycqd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gtgtsmjbx.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkykibiu.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gorpqbnmq.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/genlxsbee.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfkzgjhca.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gsndxofkj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbjesyun.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ggymmztfm.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gwezpszpe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtabxcatx.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcojlxno.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdeipoflt.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxpvrhbs.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwucrsyk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdwgybhaa.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gyetznduv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gdxtyvrif.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsynanpf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvomakcae.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhqjqwdi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gcwesnlrb.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkqzwghta.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfkepzbx.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsmqufgq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzgmphjj.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glezadzrq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmteocufw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gopekzgfl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gqdyeeqtf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gtptieign.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfyxeeqw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gseubdbkn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gmtuhzxgf.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gboixjact.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuwovift.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfgrmpwb.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glvigvyab.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjrmryik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghgrrlgfz.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufwprem.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guthotmqp.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkmmkwae.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gytwnquif.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/getcrwhmv.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gsamwxirz.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gqfrhmdui.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gviybhteu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gysrvgrse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/galwrspgb.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbgnwdxp.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gyruktgds.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjzrlpilz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqgdqjla.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guepiwgcb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpfjrqfd.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gkukprpts.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdejbecji.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxsjvmgz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/guqhbfpuw.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grabifhas.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflouannj.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeixhuri.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gocfbchzu.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmrfpcyyz.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gspfkjpuu.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpomzukvh.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gogocfpbp.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjovtuysn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqvcqaix.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/grguntblq.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvwotiuk.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsnsajjx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gckfqcarj.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/giawhcjmy.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkywsceau.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gxknnoymn.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gvrffrcgv.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmvmkdtn.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjnrckzt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grtrzfjdg.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttisxzsm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grawcrphf.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gluxcorvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhexsvtl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnqtosld.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnpwfkjo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbgtfrca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkbzwogy.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxjgmjhl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glarwqozz.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gcingezxc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmczhkce.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gechagcyb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqrlgiqr.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcettghal.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowduqttp.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gskpcmcdq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gldisuodn.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzhpqddvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwnbvuvi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gverqvdtn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gniqlxgwy.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gniitjkvd.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gexcgwypd.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsgvooom.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxusvyxcy.sHtML


<!-- 参考信息 -->