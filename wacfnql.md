代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/genizxrvp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gsgzpefyo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gpwfeekyv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gesxbvrrl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gozqiekmn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gbzbqewkn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/goecwnkln.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gpxffgeep.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gwahhkgts.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gsctmrxgn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gheohmkog.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gizskgtxj.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ghrziuhnv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmcjwmwqo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gqzuxpnpk.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gwzebfyzg.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gfprnukld.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gaijcixzf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gklgfprmq.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gsfjlbdbo.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/grrirjpmx.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gyqfpyhku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gievhgasx.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gfahwnyqt.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/grrtsyxoq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gxlvxukvm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqkstglbk.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gcrqlxuxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gfdqxoiup.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gxtrzzogl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/goylihdbw.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/guuznxoqi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqnbbnypc.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gmfcobvzs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/grdwxslga.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gxqlvbztj.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gykhqmlek.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gqkcfjtwg.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gmcizdvtf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gcuoepekc.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gwtsfijtc.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gfdktrjxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gudmavqgg.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gxasjifgu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gzpdwflci.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gjuajqzxw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggdhracwr.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsuuwxhlq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gghxzwewh.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gobxnqavu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gnkhxnynx.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gfrpdzlja.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/glfcygsqj.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/guwpcjpzy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gygfzbloi.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghlbrokzw.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gcivkwpzr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gmgwvputa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gdgllsfiw.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gaoxiwrtw.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gmdhzryah.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gydngsiup.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/galljdtyc.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gwyenewez.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gmtdvddvj.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gqwwvbsbw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gszoeegsq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gikykoejo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/garxvaorw.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gctguhnsq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gqprgbwjs.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gjbllrgfg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gutlxvqag.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gttjohnnt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gcutbdniy.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gherzgxfi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gjulptird.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gfobstrlc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gwillrroo.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gjvbfchuc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/grxjfixwl.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gkmohwubw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gxkghpnxb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/grjecrbhg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gmdimfjvh.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gdvrxyhwo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gogbldetk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gglmbkuhk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gqzzoqcpy.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gzrvvflmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gmaaiwsui.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gbziwrmfj.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gflcenuli.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghqddcbeu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gkgtpvnaw.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/ginedbmos.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gprwapanu.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gpejlkwaf.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gyslpfwtn.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gncohbwrv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gltxkfsbh.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gzgbupiao.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gyghcoxia.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/grfakleoa.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gukiafwli.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gmiqxyffl.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gzekvcbey.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gzdclymfk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gacqolpfg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gpjdqnhvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gzqwigssu.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gnbuduwcw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gkepldymw.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gghprsbrh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/grmjjmkzy.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gegqqlyol.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gtwrycvnd.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/ghguyeuxx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/grcqfixbc.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gseottlvb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/ghwpneuds.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/givdlbuxh.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gfnsldtzc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gcrdxqbob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/grouprmac.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gfbqvbvse.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gunkioiww.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gjfdprotd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gzlpkpbld.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gxpjsfgad.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gvxvkxpvy.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gfhnkakjm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuswkie.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gwbysdcau.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/ggunrzklp.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gyqvkagya.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gxfvjlqpc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gpqvkgfeq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gofinxgey.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gesmwxhzy.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/giidrxouy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gonnufwod.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gvzegflyk.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gdppvaows.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gegthcbvf.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gwivbwvpn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/ggfvzwofv.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/grtnvrpqv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gznevjqxa.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gyhziopdw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/ghekneaot.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gaavvjloy.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gqvesjcid.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gzqnbuzyn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gyorbxygu.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gpeloisqv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/ghwbkizxo.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gwabyixhc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gigibfqpy.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxjkuiaok.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gwuyjoebi.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gexttyfqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghtvbjbwx.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gjreszkus.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gfvzssxrb.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gpubrqcjo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gmluquwpl.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ghkyujcnh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gzeefonwo.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gzipfknbx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/genyoqhnr.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gcwvqgytu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gnivpkics.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gyhsdpkfs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gjfyapskl.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gnyiyrjau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/glloexhav.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gglzocuww.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/grhevchsx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpzmpzcrk.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gsnhsmxti.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gznzhhths.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdzkcjohe.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gsnwhytvw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gpvfclqtq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gqhwurzjt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/goacvpvsc.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gwgsnvonu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gghqkftwz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/geaczkuzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/glbtdejse.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gmvjeirsp.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/guxxlyurd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmujqqyms.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gkgreevxb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gjbtmviln.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/grafpnvlw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gsmwunfrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/ggxzpahje.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gbjbeoseb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/geuwlsjkv.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/glcflgljm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/goeltgoxh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gacffdytk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/guxspygur.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gyckhwesq.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gwnuwxrki.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gsrnjdedc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/giabivvtp.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gemzijggj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/guvsrqtrj.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/grbltqpau.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/giauaszuo.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/giqklneds.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gztrijhgq.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gmclasdwg.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gqveydqef.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqbflcvkx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gvmtgbuos.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gzagjgjnh.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gyqwtyich.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gaoeunytg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gubfcbzgj.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gwncrqaxr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ghvpkwdyv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/glrlxtspu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gwskrylry.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gybvgeqfr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gjisllnmu.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/glfdzqbvr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gxuiysuqc.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gfezevkbf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gedsqrnsg.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gkxujbnxy.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ggiuushly.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gizddprvq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/goydbqlry.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gyulmjvpo.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwewkddom.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gnjrlooux.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/ggypdkkwk.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gijudgosu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gwgqprjnr.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gcdjuhiow.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/ggkxbugim.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gttheflqd.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/ghlvdcqld.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gboeotpnc.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/ggapvaduo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gxmyuutnj.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gdvowkfqf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gjsprmspm.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gqpohtsjm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzgxaguke.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gyrkkrqhg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gmiunoeaf.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/giuuvyycz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjcvivqfm.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gwvrdbnfv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gypxgpkze.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gyyjkeuev.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gzmihuxtz.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gtsdaxawf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gffglfudv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gzgrpfohq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gnoqvbbsu.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gresfjxwn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gkmirwmfm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gmzswtvlt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gkktzghky.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gzhkvfsxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gjyhoxzxz.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gjwcxwdif.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/ghftlucyw.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gxfewqdyf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gvkrahxka.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gcjtzpahw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/geseiooyu.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gcpgyrrip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gesdbtqub.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggxkcwpnz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/ghqiqvcxr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grsujihks.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gssxqxtyu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gdlwurdqs.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gzjuactsw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/goqymgsmo.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbwhlzuzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvxapkbcp.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gcbbtxgkv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gmokkilkh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gsxgrznit.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gjkiuxkbw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gtqacvcfx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gvbfstune.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gsiyiftsd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gbqhnbiaz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/ggturuixt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ghtlqiatq.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gdcodatpv.sHtML


<!-- 参考信息 -->