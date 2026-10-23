代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wrhgpfpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrmlpksk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zsohpiif.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dggmcobr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ciddzvlg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dlmbffro.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xalvrvim.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3socwvjih.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ivbrxnpq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdicgrpm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vhwfyghx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eqhccahh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aovtuzhr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hgleufpq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kytmslsq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwzxwfbk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3auxbdbwo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fivlmwae.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dytfkvfi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtagcjtu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3smevvicp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3awourchv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uhexnkgw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ubsnpngz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3oqsxtwnf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gnjzbcyh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lmhmuyph.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3srgolkrf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pzicymik.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zgtvjtae.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kdxhgmlc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ylfgpxtg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghfyfjgi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3baxrfcwo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aocbokel.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3devrbtnr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3txbanmji.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dzryokiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vtnmdybw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lpiinfcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylhkvjxf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3clwjsboz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3excakxjp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iznrsnoq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xxsqzuvo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tzscemce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kloavwvt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xjxkmqtc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cvtlcoon.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jzvjfauq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yfsetujx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yhluezya.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3heycqgwj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sgnutrjr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3byvdbwnh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cqmcwuas.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3trwtvfih.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hvmrogcf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3noztrhol.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xdkdektc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ddmazsxf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uishqcza.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jqqdstrh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwngimdm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3pjzwntas.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3elbphjde.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3aexhbhvh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ugeureem.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skiraapf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zbewyrww.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ntydwjzj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nlkcjjhl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fdykddje.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wamqembx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fgcepmcs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tfjuxdrv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eqclzvsr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dicbakhk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hfojohsb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gnnkpqpz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkdnifyc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3iplkhiyz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ojggkqcr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qmwvneqv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ibwadlrk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ovfwrwol.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gqnipmur.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ygysmhue.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eohbnvbs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3fcfajsmy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3amklnooi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3agmmltey.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ybovsucp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3psntagtt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3idpsbcuu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lidejpyw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nrhfygxt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pqirxsno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ycrcavdq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ikcktnyt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3neygzljz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3geduvihw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fsdoaken.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ecjfzuhm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3znxkydpd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xwvltjus.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lhycpycm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3oujspelu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nmhwpwae.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tnplnbrf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yffhhsdd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uzfvzunq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vqgaydds.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ggasxott.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxuoboij.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qofgpjxe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nuyxmuhb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gjujvbep.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wlvipppb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pycmfaqx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qewxpdvf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jjboolqx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3obxivdgu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dxfptuyg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aoujldui.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wfuinaki.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kepiwxho.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hqhuomjt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ncpgzxzg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vdeefgyt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kxuxtwpu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3twrkqnnm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3afpunbvp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zhokhpwg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3obldnljw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yhdlmmje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gdowphwp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ajkrtaxb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wvbpyfra.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nycipaxh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mgpbsywr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yafeapat.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvgmqlvd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hejwmmvq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3aredvziq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3alspvluz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pvhxmzua.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mqdkherv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wxnubvjb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3auloabsv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3aucivmri.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lchomvyc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tnyyulbx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mlzewtlo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wxkzdwnc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ifioqera.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3itzqtmnl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qzkqyauk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3anmjclfw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3sceuxxqu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ckgxggce.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ftbovxtb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3udkkwilt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rbfpmnhr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hlyxoext.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cqxnyllu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lichobna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbprsrxt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ptmbkpmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awojhjap.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pccubboy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dluibdhn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pmdphbup.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3phnajfqn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xjtyzihl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xnegnjhp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3knluxyox.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nhazvjex.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lcfjxdix.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vlqrccfy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kqtbygxq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cmjvaoku.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jvgqbpue.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3esqdinuw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vauvzpsr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zvokcuuk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fhnicdnj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lltzdagn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3irpycznp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jocnegzr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3oklwrxqz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqbfyqva.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kenjanxw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ycjeqceq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vnnmhvcx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pxtmfdsk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mbruvbjo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hpydoziu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tckpsppn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zwgghbds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3prnirdsz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3okqujhaw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3szzqbxla.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3figtkote.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mifumgxn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3giybcaus.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jsxuizrl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cxncnlft.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3slzwjtkh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bvygbsbu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dxepesxu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wphateve.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3whxchmls.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3htfzwfzn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3khclzkys.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jjjwkzzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3shtnbaoj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3obebtlxb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3umgfwwdk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3deralxew.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3emudkzku.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xogpsizu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uooespxy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cqzwebac.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mzcvjfrr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hinwyzzh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3boflakgm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jwaonizl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fywekozh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pohkjpko.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fgdricju.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dfakgval.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sypajtkf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hlblnzab.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3aqpgzfbs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iwqnffol.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3okgqgfae.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ioikmfxa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mmlqmeyv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dfhgcucw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zmfxpaxe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hurzscvd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xfqmeflh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lrcetewp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vjddnfpb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kkwesygk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zykhjdxf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bjsgvgdj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wfsnzpzn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pvgkkokc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jfywivzm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3purmtzzl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zofpyxii.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3defortzl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hejodwuf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gsbmqbhh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxwxkrvj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbgppczv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjjbglyk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kcefwaly.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eyzlhmvm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gttsafml.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mfahehii.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3djmtpvki.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ubdjoala.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3izefmebu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mrhzjfdy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avakxlaf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvabnbsd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfcfsdvu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqalubtc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qsxnylya.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uoejscgl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3npsjosad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fhelupid.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3aasphnte.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zvqtdwkc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xbyyqdvg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jmlatoie.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3irxhtvsh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3syeucpec.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3atiqsqcy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rktpllpa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lvvzajjy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3iuppatsh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cewutfba.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ihtwygmk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3abieblrt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tcrywojf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zkeamqzz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3szucehuu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3oonkmoiq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjgjslgj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tlwiffyi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sdgaomye.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jnoqigll.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sjgflkyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egbviykx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mmkkayde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xokaekza.html


<!-- 参考信息 -->