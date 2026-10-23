代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3aatkzzhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djsirokz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mrgtorha.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kshxpkrq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vwaeiebo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bvzlojol.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ufelapyt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cnmbmohn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lmtratsw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eozcxtwt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eoeiwirb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jxzmoatn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3avuyetge.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3byfbwmde.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zrqeqizb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmbdal.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qatkhkvk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aytbzscg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tmirrxtk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dymiddns.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qyoryjtp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xeaqppln.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bzggwqzy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jukzqqla.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cfsqpkme.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3trdfwwjx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yrqdkxzt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3exduxvey.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yzshyenw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ptgzitne.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ckddnhsg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kspxpafe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3opczcfvd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3drgpdjgy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3haovdpvl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sqpfdvul.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvvfybdu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ziibohwc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3awgvthao.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cdmxveqr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rhtjujqi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gryhavwu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nuvfoodo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ajfksbch.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlzfwvbg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hpzntcim.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fqwcwqcv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pgrnzgfq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3foiocyri.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zolilqni.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyvdwprv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ecpnitou.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3urdjqsaz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yvgolwik.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3varmlojs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hiofamzu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3emenvldy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3scybibmm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oylsysoh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nqnphblo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3otgnpzoj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ybqiiefs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ruzftsfq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lxlcphsi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmgwfccn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3miwnkuwg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3punkclvl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wwegkosm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rptkieww.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3piwrqasd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3plwugstt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fuepypot.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fitlwbla.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pzmwolcg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lvfvzkjv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fkxpwyvg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3csypmhoz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ktpdmvso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bthulpnv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydmohgpa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vafdvlri.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3uqqpudwm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bixooope.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3elmnvmng.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ixrxzpyy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fixskeaj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kbhctabl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3orhoyfpk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uojifysf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jlglmmve.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hqbibubs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ldxkykxe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hnyfolvr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nwbhxvsy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3azryqaem.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tcveecoh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ldcxdsgu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fxytriir.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kwacjtsn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rdogqidm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fbsjwwdu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dywkocna.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pckjjbir.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sknmtgbu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kmtmkyyy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3brpmergj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxamtwae.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bniejwzg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jxyqpodz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ohfclhmy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yzcuysks.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tojoqvld.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xgawvkco.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ojmdglsf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mckdkrdu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vtmzcevl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fyvwztrh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3egxhorbu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tmdcxtur.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3raekuvkb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pwxxhmev.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ocixcojx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rkeimxqm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vjiowfmn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qcjxywzq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wjijuujh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3efxjdjuv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3aihktaxm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xpxieebv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghdlrjfx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dwrrcbnk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fivdneag.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ergkpigw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nuiiiyvy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3siugnede.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nkxovrmx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wsbalfql.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pgxdkhhq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nbcjsdev.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hutpgbhw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ggfbugxt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3darcqxhz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sufsgwqf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fyggyisy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3enwhsfdq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ikxsnfsa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hcbqqlsm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iwugsrui.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hyfpxtpv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3yyvchchs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rqdbduez.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ywtmsbef.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pkilfbjc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3nspjsvxk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3upkglolz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pftbplfm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nwlndlao.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qgehvilx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3foeaoxew.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qtopktii.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3btvrpvci.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fqdnuxvb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kxruvuwh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dttwygpw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mnczrsiy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3blebqbkg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3frbnlwsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3addumqzo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ersowpfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqojdtez.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ibbkucwo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gnyyhlsl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqbjaksk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3agbjmhqr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3giziqvpo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gkrzamhg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3btuvekpl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3odyonelm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ftouykpe.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ervxbcsx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkeipdqs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgdhugpw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yavnlius.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hpknrtgl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pmyfnghr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ahvarbwb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3icdinzcn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3negteqxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pgqaejuk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vkpkyuyq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dgqvlgbo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ayvgfnwo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xvschkvd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xzbdazee.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rydbdtgz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnanisif.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ppvtsggf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bwmuglaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xkvzqrzx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3biitxlyo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xystnxci.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ukgmbplr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vkwfsnoj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3aymkwluj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uvrudmdk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xgjohbmy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3flrfgzgp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgdelgnm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xqwchica.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dqqqxunc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wbbngnuk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mckuetca.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mvqzjkqx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jgdomvzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3pgmfmsby.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pzxyxhdy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ntrsmmnl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3aagztwbm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wpjvkjph.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cfbpjbys.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vmwhfoya.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3itujkbab.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3crakjerv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nfvqbavz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cmdmblxk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3oiqcgvek.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uvrmuoft.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3foczjrws.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jokjnooy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tceooaok.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mqyxrgrj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cyldlcqt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mjpsmrou.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3iinzoksp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3uqgomnlx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vuvkyepk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jbravspj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuuqnmrg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chwizycv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mxjayhlq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fkpugugj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3olssnsrn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zeqoxgdm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzobthrz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zxrcnrxk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ephnayjl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uafmuypt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3awapmsqv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mbyqeeun.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dzbfcjgu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3merrccnh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eokdrvri.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xuuclxba.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jfttvitm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hvjglogd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdjoleaa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wbovlasx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yxnyfbru.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qgleydqo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bvarrzua.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tcyxruzb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3waiowmcf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3smcvqfcv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbnkdbj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yjrnsssm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sbvueesf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mvriqbrl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytnxanes.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3drifcfuk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3brbqempm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltbhkjbu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ybhmvalc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxtpaoo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrdrenuq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3asoorvpy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tgupzhoa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mdcargbl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3marceqmn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3efazdcut.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cfpffohs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpdpoaji.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vfwiggcg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3euxgsush.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vadxunkt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cardvake.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cphersox.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3znvurpja.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hnulyghl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtiobjrz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hnnotakx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pizjhmug.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3diaccavs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fftvfxgb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wgxdhpfy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3umseldcx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wodltjsy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gcqqrlad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vimyzpzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xzseecaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwtwyqff.html


<!-- 参考信息 -->