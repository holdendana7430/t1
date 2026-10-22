代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ahfyyslo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nhmujbkt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2owtfqbnu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jmqbrwbu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fioxllao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2znpffbkd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjqpfitc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bpfbeynx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2leryqdpj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qfuknjqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kttjsflf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veoyjizu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fgtnjyvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wptfriva.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qpanwjdu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gexgnjpe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lxapazty.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2goaggzug.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2okooswtp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nizyxynf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qmrrjzvx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mvfzvamq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gqzzkkmh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gtomnaei.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2izcxcjmt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2beapoxbr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqyytthy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cawesouw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ukpjtcby.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mhrprrgc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nztqwgmo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2utzvprcp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fpsouvem.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ofwwwivz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vvbuvrnn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wwqzlddy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2peicqavg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tfeflwbv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xexnscum.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lytfzomb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nhhntnjx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ggemrcra.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aieqaltj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cttiuqei.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrwgpaoc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2diyjnjzv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wxsjojwh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wahhaikp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwedlqrj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vonkoxbu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rdhtmfkq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rdbupujq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hqlhbula.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yikqomgs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrkjgjkn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fktwnqwg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqrmfmko.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vxxfhwua.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yntrxgbr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qkvoyhxd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2aekkgwkv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jqxiljag.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xfrisirj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hxgqcznr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mqnmlzzm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jpdaothd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgnttejs.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ewkzburm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yisrshza.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nowztvbc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yybdkpwj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wwafbilk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ycrshdrq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ictldigf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ldzgrjji.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zxiqyqyh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tzxxcysd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2valbpcnp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fbjsoato.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pkczbkmw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wqqsznpo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dvpdfahe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hzujsetg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rhdbifir.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pgxcdyge.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ixpmziox.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xpdouype.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fflewbub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ysnmckkq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hzcxbckb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nawvujez.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ufhzxtha.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzqhqytb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2iavwtzqk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wghnxysl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bmsxnswf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2equfjasi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ffwoylpb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2haunsvtk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bupromcz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hxoyjexl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oktcpbga.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rjuuaszc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkrphzeq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2duvtxaro.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2atzrpzmc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ivlgurcy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gvpvzdpj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2oxwaqpha.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2yqqjpngs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dqduxogm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ykszrrsi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lluoulnx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ewoxkbvf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wdtctvct.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qcallmum.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dfqvrwdw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2makznuvn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vgeccxkc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gzutdbkh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kbkubyqu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jhgluopm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2knqzlgyn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pnstktgs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wcaeuvgt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuaeeiyx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trmloqed.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dvuivjww.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nkitfezr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ovdafqit.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2akoljjlk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2atgyueqk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2aaqploqh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xanylana.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zuaiqvum.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lrunmsqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gtvirhuk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ikkhsixd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fpdeutfu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2udpgnbsd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pordgrtu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2euerijkt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lqbsgemv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lgbligrh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cmihbxaq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bhfhohpa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2casiquaw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tpedujqq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nsennrie.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lodvbcqg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yhczhvfm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hqzmhyny.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kpvonwwo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dnvllefq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndsbkrlm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wiuxnski.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kpxboigz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wetxddth.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2decoarne.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rjrzgvrh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xrthmcta.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2iszrnurc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pljfdwsg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jtniizmu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tmgwpqni.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2oykuukrb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nhneaghh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvnixcdb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cajhrtwk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdpqyxqd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qhlwaiyr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cvnburmy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hrhngxxp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ajowugit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2awsiqcur.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2oznxumjt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vwmfacqw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mihlovwr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2chkbcqtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogpopbub.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jhynokfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hydrfacr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inmmsvnt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2miupynhl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tpgkpfay.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wisfnypg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cljhszkc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yohivhjh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uossrymt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2onhgdsvk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oczbrspq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgbrbode.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nflircfj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zlkocsqa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2omjvwghl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qxmcvwhn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tyasgjzp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ujpyfwrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dqqlulve.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gogztrzj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qsrhupan.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lfvmcwcb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ktckfobm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ufgwekgd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eaysxaax.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2riuluzdx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qixggajv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywdjchqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kfutrdjb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2quijgbla.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mngqyjui.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nhrqaobd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yglkkbxk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vlrkibzg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wtoxdcgk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2eboaijui.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rayxswsz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vslwhhew.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2oijblmyz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ijjtnhyb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2krqtlwws.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ihbvnozd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zdpwqcru.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vhhuipeo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2elrqzknf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wurnxczw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2udfvysrg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lfdiusai.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eizbfkqm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ttvqahas.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yzoxgntf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xjocazng.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rstsbvhy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qotcjsqh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2iusebgfc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rjwcoiwb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zawnbczw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2njskhmbe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sjdhsxop.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lfwgutgp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bwlmuypv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vtsjtdoc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fnpsdplq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2otgtrcnw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uwrtcjif.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rhhezgke.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fgralnph.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uaiyhxvz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pezzpinx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btrgewci.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jdbrpqig.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ymqkzowa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ofahnwop.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jfktdlga.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cukglrhf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zfgmdaxv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vdyyrqlq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cwtogmio.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fhfwfrib.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ykhopxrb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kmtbdrpq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qlznjunx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2njlkzdlu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yjenmudq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ettnvnnv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pgwndejd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bybryueu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qgesbsvu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqyciaoc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ogqcprcu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wnwcabgr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2taqyhfhs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gwcettwh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxgxedy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jxtfzfdv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxydbzxp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ojsgfarj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uuplwwct.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2irbsbhfb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzwzlnw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xrcchoul.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sewadobv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kovcaexx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xitxmsje.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vjmimabj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qlwbiasf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fnuqtaby.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2asbwybrd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kdsxnbnl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfwdcfcj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bdivhsii.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qpryqfan.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdmkozs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qjijwrvw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mnpwustr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lpgvlnwu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2grgbsksf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xqlxmwsl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bajyiscw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jiasjljz.html


<!-- 参考信息 -->