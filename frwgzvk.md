代发 wailian999

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/goeecdbok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqbonspwm.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvtimie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgxvrkbd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggslrrzpr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glaifynqx.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhsrlahv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glhxoclxf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyxsxojk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjcijbbqn.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gtndglnxn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkqhgdua.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyzmifup.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gcuvqbbfw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmngarvxi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garhbrzbr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gznmvuccg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gojnugpvz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyshkeiwa.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqlgmcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gbjmiodag.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gnbdjwuri.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gppqxfttr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqwvdjqvo.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvjegmp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvgttvdk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gomvetekf.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gkfqwioer.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/ghxifczun.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gsfzhbvlp.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/govnxcjad.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/grcwdgjcc.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnspwacd.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocluqpmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwmixpdf.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycsdnlej.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/glhdrgkio.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwpiookax.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzoatfcbw.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/glyglmmhu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdlqfplrp.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvjjpkslw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/geahscmit.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghyzlhlw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawpxuvz.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gllkgqdmc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gykomaish.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/grvfulxrr.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzpmbtsw.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmovprpj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtftgajzv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggguiewyt.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gspffdtsy.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glunyzvyy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsotboxef.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlkvdwlm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glylamrwx.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbwyahhq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmytqlanc.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gamddupof.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glkqrwkvq.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidsocuas.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzevntet.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gmithqtow.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/getxtprgx.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gaedpffvp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkkyhvjun.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsbrqvlu.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkguovylt.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gneofhcay.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnejqovvu.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxjhdfsbs.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfkqkuvt.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gnuthuapp.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghlhqmsdv.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtjauyvsu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqzfprlnp.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhuatzqy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhzwkxg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiajkcvu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqsixjz.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzwwcxydj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxrkxivd.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkljpsjoi.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/graohbttt.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlksddcw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzxhserv.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjazxllzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhxeauht.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gifrmkgfp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/glvywxbtt.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflcoojsk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gifqgwjls.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/goljaivwg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglmuepah.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehbxpuid.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfyrgqlo.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsxhkrpo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlaqwnfi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacrjpnsq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/ggpctkpae.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfyqwtei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/glumgfiqw.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqnouhcof.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbwvyipj.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/grxecsmis.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gloyctylk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzpufzfx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gtsllwbwz.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gacrpoyus.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glycnwjbi.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiqzqvby.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghokxxasr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golrvcigv.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grbigcodh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpvjizbo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkngiytnk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkezlpeo.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gwychvjgr.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfzfcjqs.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/grhxcewps.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxoykcms.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkozksxx.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmghumxvq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypxequng.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ggisbmwgb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/girgrmjee.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfuhwyqnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gosnhjhtf.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gqawhuwqc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvrwddhy.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gmvcviand.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqclcrczp.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbwmkxwg.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmfvtszab.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgljjmaq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmmefqnb.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gktncgngu.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glnqhajof.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gboadnqnn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gvqqcuhfg.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjppxklpv.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/grjrycrea.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdtnkygg.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gedxtnazm.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsucfuqwv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/griyviwkr.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyuaelpk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gczjdrzdc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaucaomo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/govrwdhse.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gplkcdffa.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/glgobhcih.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfatzmmb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpspcpbie.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/guwvwabzf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbrwveri.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvfyifxwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gwerlrovu.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvkyxafe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/globdwchr.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gpgpslpai.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyicmcaf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmenecsso.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwqoizz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmmetnjo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsrovvxql.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gedkdyfbn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gtvcmqkqo.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggmqcywri.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxlgwfu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gytafsjzh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhewmbfv.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gavgzllgl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkoygxnj.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbkrbtv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girdbozik.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgbjrvfg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwtnbhce.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gihlnffjp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlowxhkx.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjuktijy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gghkdolpl.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhkxninu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkaepmoi.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/goawbshwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gprnvaqfl.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/ghljsiuau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnhvliipn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevkfxdza.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/guoudkjlu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatskwfsh.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gzzmsikhd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlkxobqi.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmuzlgimu.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/ginrtcacg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvofkvnmz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/grbizrzur.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvubvzcmh.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gjjwoyoem.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/godiylsjk.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdahxcvve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndtqeas.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/grujdllzl.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddtlptjx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyqafeti.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/glseqrhgi.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gjvghxujh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gckxvuwrj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guufppcbg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbppugvj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/goovuyqeq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gsulvgbkt.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwcaibgh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/geqtihzbp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhsxxzjq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeobuucp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdwodvwl.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gazuwrafi.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwairibam.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvxwhnwmu.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfyfsnsm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrjtlhof.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxectdhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gchhnuuwl.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxluvvweq.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gryqqlulw.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdasemnzh.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvbnccwn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbhfbyrnk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsdtdhla.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glqmigwse.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefdliwod.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghvmbyyhf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzaejozav.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gcnhujdmn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gikdeddtp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwoycooo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/girhjjgra.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnynbfcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzsnsnyh.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyhvdnfb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqjvwgd.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtoxwmcst.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosyqgnlf.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgpvktlm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhxxzzpl.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/glxwfafze.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmacvcrom.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/goridetmi.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwbimoqxe.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgtygwic.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfrxedidt.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaghgmsrj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gxpqvcipl.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gpvriwheo.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbokjquhz.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuystvnd.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbiorkht.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gghcfvhrt.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyzaemfo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfspddag.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzcqeqwt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gbeetzicp.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gvltcoaob.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnrxepim.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/grtdjjfow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjecipntw.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjdzwtcx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gitqvcibz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gioebfewq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzgpekke.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtkstblk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcibcpqia.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjpgnvnb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkottpnva.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgdynuzn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/grgprubvi.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpyifxys.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gppaepefr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcabmzppg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtikmecmb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmqlvshdj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gprficbqr.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gehwewfqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gsdfbxlel.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfgbgtur.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtopvvlhl.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgzvxaka.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gftxpgrga.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuptyziz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzumxmnh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgolkskj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghzofxkfm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggtwivofz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejidnojw.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gookjybqe.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gorwnvmrw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxxvfcba.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfizelhf.sHtML


<!-- 参考信息 -->