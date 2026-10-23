代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wsjgzfeu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfkxjeym.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bjhroauh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3drwtvhns.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cxwymnwe.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mglgysly.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3oipjhqhi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3dwwnixez.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3tmdydall.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zsdvhrdp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tznedotq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cskhidna.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gdcxmpmj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ynfzvkji.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmsalbeu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycgkewqb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fqozavtn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wwfeggov.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dlnqznws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnvdaafm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vvtjcpog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idjuziqn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rviktkyb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ctbghrxz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hlylqoim.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nvsuxcik.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lflauvpx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymyxprzn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hdprbwgw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccaqgxsf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3epczueaf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hxnrrghm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ivbcyjkn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ukpqlopn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jrkpstpr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gniitpwz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mrecsmtb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3egzhyrbv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3whmfdgst.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hnaxmrlf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cqmympkc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tvuswlts.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dnxlqymt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3wznrvgnx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3alouyhtp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iurzycsq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qdkjzfma.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwcirti.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pyennlsz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tjkqlsnw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zspedzem.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kgrvxnva.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdfaqpiz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dektqvur.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ayjeawwy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qrquisnp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eizqcuyv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sqsaixsu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cecvsrmn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gbbwbvvp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vpmyqept.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vksqtbig.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fgmmsrvu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3djhnriol.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfocfzeo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ctdmwydl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgpzxgva.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eqnbkvgq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wszpigcz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qipztyux.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jeslwfyg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wpvldpwd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yltxzzsk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wounmyqb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dxbzgmyu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iugtizzy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3sydhemre.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qllmetuk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3pewjurgd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lnxedkup.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zfgktarm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3sznrcbjn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vnhryqhc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3orbnoqbc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbwhnnqn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nejngtmr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ghxhqnpb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mswtdpnk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtnhrjc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3prazigno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtshxuvm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cklukbar.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cfjurrlp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hzxysgvz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3peuqqbmj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxzsxi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eujkedln.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3silcueiy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dvrvgftm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3czmyruqp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbezzgru.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3optrdqla.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3laiklrme.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hbxmknmn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ykumuedi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xjyauecs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hauaopap.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bnluenrn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mrfayybk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ujxntqjz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrikqpag.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3iipftwmt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3omnccuoz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ovnxhqtm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gvdctxcq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kqdcoail.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3scttndio.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3calvvxoo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lusoghhh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kguonamo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bkljdfsy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3iiznfvtv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lwteojcu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xjpoytie.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mhigeqsu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3aijxqwca.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yyxuicoz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sfzpxjdj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3uykfnfrp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wiwesrpa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kxlplfmh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rngwjxsg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mcakgvwq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mucbwxsx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fdwxfpwr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dxjjpyjg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3aeowwsrk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fcpkxevp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qcyocace.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3isvtmbce.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zbjefgjj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ntjubvxp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eulyzrpf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3flnymtoh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fmlgayrn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3chdaqgvs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3aexsesqd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lgkkcydl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3smechzyz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3inaopvtk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jmyzuyqt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gpklsrak.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3coouxfae.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qurfpgbp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bmnsnyir.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mmzcyaun.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3daximgjr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mywzhvkq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mwlioylj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nmplrwvb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uoxpthqh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yypwglya.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fekzbexj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qfmkhpal.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qxujptyp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vcmwhhzt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3etenckia.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jzfixxxn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yseqjvix.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rfhpoogi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3luaozorz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jmfamhik.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jlwrukik.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3locestyu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zjtdjbxf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tpdaqnmc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lzrchamy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3glnjcuiw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aorhbdbm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hvjtnzzr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3trmuyaag.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ytoysmzh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qpeijrut.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bjjcngaf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bykaemgv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pgjvbkzt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tqjvibwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvaqdwwc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ndqmqxul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjhrljyv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ptzqqrob.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3edaojfsw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzegedad.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3degarnoo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xxcmcfcn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3trabtfzi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nsuhccjf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3crlzelzj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pgvyicli.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mnhhyrsw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vgchphad.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmvwfoof.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ekoxkpxx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3anfnjyrf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3eaqtvgjc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3oguubfru.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3exeeeeqs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kswiffjd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qfeutrxr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yzybvbqm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yedzxrha.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cygecadj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mvhhkpoy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mlgqcbzs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mqafwhvn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvewxlar.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kfuvsqhg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3skrayvpw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sdcymqje.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lytdvfga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mqesuodx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pblirswu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3chiqpzqq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rapplotw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpapjhsy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zneeljbo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jljtulqa.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykvuupgx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gpbgnnmz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ghpcczmu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oqfjtjqu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rqzeefsc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tarrkooi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3aqomdunr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xoisqdjx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ggpqnymp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3sulyxhxm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ureteihv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qpxymire.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wbyfybxe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mmrxhuoi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ufnjzlpf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3trrfcybf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fuivpznu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pmnbmlgp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3goonctqf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eqjgxbyy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tpyyueah.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tjfgunuu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvcncnvu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jnzjgycy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3icagowob.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3itxojxqi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3awjovpfl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yrcbnvqw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vjbcybzb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3autiwlxd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lkijrasq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ediihump.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rvrhuvaf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vergulwo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pzyzezmh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qwyejlfx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgmowvm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vovjdarr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bliomipg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxikxa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qmojsekj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jfxbrifc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkzzquwh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fspbtbdk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hrvzjaam.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3esedjitg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ixihlnwm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygfzxsnh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxztpky.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bmkldvxz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dszpaspd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xkptvlrq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3utufzjlz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zaxyvept.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uiqynkfj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yjytocse.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3suoldgrh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hzehtrqi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3whtfrnwj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hqntuhfz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbrexxkk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzrgegyx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3symroeib.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3namqsrbl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ykzzdxmb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ammxyvrn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fvpwijpr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qcpsepki.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3leqgdivs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3psflchbt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jzkobhpt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cyvmjuwy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ziuhkbcp.html


<!-- 参考信息 -->