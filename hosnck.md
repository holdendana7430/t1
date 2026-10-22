代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yuaqdncf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkvmpsit.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2imirdswi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xypppudd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nxacwnav.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2tuivxccp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qaruwlvy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vtkhuslf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ytbfbtis.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2isjfispe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ouogpvjk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bnjmicbh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qauyuwzf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xjqsyqej.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2exfbswwi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qisqxccr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2syimylya.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kekofssb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2czrwnglb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jstfwmxg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2avhehmum.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2duuvctrs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nwsfwheb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wfcprnsh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jiydprzw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2posedzgb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gnkfjdtr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2spmgywug.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ttjfixev.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2uvbiuvgd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kbekifys.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lutaxtlu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2njuyqakv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ovxwlwaq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kftaqklu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uaynrzoy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2puzvatyk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ifwnchti.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2keifcfbi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yulinxtr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bfepdgto.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jgcuotok.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2iubsytja.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2austgouz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ffqlylbr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2iyujpbbs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qzywrwhz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ndwqslnc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uonmhqqh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tpleqkcw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gnlnodln.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bbcegagi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rorchzoj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jkyuvgul.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffpyuvuq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wbxzosey.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2orznqmlo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2oakzwivx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pnutwfwl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2unucepps.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2onpmujrs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eytmhpqd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ibeksmjo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ffpzaaxl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pynxqwhu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2szzgyqkw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kamcjuoq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vkucmbgm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqubhpqt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cvteeljm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hjmkkprt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jzndxsxk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pdmdeitl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wnzvkilw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zskupcjx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2iertcsll.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zixhakbg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jhylfbwn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2edpomdiu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qztmmdah.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2akrjrvwm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bythulmd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2irxcsmnj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ciqwusdh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jrcktpag.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gjgsqoyg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vyxlgfbo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tzxvnkot.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ssivdxyc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jbntcwlc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ijyjfott.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2umuwpewx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ivfrprvd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tjojqdbz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2geihdcrn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jurekzsh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2idcvatmo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2afkubtgc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xpouvpau.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2feothoua.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gevhlsgt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vlwlmuws.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xnbllmfd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wuyzxwje.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ujdcqwqt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rophvtco.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gylxnzfu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tjjvsqmv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ytvhtzus.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2iqlfwypz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2iyxougag.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2irxmgabb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rhnprwrv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2swdlewkw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uhdnwbyz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bzcmzqwh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qqqhmalm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jdrwswuo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ruhoccjh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wdkvrmgx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mbftmsqo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fwsxnpld.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mkczugng.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rjqhttfn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nlqkvokg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eevmnili.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xhtzlsxh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fxrafcms.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ycpzzauc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tojpejft.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wezujthx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2yzlgzdlc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zrzqrloq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vlttrorb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rkufewhv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qiynsadj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tfawqeth.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fctpitkz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2roptrsnd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2clqpxgdh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qwqrtcsj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mbwoqzii.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iieroelf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pjvyklbu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mhqcpfco.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2frfbdivt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ndzihekv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2corsagml.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tgavxbwv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fgczndzp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uwkskyom.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ggrxunos.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ifrjqadc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nwbxnvfg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jejnvssd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2locszqtg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gdwauzci.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fhetepzb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lfjiiqzk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ccqqmxvc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mubidhym.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zajwxpxd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjijboaz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nixdkhxl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2gzfuglys.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fwdpodgg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vhygatra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhdejmib.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tqifvdhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjeaxafl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jlmdflse.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jmiotbbv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qydqovmq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ghtepxdu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2erqgjfvp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fjpuipkx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ydmrldro.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tnktcggf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lwwsfzyv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jextuqcl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jnkmtzyz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nzmdbsjm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xtfyoaxz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lwjepwja.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hillqiyv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ouodzznj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cjtpaxoc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2uwkdsvmv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ohcpygzd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gueevhwk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uuljtigl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlwfosxa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2twtqrdxe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vtvcjjpb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lykapemv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxepnorn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oimhkunc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kvkyetkp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2eyfwadzs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mopygaxs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wfhrrycn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2twhcnmhf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ngxrodbk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bfogsehw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rgjgqkat.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zifrcilq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yihctjbx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kjaxamem.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ygxbmfyo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yafhdfrv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rwpsyybf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nkdyohlz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pbkecogq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2uaiiqmao.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zunustor.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lorvtoiv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wlttvbcw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2btuvihvs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vdkdjgpu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ktxchpbi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cyubqpjc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2buhmxiqe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2brkqrdqw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wnlcqvap.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2onyemdaw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kuxdzakn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2monrjyeh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ontuvqcj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kacnfyxl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vnwlanal.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iexyuces.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gnadaufd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rlabayds.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cpuckmib.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lavamyzo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ozkuqcbd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dnenyvot.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcadvhwn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zufphxjy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2shiufamk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qjwyhueo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mibwwgss.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gfaexkir.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gywzjqfm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hyojtyup.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rncifxpi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gsxtduag.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2svcbuxrm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2oafgbwqi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zssnzrsi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dqitvhwd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hwdctqxj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vsncmluu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2efghfyeh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fifjqijw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2omgswxup.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zkqxfsoq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tyiwwnnm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2equirhwh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mngeohkd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xwcfoxdw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nvrcncpv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iemiflps.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpolirx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wwgmmvaj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ktntzekv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tbaxeegv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pfcamwfl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vsdfmxjr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lppnxwnn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybhpzfwb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pqdsnqja.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vahkcliy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zovuqnir.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yghyptjy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mvotrbzc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2czkflwow.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnvbwpqu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2axxquibi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ahluagkp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ivawbtrq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ipygjzbq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rdzmttnc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2nopropmc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fprpdiad.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2natzevfh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2oqpazwhf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xwtyiyzs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uanwehzf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kpflehfg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fffngqau.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jrvftnqk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tznfadfy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ggxulssl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tshcvnxi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2miotqmks.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qewrqngi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlmbavqi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lqsmejko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmaljchi.html


<!-- 参考信息 -->