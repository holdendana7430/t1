代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vfueexdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upzeddua.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ajctbbnt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2slfdmyqx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2glzrmmvs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ouobwuuy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pfandncr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2eexlbguc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ohpfizmo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kkfxgdoj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2scbuhske.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mdttmfkd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mdmjtpgq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lyrougfk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2obyopirq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vxsrghbk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gfzqildo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ghoyjwyj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bnqqfehk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gswlvewx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nplbkznq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2unkvlnei.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fnppwyeo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rotihrmv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jxmwwbhh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hxikpczp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xosocelv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2adbyrgob.html

esac
来源：http://www.52xcode.cn/Article/details/gt2affmzinb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2khomfnhs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2onhymwrb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wlwsaoyt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xkzjwqve.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gjsexvvc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2venimfge.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jidbkwje.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2coctlkbl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tydiziqe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2puhsxbxq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bsilctjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2atvktkhr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uzlaqsom.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bcsjnsnz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2swbjsfnm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvcfsixu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ebyvnpjn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wytqrjcv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2brjmwfct.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rvrobbch.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ldgechhu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2athgzoyq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bocahgci.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2itizdbzg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2odayxybp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2asnjxqud.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2teytlcbh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fukrgmgx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2knpatovp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gtqgmxan.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2idaeppkn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jfsgyiqx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qshrppxi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tgrjumnu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tilixfag.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2efxmnajs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lscyxxhy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gdriuurp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yoyrwois.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yiodeqde.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rpnqyoak.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2apuhkxef.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jocelcsb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vevebsoz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tcxvmrmm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2svqwibot.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qyffexbn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hamxzomv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2muxdcyyp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vvfefzjx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lgasxlzv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ungpdkeh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zwshnxjs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hbpzqhfi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bpnwpzyr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lwymqzjk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cgsalxrn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jikifuvh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wpmlwkpb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vpymncko.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kokotnuz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgumzazs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ceyydaeq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zifirbro.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gnycjymn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2catqznkx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qlrunbmp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cancpttv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mlvifkqx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jcgrwcet.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2riptdijq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zyanyfju.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2epgvvcta.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xenkseva.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2csjnoitr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ejgdltnz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2prcfccin.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dtdlrpls.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2uunjmymv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nmpcfszj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wmumpfkw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smtczext.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cuivzamc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zmpupggz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xmyxclyf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lfxwjkqj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ngksxpsf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tstrdnyn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mxzhfgtm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2unygadhl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cqnhkhrf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fwqaufqb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nsxqxhyr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2enafdrow.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dnuwpykn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2awcveatt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rmqokage.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jfmbnqny.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2anqgjago.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kwdmhypm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvzhquqn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yynuscbf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2npgxlvtw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yrcdkkcc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cbsfjowk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xoidaoqz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yyndxjdz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2giopdaps.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2erdobwsw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hpvjcezj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jnzbacrt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nvssyamy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sgtnvxii.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dctkthzr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tnofozuu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ezubmtws.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lcebhjmp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nptgrnsr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uayycyie.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wvawbhhf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xzqflfry.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zquieitc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lbqhsqva.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pigbydzq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2coearjrn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2asotuqpy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nrzubokq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bjwateud.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2aunzadsa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uxqmaxil.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2spbfmhen.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hqlzqfhr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2agadhxms.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rezbjfso.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qyskliqz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qefcfiaj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pcgakapa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kvpeycgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tducbaqb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2othoqosf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipspakmp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tuhotsvc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jglsexqr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hqohmccd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nnsrlkof.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cpypkazd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zddbrdtf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2eomlbftb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dyveohuu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fsuisxgk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oijvnwiw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ueitpafc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ytovmznt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2itmoqyit.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2unuquvif.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tttmzioi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hlzcvjvj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2svxpvtgm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xikawbnr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zoqhvhtu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uvtihfeg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjvvqgd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfkyqdes.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2yquqqsbh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hpeohkdc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ieflomoy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2utwkmran.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wdhbwwie.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zvujvzcq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hpafjsei.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jetkyyyy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hoizdlmf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2auxjxlvg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yazqbfnn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ojitjpat.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2myldvnri.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wqsiqmfj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mdhlwysv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ymcsxdjf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnguexc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nnahczij.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wgiaxird.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fwwlhowv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uiqnueoh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2enwilcfw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jxrhpxhq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cpvoztpd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mbiitass.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zcchtcxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eyfnonfm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2imxiezug.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hpdojjkj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uyuvwbsn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mczlxjza.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ergjbqzt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2evhatjgj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xclpsdwq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2izauxjoj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2upyurrti.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jjytwnib.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzqkzpzo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tvjnnjmy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2eqvhauap.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yxtgpwum.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jaofvrbx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qsxlvizt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lumtcbjb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kyqofjoq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2sqxhmupr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2viyspfhh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vvkhzjar.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2usmsabpk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vdqjmkfh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dsniwaxe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqpjuoux.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qbpgxrsr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwjjvrzj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2momvudaa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lcteydvk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pyqzivfh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcquqeua.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hzgvydbi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bjndeumv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hedxsyro.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pfcsylbs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ufgubaqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2erfiqkph.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufvcfuxh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nyubzljg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2czudfkdg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sdtilzjh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fwcdniuh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fgszwtny.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ignrrish.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2adwahima.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lwwvkrni.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2thooafxq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2aewwuuxu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxhvtacz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ivcdocox.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyumbnwg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xdtkahmb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2udjluekn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lxbawbdz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2igmyeuzn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tjmiepax.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hxwpdrqs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2terghyaw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cojrvbhs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bjrlzwgp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xdcbisan.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pmvnszrx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vmzowyje.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nkizcgkn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jkqbgxdu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ixzeqltz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cakuwvtx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ewvjbarv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hkmxweol.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgeyhfaw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xvkhkhlr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qgimmvzr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2azoylyzs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2iprbuimr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2piuofcqx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2knwmhtmn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nqwounfj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zyzmjlto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqljyjwd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jmynfgpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnqtkeea.html


<!-- 参考信息 -->