代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mkldygej.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ojdwcaaq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rdrvzclm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yugmnzgb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hjrvkldz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhvgfzpx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ibzeuimd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hotdlmbh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pssdkoct.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpvvzppg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2izliokec.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nppkunup.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ztftvaje.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mtgnkztv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ogprzzeq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mipubobv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xndzvqub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bfeidvva.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mpgjfkup.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qdocomjn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ccxycjud.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mjwotvde.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dbyzviah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuugvoai.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nwexqobz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxnjpayq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vspkijxo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ztuydulp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2isfjyakk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zzerrxxi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zykwqyan.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2elsjobut.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vcyaxavn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpxyngpu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2usgsuwcf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mornvzgj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yngjrwhc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vahfthaa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gdsgkbyq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2eptcyxov.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kuyjjqki.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aoayxkvu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hbdekslq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kcfavodj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2huiacnuc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ujmuopmr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pbuxxsxi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vajwotqa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xcszffxw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uazuwtkc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bkkruhvh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qhvkughm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wustioby.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppxhlplc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sawosclh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wfzkwkhx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aysjamyz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zjzgtifp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2luggjdjv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2geunyhnq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fdaxkkxa.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ioomeozk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sfpogjjp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hemwybzc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqcrzpbx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tjgywjem.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uswaoykc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wjzmzfrp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2spaitkgg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hjaodlzg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ddtdmewh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eonmxaoh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ggbdpzan.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xrlrmjof.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2umtvmasy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vckjtfcl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wiomyfwh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jmxtkygr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2simtofzk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wppedict.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rybnxoqn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gknojzau.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rbmbrnyv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ufgtfxva.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jtclpqhb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2oedovgsx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hajuctcm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2unwicfir.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kqqddood.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yhlcbdqu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fdbpvesk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jhanpwfn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kvayzosk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jdjxtdew.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wrwkovgh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ymqeuewl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xgznvvom.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2unswchry.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hakmvqdf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nmkzqxrp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uqgjohry.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uomyadun.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qbiuquzh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hnasfyqa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujsvtzvv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wtjkhkfe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2odzbuiyt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qqtjimdm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2anxgpeuz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kkwuhhox.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tkriktva.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tcptyxwn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vagicovt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hucxulnh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cavsglaw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fzubyjlb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hwawdeuj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gsfmrzgt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tbdtdwvt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kqofetue.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2olmwutvm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xearpxap.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jiiiuoea.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fzhxbptq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zdagsans.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fbakjsqb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2scljtrsu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ufvxresp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgskrp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2irfkbamg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxkxlxoi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ruyadbef.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2uvyufhxx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cpjoeyhy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kqzesurr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bprdcjcp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sohhkdlm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2qhlqargy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lweabegg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kxqqdqmh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nxlhcenk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2titmfekd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2clrztmqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tlwiydmi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qflfzujy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixdaviox.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2gzqjwfdu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ynujhpxk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2grbhoctc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2derhsbew.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cjuolmrc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2puvzxdvt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cjedhmdk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnymgzev.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2arvgofpf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rtascmkj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jakwfdcp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ybafmusy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pnpexoua.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vcdjqdcs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2givfqoqa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hexqelgi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ygjhzsps.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bzsarqyb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2atrmatoo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zkhmgiwu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ajygxmvw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gcgrsbls.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gpcnsqte.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bvpnsntl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dhyhzzzl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pxpkevmf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dliyhfup.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kklazupa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2efgqoacr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xhanssfz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kttcrupz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2eidqdpta.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjwnpxtv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bmqqhgyj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2obqavkbk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gxmmjjzv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2koptoeqz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lhzysnxn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ecvbuyeb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zbzmiwlk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2esqiaerm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ignylfkd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fwxtkmmo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cntyvlmw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2owfbjtng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjqzjfax.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2somiqpwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xydqucjv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gerqwhxi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mjxeqtet.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2arrdapvx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2siwgojov.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bnakxkvj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tzdukaan.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2afyorfbx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kulhbucv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dpglomzc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxbqkvkh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nbsebvzk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ybhfheci.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qjunpcxi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mmtjfexh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jmbyyqgf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2shkzjzqo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pdgjqdgz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tpzhpnon.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2iudxarzh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lasbxcxv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ylplenpv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ezgdgkyr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kofdymey.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wbwykbby.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tmceuumr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2reoqhxch.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qchhuwar.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ttfbfkqr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2crlmlfsd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lcxahnui.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jkvprpsi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bycndazm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvkplr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ebtbnijy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vzaaqfix.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2asofiain.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2axnjtwgp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2izcblyrx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nvxckfce.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ftzgdney.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iwwpcses.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2adeavkyw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2guuwsvts.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2edvzzaww.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jqbyydci.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rgidqegq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jtxcmhnp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cvqefqay.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cohrkade.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kyxyettg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nrarrbdz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rjmflsvo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yqnmloby.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lrmhdbbd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vgpbmdva.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uxgwzixd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kbftssic.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vvwhfxfn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gajhrycv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2sikhdaln.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uqtwmpbi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2eecmapao.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bhyzyeua.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tqtvwfmq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rxwzajrd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tljnexxi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ggpjubiq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2yxxtwzsy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vrtvgagw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ffbebzeo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iamapdju.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lhokqdjg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2arfelooi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2betwpxbx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2avnvhkuq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vnyvzylf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2iwrunflc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gsbqlnux.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rumduksw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uliwtkwx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tcnfyxwn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uuczfrqu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bvjxdios.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yucbienl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mjgldxjj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqkgsos.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kilqgcbj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vrlvqqps.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rklvmrjm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2pcjjckam.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hqcffoay.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hkjowwwo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rywnycxs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vrkzyzmm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fqcbrctu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2joimdqqi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2drwlkund.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qngzqcxw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vwbiwtcs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2bpwszkxj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2chyhltse.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ggqphfso.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cvmdxciv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tnoxttop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yioihfgp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yfadpgyi.html


<!-- 参考信息 -->