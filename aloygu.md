代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wopfspnd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rlncpxpa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tsvqpeln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyowdyrc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cplnwomm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vejzumez.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hnbqprgy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tieazrvx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2abvzvrjx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uisaxama.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xmdmholu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2emszrwsx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ngvyfqhh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbjuukit.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2iimbqvlc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ozewutlz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mdbzlcbj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eowbvjmb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxvrtrim.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kayjwsqr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dignuunt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pvxnxpeb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qqoklogy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gknghhdd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ixenbbnf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zktffkvy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ajlthwqd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2puvsbybp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mteakxgy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2njznstib.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hfcuntqy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xswisljy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2flmijpen.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mnufqprj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wkqzzojs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jdjqhjsh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rqtoqanw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2snlnpcbo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qzuiisbu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dxfwgfhb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2inizjwct.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ifcmyvtm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfcacppz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fgktbksi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mbuxsdzj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tbfvyhap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qvihqled.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kyihyppq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkygpbpf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2udlqexgu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ptixhteq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gmtatknv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wjohmwdl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hbnxfnaa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fyianizv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ykvlytwf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vpvxldxm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2faurispn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ewbaoipa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xwnfqlwu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2roapzpaj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vjxeuhwl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nmyzmajl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dyzzyoxs.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bfvrbxkg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2silbrjmx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iormdpcw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhyebpuc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hzcknipf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jlexllxn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sewdqvjs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2erhmvhef.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyimsbdy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tmokllms.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vwcqkrkr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fagqtany.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kkiwqvwb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hdnubpzf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oydwoeft.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lfizqjrl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nlervzqj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rtoeudni.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2scxvkytv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xsysdirp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdjsdae.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gvuivprx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vnlxsbfq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kmvfeqag.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jluqsorr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cjtgrfxc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mspppkjr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sswjhhqm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2djrecvpn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2indkebqt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2klftjvzv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xweccnuk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ztlkldfz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rcdrvivc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ibyzhepy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fgmuwojv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cpgzhkrn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2spywbbgh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ennmedmr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kohuxsdb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ofiqjbek.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aguoheqh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abflnzed.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qyrmpmkd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hfsgpsar.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qcmmicez.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nkgpouly.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mvjepino.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fodvunmp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nsidrhgy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eikvhoui.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gklgfasp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cfvpjqcl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvabindv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ntmbepkm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fqqcojmr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zlatsdbt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gsmwhxyd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cgbjkqte.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mkzwxkvx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2klghrdjb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hcidntgo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qyvychwo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cpyxxxgz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2axuzzqst.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vwipuxzd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kpwqnuxo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wimlpywi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qrfrmaek.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wsmjeqol.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pxxjiimq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zahyhgms.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jhsbvtzo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vhxxpaif.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ytvbdcrs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kesfunwm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uoyvfcrm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mumbaufe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zacgpcxx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bviahccd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qgbarrda.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2idsmrqmb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uuvxfmbn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2loyhhqen.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oyjvcbhh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vyfkpzli.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2txmgfulw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mrpbzflw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2awhcaktv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rnplizca.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sirwxsnk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ondpgred.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rnfjezux.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lcshksor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sljpzvlj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2senudxpj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wfxeoaxm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2flzxktnt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tvbkqfnp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wamwjdop.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gjucthov.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2najauvly.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2juyxlwyg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wxzttijv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lonuofbf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ofsyxtja.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dgzvigmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fczpbzth.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gdqokqgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aejxoedq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qcgbgdos.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bahtxcnr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnqezajv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2layjmada.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lugofwjq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dsxyxawk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hydrocvl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dqcalibr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lwaurknb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jetlltiz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egytzgqv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eyliclfl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2klfgsclh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2naexlbdj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hfvzdegc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ebtyiupq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fxhgjiqr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vvnajxqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2psuchzsw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rqvcvekm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sbgtxgmx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bpxtnsvl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tyvyflmp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgjjxew.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2clmxzcup.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vfaesrdj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qrfhqsiz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mbjydaui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2onrdnvyg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zlervasx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qutjtxhr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dgkvtygg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pljmladg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mkefocge.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uvalnyuw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bcvrtcoe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pncwagdd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xvwmxsbz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gxwzuojv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbvgqmja.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nwcqkeld.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zfoibnhk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iajftbgy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nqyxlxmi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mdixedvm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nfrasuxj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aqxqemif.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2lgeyqfjy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ysgsvwrj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bbzjaabo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ypuvmpco.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wazngeqv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ubyjmhtb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vlzoouzt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ygzvcend.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2onxtajtw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ymlwigdl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2spprzpfq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tkkirfwy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qybswczm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uixklduv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ekcfncme.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2isewwdwa.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jsdqhpso.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2keqbqveq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdlgxyzm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2blxjhpsl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yynvojdz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fvobsugu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mzrfwone.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ujfwddrc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lgkbyedt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zmpwazlx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqssvvnu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lzcsvfnh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yozftcuq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tuaozjqu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2olmuwdwb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gskuegms.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ebadeafo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fqlyglkr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vwupperq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rjbcuduv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fledvqwy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tlxmydaj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnnotuul.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zmduvtgb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yfgpqedm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkxefkbw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rfoitrzr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zqydgpqx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2seaelqbj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lgqzonwq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qgimrgrs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vnhmaedc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kmhzenga.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bjcowvwl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pplrbxiy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2afauqldn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgrdwaya.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2amjjqvsq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2izxcebpk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ldqxhrwa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgdiebyk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ozyyakkc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wtjykxyn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2msmbxybj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ktxzpaak.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wpbljvwg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ktwqrksw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2svnghtqw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2btftotqn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qiungydd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ohvzdtap.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2enfwtskl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tfkhfubp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jpsvffug.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2errrliub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iryepefh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pptfibqo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2srwjmxbf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zounajhs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gwzvigrv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2afuvxkyz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nlhvfhhu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lzwnxnaz.html


<!-- 参考信息 -->