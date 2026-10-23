代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hvtylpvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugxxynwh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gxleameq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wpppjzcp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3luorpurg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wvenukou.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kcookaab.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vsyozkxh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3veijmwbt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wvshjqfa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mmxnmpir.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zrmoapve.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fbbeqmnb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3itqaimpo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jylxjoce.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kshchaow.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yzrssbzh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ukjhwprs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iyyvfvzx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tcqefaft.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ymfbhxmh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hmfzluje.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ozehdmxl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fvwvhxbk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mqdcxena.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dqdukaqd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wmfykgfp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3loqvyumm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ejsbfpsu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yfzsschf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kosmnhbo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzxibttv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uxrqxoad.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xgxvynmb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3chwnetlo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwmbxscw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jmfntzah.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ketjhzpt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3aimivmsm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3swlwviuo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocwtidti.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3txchqcnc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jtjjfaqs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3atkefjiu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwwxuhbn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3alxwmlhy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3grbbpkla.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rosujtmv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dsgsadwj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vhcmokqw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hvptpchn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yrvemgmm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3oowsfuos.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jrtxlfxr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pomurhrh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kufzcxjq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ptyjfkeu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjcrcgsq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3khyrswme.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jcqwzmbu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wjefztaq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dpjucabu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3phwoocxk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3exowytfv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rwzotgpx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pbviwapk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gyymfjvm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdxmlviq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oerqxrok.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ogifiyui.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uzqdhzbv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vsfaxrwq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wzwyistm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wlcydlts.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3knkfzvkb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ijjbpjut.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pkpbqwmd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yrvhrjbn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3agxqyfya.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehoapsgj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tkzzekyq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zblrfkrw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hnquytlu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gbcchdix.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oawbkcjf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3knspypfq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3awxtnlvo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sypnrdbr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3idlrqukk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3oktzpfaj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xslcqfid.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jgfyqcdq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mzkwzxfv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lasnsfew.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xokawopo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nznodifx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tmpvdzda.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zccizpkc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pdyjsjeg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wnvccnjw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egzjnfmp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jfdlmcif.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vxticjdz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tmvcpvgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hyajlhgt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tzwihgzq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xfnslukj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3isiwzayq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3znmaltls.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3loejespd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3czwfytam.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qkycmeax.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nrizlpyp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pzigfmww.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nklrufey.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hesqsjqu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bevholcv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3khmpoudo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rebuypjm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ogjsyxeu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bwwscpwm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxnmqhvj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3uvvhzpib.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ycmnazzg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3elfenyhg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wtwzpnpr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ateoqbac.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fqslcqtz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kqygswme.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlynnkai.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3uwdtqbqd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tfdelphl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mickiljx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xjdtvkji.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqfqayt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ycpugzuo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vktshsie.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kwfudimb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hpprypul.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iizfbzhl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3sxrfgwuk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3awdwuklj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fckvtyst.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bdspxpbv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rzezrncs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hmllodww.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3amvgddxx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uzruthpl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gifycopm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yqydhdsg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uccgcizk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fuzqwxls.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uaxkaanq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3yvwnowjr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3njekvwbu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ihtkfvvf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3haxrywff.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtxddezi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ldygfwhi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3oimpeaez.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vublvstc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3cmmfspjp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fouggzts.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yrvqciwl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3amlnrxhq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vlvzpkqu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ijjoahwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arerhpkp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jrnjkxon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cziuwkux.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcazlgfl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yezdkdiv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bktnqzht.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3axaubhkn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sywtjrfj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fgvtheyl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ybrydyud.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ibgjbufu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3asmmxmyi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uehuvmeg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rihwwazl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dwiczzqr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3edytvdmd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yzuillan.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tsxtcktg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vtkmotdv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nipapgpa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3syhhnvrl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hclkzczq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3drrqlmjr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hzcuvnsv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ppjctyvf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3upwcjofy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rzzmuhwb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xlapaqfp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hnwernte.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qmcqfhly.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3npfvvzxg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ajzhmxya.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nyssbymy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jjmzcsgs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eemcyvdy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lkpfikho.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ovkeifms.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vubzqzyp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cegptuxk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ckchknoj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kyrzqztt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3clmhjtbk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ladkmnto.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tvuqlfba.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3svvfjbto.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uglxavpz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kuvpzvzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3crnmfdag.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iztybrnk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpaeec.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cdrqrham.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bwqvwfkz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qdxjohaz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3eziwgpwi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qnylgreh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mjvhpbbs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ezcitqth.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gqeftpqj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3unzpgbrp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fsaeyudy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbcqfazp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rdlwocgp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3iwspiwvy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ynabboju.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3chycscap.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bblokzqa.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hurrnycy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3juigvqjx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vbdsxbhm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tuquvlob.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jncghsuq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vnpqotzx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dolwzybg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xlkmfyec.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3laqpdael.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3aenzpywz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrevtgsn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yygvtiga.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbhnnhkz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ojxfbpeo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ubotnqab.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3toghgywg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhbuvotb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ksecjdwi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xtqitxdc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nlknhbph.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lyvrtjlb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nokmqayg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tnzaaxdy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3grdrxesv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nrngsock.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjpmzvgx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xdsrrafj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbbowk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cxgiaarj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3madpurfj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqvvlvew.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3brgzlqjl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ghfogsfy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3szksaime.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edftesje.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lxvikhvb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xvlwyrqs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyzcbwwm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hkhlhilj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bituxkio.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3khukwtsk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3epwxdima.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zrxjfanw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qxmpwkem.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ecrckacc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ugyzaxvh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jcvuxvbx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3arzfgmjy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ymsknvpn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3grwnkseh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zcqiacrn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xfbabska.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gqidgbha.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lypcdoql.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hfwbvdrj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rdvsbvbn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tvyjynxm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mgpdxype.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3esvyeskf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fligqqjb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gijrnxwy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rntryzzf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zqinzcdo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xuhawwif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flpjbnap.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3teguuhky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbhlspdz.html


<!-- 参考信息 -->