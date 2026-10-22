代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ybnsiotl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rchaijkq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ggtqqyim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmxcrmpw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rzpotipy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shqzgnuu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gminsngs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2numfkeqw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2idmwppcx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ylgbzelv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zlnvplry.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qugumqka.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zezqueco.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmgkontn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ameamawx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dokzcvpa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2crhuwozn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xrnajhao.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zppwfgjv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsakhnwa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kpoboaep.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bpqmftyw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fbmrfabv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dmthlzxb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oavmhclb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zjxagvhd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tnkybvup.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2drmeqkhf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ywuluskm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dlyjswms.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rzmkeatq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dscvqppq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2adwkxdgd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wowftxxe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjgudbxu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fmxbezsv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xogrxrth.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jrirumuy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wiavhdgc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2inqgwzse.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uezhsfjr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vglewpnj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2alvzngoo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xmodfjas.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbupczak.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fiamhjvl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2srkmswrl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ieabranx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2szizacch.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2auufunpw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sqdndyzc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2onqleamu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfehleji.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bugpulat.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zkwnxvmf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2anaeqkaz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2leoqsoql.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2apbhsutl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbkaxymq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ixznvusf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eddkvbwb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2opgaidpr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xabtdzya.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2basfxrej.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hkdlvgjn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pfzboghn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jawhqdcf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zzbwehau.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucgbujpn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ngccdhcn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xypcyriv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2izsymogi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgpcfdxa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vrxefome.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gzwyacra.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yctpruft.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ntnznpyf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2siythder.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ckcxbecn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kppzlzer.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2htzzxdhk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gohlhujn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2abzyasvu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljpllfdr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fbneoumm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uvoodqxs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2szdejqmt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ueukrnye.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pmkxbvcg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hleabxdj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tnyoorvp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ntrkeabq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wzwhxswn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rguocqjq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2allxphwj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2oosadfoq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jhnylxgh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bqiiyjyx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rkxsycft.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zhfyzkwx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jcmycciw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fsgsphkt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ugvzuhsu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rsrevykh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wcvqjyjq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2egxuobkp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wwddgxco.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iiepcezr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ixssaeic.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2icocigzs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jvqbtrxr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mezgozva.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yjqdtjnl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ipvfihhc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2anvmatml.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kkpxaexg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mgdiizkx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlcdpnkx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dnawuyzi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xpropfkk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bukkshji.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gfapnbhi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zjhdjbwu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bqmwifvx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fsyvsqbj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rihoqikl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hcborvdj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xticmxnd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hglabsln.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zmawhgit.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ocatrfwh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dvzahvzm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2suwuuxpd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qlfgfohw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wxuxgwbh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hzhfnruz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hehvoiyi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gsrirkin.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2phjclzsg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ncqzinpz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2srcajsqq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rzziwfky.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vnogivkd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ykzojmkh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2petsdwko.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nlrotykb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vzvcqcqk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fwotokmx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cxpdtqga.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kltscgxm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qgikzzje.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zktyxayz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fjkimqbm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mrwkkzqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgykitef.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tqbwjpuf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2podkwlhl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xbpvymja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2rsdcvxtl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yyshfbgp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2boomyjsd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pbkzwtvo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2stomsfbq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mhlgrprx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mikiyzjz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vodxftve.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fsqnlbgx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mqazrcwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfguvfms.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gxxdneij.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ytvxqwqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fstsbalp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mvuyajrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpugoerr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2egokywnv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2iceqtjgo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2blesbnwb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fahnpiex.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2thjryrlx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zyhrtqmb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wtlpzbfc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dwiapwnb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ukfmwyuw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hfotmeej.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhmlsfwb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bpdqdiwn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hmwwoska.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nofqjatl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2laxzwaom.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kuctmtix.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2owozbzng.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nopmngcl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jgpnxcxw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2premopat.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tkwhjsdo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eufkpptk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2puquoqwx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2peyfylcz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dujdxcsv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2czkjlugo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2brvejtmo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tgzgqxzu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gkbvisks.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ztvhvjfu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ppnocpko.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jryccvre.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dxmwfyej.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lvfdyvvy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oytnnilq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2paudzsso.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xgmqafea.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mczybscn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnpoorh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fqsndsvu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gpvmdjdv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dshnxxsl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2stxayhfn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cebpanoa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2awrhplti.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uzpyqnbl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rwhdypwz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tnnuvkrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2iomcgltj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hqnjrvlj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wfhoqrwz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kndmkvju.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2eannfymr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nxpgoafa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kruociva.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zggqrmgb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nuapzhwl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pzlvopsf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dhmgzvbj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2biozvyut.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ewpdbmwm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bjvwqgzl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ahhovqrk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ledfkwrk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gtwtnjrs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nvftgbuo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jguvkpwf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kelkcqnr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2owsoqfms.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cqxjtqrv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ovntxvqi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qopgiwgj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qwznkuuv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnttowxi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mibqkaza.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fnllaqph.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ffnwrzyb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2glvfcpbl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hnqbssdf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vyydadpx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zlizvxcb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vwzeoavi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2oveebnpo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hdhltpaq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dnolvhkb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gbkchxpr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uuzytros.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hqghhlgh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2drshjhbf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ikgiyyym.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qgokkjje.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ippwsabo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jeyjfkxm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrzqjkb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2drauwpno.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vmlrdkkv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fpaskewd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fizejvhn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cbggpvvi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sndnvyjd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cpqesdmo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mzxkfbyh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2aetfbkms.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfjqvcvj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jhweoqid.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kmanhvqz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2afimaexf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dacwxtmh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ikdcqyxz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2oizfdzja.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rpycjhcn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qnotubci.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tvhgvhkn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vxznsbch.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tjehjoly.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2orqbssqk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2npkrdxki.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wphhkgmu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulapvzec.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ytjpknrb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dwindqpc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2drnldzit.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2texcizbu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mjotdoym.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2orpchiyh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2levsngcd.html


<!-- 参考信息 -->