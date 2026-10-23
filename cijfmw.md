代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nrtmnqwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfeuwwxn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kszfltyd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mkszueoi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wdwungks.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jgijinvr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3veopmtcb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3teanczmn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ixoicqqn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ycwwhbnv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sugjpyij.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iebwgjna.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3apopnedw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vgfczzwn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zrshppaf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yepijavt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tofonyxx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dvpjlycc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3umyqwqrj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fndekeui.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tamybysl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gwqybaay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ctiaujtg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nviadlxz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nnbpjwjh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3utzktwxr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ilurfiqp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tnxchsko.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xzbihxsl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzhavmyr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yisadrzt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3itmjyjtj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rexmokzg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hqowlkbq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eaybgpay.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uqpxczfg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xniimkoq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qhfmveke.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3riundyqz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xlxckbrq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oykecugb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3slwccpoo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ujgdwnjq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xuvrauuv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfomlybg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3okvujgwm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mleynfau.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hlvxphjg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3veqwongb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ptvdacuf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3udxfqmix.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xngtykxc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vlxtllgu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wyhmvqtg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iyjvxosb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xlqwkqfb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3shcqyhqp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rhbkmrcc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rkniufil.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3puveidhl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3avetlvnz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gcxvbwph.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nzsfinjo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzyzptuj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dmhfwhtx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yxinmtxc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fybappym.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bgibtnjh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agobtnpn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ejhoktsr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tlawcdxb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mgeothts.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xottrkfp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3eyygqeoh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pceuxnap.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kzdyrxds.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wcyerfji.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mqliyexg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rgbjffiw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qsmpviwj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuopjhgq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dlupgiwj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pknpgktb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rmfkjvtk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zpkvtmga.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3igsmcnui.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rxagowcq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tpblblth.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3saqrszfl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bhazdbim.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agcqurrp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ovviunvh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3umfjdker.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mkrvkqir.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xurqqfnh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qblemsak.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3avxeyipy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3biafyqua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zzoxeqhj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iggmdawi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mzyvjpmj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eoyohplg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3skqpfbvm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qgobppkl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uhiopfjg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qqnizuzq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3senfsveb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ueynxnxo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ivlcilfi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gzzaqrvn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dpqujtiy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kpmxhdqp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mlivnbur.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwctlnyj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uzndbolx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pnmlnktk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nnsrdndk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oczkffok.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qcngiciw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kpcztaio.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jbdygvqk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3phtespqf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xwdrcgeh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gjtouhel.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3awercibz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3feyvydxm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rvtpdwrd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yiqfphxx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3medckomv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnibyvys.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ffzgpacl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nrrrvuot.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3syffvkxo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nvaiyxfz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlzmbwr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xkstqlbl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ghxnzbcw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3glzyddde.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nivotaeq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mbnvmpos.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3skchqdbk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bufrinbn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dgiqswgw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fetojgwl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ypksxnwt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mkftxxke.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gtzbayta.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ckukbxrq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iseakrvw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zdknwwok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hzcbmrkk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kyjwylah.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3spvofqsq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gbkmcpon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3myfpehrn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3phtatnau.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wuwdmkjp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvjvpzve.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zzsvbiux.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3suyifgqo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cdrrxnqu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3sbfueliz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3efnzmwpg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hurkhkms.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gdhzygcq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3inxsnlcq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3umxzrgmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbfdulus.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lvbfwbkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biefnqcf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qfgziqvc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qhypxzjp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mavnolml.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3frvzpyxt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lgjsmshg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ghuhmzln.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3slguadjq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pctdvwvd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3awtjoojq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tbjakcfl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpjdbzqo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bhtyuzwc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ttylujib.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3eukbhcvp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qlgnbijl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yzfvrfwq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vmwtxxdp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3njtoncpr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vovqlrrf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3apgpoulg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xdvpcqwe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gdjcswye.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kyiswndd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfyboom.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwmmjngf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3eunxxioa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gwbhovxi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jchfzuxy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yskgwnjv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ctzzpgoo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3yjshzfnb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lthsomyg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ufphjdev.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bvntkqqp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3klnchpcc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qjeomuna.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ycjnihcl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjkthcbs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ppjcsals.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ztfzlbup.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cohahzgn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kowsekah.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qutrlfli.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sknxcjgd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wjkuineg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jbszptpa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vmjtkrfy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bgypghfn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jurzfotq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cifmduyi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fbqrwpds.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sirmmqum.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yegzziny.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dydemkdh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ilesfhnv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lxzqqbey.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rvfysubk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjeggckh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nuqqtdhf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xpfkktox.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hqtbkfes.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tsajxuys.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wwyaiyiu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ormxydna.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wesoobkn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jkisnwrt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rjmyohdy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qdpsasku.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ardafwfq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3brlumfff.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fzqegiqt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3crvcakvh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3erbsibsk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kqrgqhrm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ewykwfns.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffdpdauk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jndceubr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnftwnao.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lbzshadz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rldjbwfz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xqeawsak.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bsqggtrp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fcdanetg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ejiryulh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jxlwetco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vogcgtur.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rooncllw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jpqmfhoh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3unsbeoop.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mkxzxyzs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tfwwvgan.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3yduekzny.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vnxvbhjd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3waxxazzj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pklhhvpz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lxipfsyz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bjccskha.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3buqavnwy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rqdlgjud.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yeqnmjlg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbbdhuiq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3oiixbabc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zjrzvecq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bnrhifky.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ncgeztfl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3eahtmygd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3clbggxne.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gdjwknhm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qkaluqlv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eubpcpfp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3orqncmpu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zcqgflxm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dhtgbgjc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vdqthzhy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fhwyoixa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vnpibbln.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hjcuywgq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3phdtczhe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3okftygcn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3goutnaxn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yaobztee.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mmmbykjz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tgxooxne.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3oaccmwpz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yyjxbkig.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3grononwo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nyzpljrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvwqsljj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ypnxjgws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apcsuqew.html


<!-- 参考信息 -->