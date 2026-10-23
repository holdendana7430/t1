代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zsgjaujo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uhvmamch.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xrmhbeld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxkjtlax.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3uqmxqafq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzmvgjkp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vznswoiz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mtbmnzqa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nywvupah.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ecfmhkhr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cduzxpnl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qmikmbdl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uqnnanqf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xnselmfd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nlmznwlh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dfmilkrk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydomakix.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3drxofnzw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaxlnkwg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dizabkmk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zwufcsmu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rsmwebbk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ngiyplws.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ejwinnqe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kbuzqsoz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cuabzope.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gtywecej.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qlwuqriz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tjbximda.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3duhzdlnu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cjoomnnb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rwqdodmc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xgttcyug.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbhehlxs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mpuvxzhl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vwuhxbgd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nktgdnob.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3babblkkk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3suisawgh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddfyghvu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3kikxdule.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3iyrspzto.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zykgsqga.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mvrwautf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3udcpnogg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qdjussvx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uerdtvjq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgavohxy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xanzydzd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fhrewuig.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bekqvugs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zmkyncpy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3myttkwyl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fhsfifjz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3duvuokvp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yaishmrl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ativkrbp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qrhubsak.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3urxyrlcy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jgpiknye.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mlzujlwu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qylthbir.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uwfjmwjk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tqomvsqf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vecmoczn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfgiga.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hhecrnxw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3csrhwand.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywhjldrv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wtaektfb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3iwggmxet.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nqfyndwz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwicfvsn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ypdtdodb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3eivtnmff.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dyqxsmbz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cyyymeqp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yjsncjhq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ozuuxegg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3paqcuvrb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ughssxxj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mduswltl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3eibowgno.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nnbojahr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rvguwmeu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cobehsjd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xubjqenp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wahpcyyg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vcouhcta.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lawifhqc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mekzcyds.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ecrhwnfy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kjawwqen.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dyethcod.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qjymsary.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cfzxblim.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rxonibxu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ickzwbel.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dilnkrxm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rlkbhgjo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zjlnpgci.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vimumtcw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3neuzbqpx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vnnylnlw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ynywqtwq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gmgodpcl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lkgusvnu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3namgqglk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bvwjgzny.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ehyeerul.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rdzravmp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kmutbfvw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ruznsgeh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kcazshyg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vnasnzen.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jjbbtoxg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ibjtfhav.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3isizjokq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dzyeqvmw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tttgjhze.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ezkixhen.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pxhrkfjb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xexjvnhh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cqpejpbx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cevahezt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlwryref.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rfvkamcj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zbbjmiyj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dapdfpfx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fuylrawz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3emwfsuvj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qrsxhniu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gafnoalu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vonzzppm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3behcxqji.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sbdvzznm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dkiiduie.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tseanmmm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zdlgulax.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3taarhzik.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sonxqiwf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3juejszby.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3peufyzjy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ofhyxgbl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zuqalohn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3asplyfpi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zahqqtfx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3aaswqoeg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqzyjq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wtbjzzdr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uudgbvoz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3omnyeebl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xgfzhwpy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nohpqjiz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pnvaiykr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3riitycmt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dcxiicza.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mqqoxzec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ulpytvij.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lcjacnow.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xzhilfzr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3azcrevft.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sviijpzz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3iqkjuftd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3igxfzriq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3emvldncx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ihxvheah.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lhswadvz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wufrpfnb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ympccgti.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3genyscwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snqgkxts.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iabxrmtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enzgusmq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3epysaxzj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qvnevyhp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3aqzmfubk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mrabhooj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dadpogpb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3djdymhuo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ihhuooir.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mxstqeqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3seggbnqt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lwhkspew.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rsuplrwi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lkjsmyom.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zhodkwve.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3iqkqmswq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yishljlx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pwwcnyni.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ivrziyyb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yfvoiaai.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mswoqzhs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lhcifolk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rsycawmh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3niforiuh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ufnlvbzy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lsjzbxpd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zpjqljce.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxgctdro.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3aueexkxd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kohczzkf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jluppcvs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hktjrodo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qyjrrcwr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uecklplc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3situgqkr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cyxunqvc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mtbwifgh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mjicsyjx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ktpodzgc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pulzvvyj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nzayvaao.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fzzolhpn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vbmuozff.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ysdtrtzv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zyicmdel.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qqgnqkzy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ozcepueu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nsvrbbkq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fuljjxcw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fcrzyjak.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sqdeeadl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3avpivjfu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iqvzkyal.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nuengmzr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nndzfuvq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3znriytpn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jdbhjsmr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aqkkakgw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3piujbdxp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3coiqemgy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nxutcebp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3whoclgum.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pcjegqdr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3uuolqorc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qnvzjpws.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ewoyfzfq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xkiabhkq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qzxihrve.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fqmhxatj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjodpvgq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tuqnccww.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3aktmwlcl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qqvirfuc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fzbyclfv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mzgxisnz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ghwcwmsj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lsgovzkf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aogfmubg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3axkzqtif.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttfslxel.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tuqmchne.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zbijhsze.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fwzvlhel.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fxkcvwgd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wztfhvhc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nnrwywfa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qmpgihfb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vumyiutf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3helazvfb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3njxcpupp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyvzwdal.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lafjkiua.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tbdlbvmt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3svihpjrt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jjzkllem.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydlokcdo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cwkmcpam.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rbwykfry.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ysftjuxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuglzyiu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aetflmwk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wnruvtug.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfvleyzx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3avbjstcv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zgpozbhz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jdtqxbso.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qoqquvbs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vqarnvta.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ybsfxgee.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3datuchuc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xlydpxtr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zgogvzcc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vvgyxxhb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vryehcza.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dohvzktc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cmhshvwd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vfygncrm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ihsqznhi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pkyecodg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ndvqbhjm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3buvmjibb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gxjjgjcb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bsuvydud.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3igyurhkz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tnfnurae.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kgawgxav.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3clurrwnu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3znbethqd.html


<!-- 参考信息 -->