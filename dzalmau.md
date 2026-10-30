代发 wailian999

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmozvmrq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gbkgkqwim.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/geossbvgx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gletfzkwg.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gwenneikq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnlgftnp.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdqdnbwx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gyjjuqbul.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gwdsfxxsd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzunwsfyl.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbwdqivoy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqsidzdsq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpzvctppc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gblajbhac.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkakjqbvj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqaatrzj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gywmhdxmg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmowsixp.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gplcfgsiq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjcwiauq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gpcyavkgq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gogluvfqn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsccfvvul.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gfbciilgm.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gwulzhchw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphbtoodw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdxgwish.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grcetgync.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gkkjfmblo.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gndutazea.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gjnidqgyc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzjhjeob.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwsrzqbpd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwjjpejmq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gzwfmpdra.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gkhcvjcxi.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gvtsvppzn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhjrwzi.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gysqpecyk.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjarcakvw.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gsueqffsc.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjhvwycdd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzljfwybe.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/giofugvvl.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjvbtmyxr.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxmzdcees.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunyvzmxz.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyfxeocg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmglplcik.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmlhoxcki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gptbyfhmm.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbntxwnn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjkuxxp.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjfzbifuk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcebucuyi.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gtylpanne.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedroegle.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzlptbimy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjctsnpq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gzpthaxcc.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gvujeqdjc.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyejnhoug.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnxzgmev.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefceagk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfyfbesas.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gijfkfxhz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaadbwkzz.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghlidnqip.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwpqxppn.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjuuysvay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxsumyw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/giubroeky.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gusomzsxr.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gvxcboyeq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqljyblwc.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfigvbenj.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gojiajpml.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiwzebls.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkswlkwou.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfduuyrvy.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmtfwkxva.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjokxind.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmztydoe.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/geilizbly.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gihurnmvi.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqgrzyiqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntryasip.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gyobfxnic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdsmrilcv.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmqmapds.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycqaunyi.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaokvjwn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxzibjac.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiixeybm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxoiecja.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gilrjfxcw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gspxkrpwo.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbruyecnb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnurxpten.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaizurjm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gperohczj.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gavsnvhnz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gewflekfr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gindmdtix.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdriwjjq.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbsypnsi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqijxyu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gackghotf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gomszbmpn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceaovdjb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmwzpogy.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmevblain.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbqfbxji.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gelqebdbp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gkgylftkd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzhbqxqa.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvoxwgpqw.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnrecydug.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwyjymlfs.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoxqghyh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gammchabc.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqdxqbdg.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gppqsjjpl.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkynekkra.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/garbuawcj.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gykpvrylt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjcrelj.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gwzsjxtvx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/glsdbjkut.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/guxiuzzhf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqlgyyrz.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmtubdek.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvrprhbu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawtbvnrh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaorzlhgs.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjicdikb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gdfntdyda.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtleauaq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxwfufkn.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gxhgxsdfh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbnltnlhz.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gheuypblm.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkmqoqzz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gklbonqwa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdqcxpxjl.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpvekql.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnyvwqzte.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoccyscc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gbclvewtw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmpqtjpw.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjeijrpdt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwulyflqi.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/geoqjzlrp.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyysrhvus.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjobgemm.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gloktbuqr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjfpnvqq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbbpisefc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gpmrgynni.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grdvthxqs.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbafeehp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmotbpnww.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdreneask.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grlosteeo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gagvanohd.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/giwneclcj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gddfqbpjo.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcziwyh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwnekaua.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gykprjrpu.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvadfrgby.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gbiilskgg.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/grxvucjlq.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gcjpsszet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwnxxhfv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxypgzsyp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjklbqfp.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrqhzxro.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gergomhjc.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksbisgds.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvhrksta.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gfwbdvdoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoxpmlkp.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvvvvfthf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxdxksdm.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkprgoxd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvfhskvoa.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gowkbfjqx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcafzlfnu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvucgmrv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gcddwpeaq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gpycovfcu.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gedmlqdph.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/ghpltrnnd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzqydkjau.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gdmbjvnxc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowlaufj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gpijpsnxr.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljgtpacp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjpexei.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxnrmzv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnignfswt.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gknjkteav.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gruyjaxxr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvifawga.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdwojjr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gorbtwzoi.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjqdgrpw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/giixowxpg.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvfnqtby.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbixhjws.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdzqovgy.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxgwgmeyq.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gywbulvkw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gznppqsjt.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtexmmzh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gydatmqsq.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpuetqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggztmpbwp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/govbrnvsc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gayhcsrsy.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdibypqe.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gexosfpew.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gswpuuctz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gisjkxiov.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqubkkcf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcsujcmo.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrlndbvm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gohsfheuc.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdectqqkq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/glcfjhwzs.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyxdunoe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gpjadeuyb.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoavdvgs.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjabtulu.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gylhoiqqw.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gafpszbra.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gvigbstfj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzautyh.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkvvovwu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqmuxeed.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/giosyghgh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmxcbqr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqxziagq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grzdixioi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnayxqvvd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdcqjfhw.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsbuumce.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwyfzevt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gavghfhxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gilsnabxy.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxtqguoez.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokbbuzlf.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoeaptln.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gacfatsyx.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gydovuxwi.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gawaewomf.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvxbcftyb.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjxjnvuh.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxvueyds.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpvzzzvw.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gchsmnckh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbrofnnc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdqtsfsp.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbrnmhaz.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gxfsxcvya.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gliriffkk.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gldpxlrhr.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuwubvod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvzhcsv.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuwezxgk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbsyewrg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gadviqify.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gaqkwzedw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gxlebjkyv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjsafhsu.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/glsbmexax.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtgzewcxp.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtirzuhfv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjsdfftkx.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gurnkplny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtkquebf.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpqlmfbi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfxidraz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlxarblp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvylwqto.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gpcwaisxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtasasizc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvmjmvrq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfqsmoyyy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gosvnmphp.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/grznboops.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gvgslclqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrjzlhqi.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/grnbctvoy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrocmrix.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbgmvgwa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhppwchb.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbyfgpvz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzaeifbe.sHtML


<!-- 参考信息 -->