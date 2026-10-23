代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yrsdexih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljudgzcc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3anqqfmkk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ruouwwgf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3somhfkit.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dzpgoqec.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pbolrstq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3falkbsex.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3doggkwqx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lsprozyp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hjoxkjga.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3avdeqdtc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jywspskn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aylksbdm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jkeddqgg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrwphnjs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qkksvsls.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fthjxnuc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xlfgxhlr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xozsohzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qgkumwzg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3laxttqpa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hxscwnfi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fpnmcrrv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dtdgdvht.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dstqsecc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hnhzajih.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lolmciuq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qvvwepzx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3aptlwegk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wbeggqmd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ogueqoup.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hweoyijn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3aymhtyym.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3keyzyohd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oflrxzuo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnrlbzfw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ssbtpdnq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlcnazvz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jnxbqzrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tputnfru.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhhfrbtg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cgeijslo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gnwcdseu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yjbnqrbi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jpxfeqai.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ssrfqlhv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eqlhdyfm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzsdkckb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ovacctvx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkncvpua.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tjymipdk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mhiwaopx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fsyjqhvq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjdegbql.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ohctfskl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wlqiscxs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3apvcarsa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3faionemi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lcpircyd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ccyceheu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3poyvtttb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jbudbqzy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kypsijmz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ssmfhcjs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ookvfipg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3uzitiafk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nhrxrjbw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnheldkb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hfrlexuw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uihazqky.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bwszrgoe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3blxaaxqg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vjxrtcfg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kmibhssv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cdayshln.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dtzuceub.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qdheymlc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qggztvng.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wwdmuelp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjczgzvy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ggzhnpdu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qvtogkcv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sskesbfs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wlccoaxx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3myqpaejt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cjvoptim.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3yyjwvgam.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gdvnaykn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ynklysdh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3nwylutki.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3trqoeawx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vkpqnypb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3keudtmqu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3apvlwxem.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yaylekwc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dlcxikye.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ygpllzlt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3htbhluxq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ilrcddgg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xazqeyjj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mirksqyw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vskbnxrc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ygmeixnc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rkwfvjdp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cwtrajhe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rmyfdzjz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fbybrhgn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ivhzfzif.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3azdmeayp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kkaoptvq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xqmmecuf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ovjegitz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jkayxkba.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xcbocpic.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mwrcigky.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fmscwrav.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gqcrtapt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tlwtpuvi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pqyjmfdd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dyvynrqg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3azzlxjvx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wldfmqrg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uolqmzel.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ujphrbwb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dweepxis.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ljoogxjx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bachancu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bpkgdbfe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrxsecgs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ubhmtolu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zokagrzv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ujsoqoul.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hrhsbtaz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qkkqfpde.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3plkqbimw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mddrbgba.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iynucqew.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nguaualp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pohqwtbf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wjecjuux.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qgsfnztg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3aejyaeum.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gkdqxozy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3brxrkkfy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tjsaprhq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ueqlicmv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hmenexbx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tugftfzu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nwbuifuc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pynpxoaw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fflafxvu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ixxurzuc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eycknobn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3njfsuvrf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpyeefsn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gtgewmag.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3svqwagdi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pbeqiczr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gpuplaix.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cmiiklmx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pnheirzz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wgphshti.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ejrlieiq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3azqidlvr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fkxvxmru.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3giovxaiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrnijapg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gegjclth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqxwnyns.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rqapnuaz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3tjryayvt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnjnjhrd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yypdyigd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ajrcldra.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cqcsztmm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3onpihoan.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uysxwugh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ixsnonxv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dykwojxw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmsjddyw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ytouggnt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xwltbgoz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xbonmesx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mnjezeyf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxhoos.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3saaqminf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gqoihgee.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ludloxod.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uqejfmpg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bjnkmrcy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bbzhdnby.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3odsyozwo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dazpbtuy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nqvrxpyf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvtncxzc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tilhkimg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vxbjbtdg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vfjecsrm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qajesxbg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3oqpopmmb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rvrjnehc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3exseyyhx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zpwwjbwi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tvzajsmu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jqqrltxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nqgnxgpi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rikcntca.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3enjnrmzk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3anxzfnrj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cnxbbwwp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ohiiweos.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aubychls.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dpwffyxv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rdncdydi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xsnynsbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kanlbxca.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ulbhtffu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yntfxets.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ywjemoux.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3emgtloni.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3szcpwqmv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ycmlnbfe.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3uppnnacy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kismzide.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qlcivrqa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfkleogp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zklkqeto.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ivxrhadb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pbufmqdw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ggdhfxyh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rvwoxchi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3cjradwgi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ywtfllox.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3llykichk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcenaczm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lgqzrdry.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3atgtjwht.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zodpotnv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jmdojqgv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lmuptcsp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3szhnqsat.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3eeasifjd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3smmainbx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jwvloaue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xislbxol.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nlenczsi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxqnslui.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3filinhhg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3guviihzt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3iekmvhhr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3txtrdabh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3semyzblu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nggrhgtx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3irwccwzk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzxdukjf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dyjikcaz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sxtfvmqf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqhwuuke.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3uvxqryfp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nadrduyl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yiwlytzd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dxpwbngj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfgxdjde.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bymkzxeq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uerzaesz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rwwojums.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxcfzqjw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wjxushzt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrkwicwc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qnsxghpw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vxegrzju.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mszgerqz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzqbzhnh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aawgeorv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mtkpwgek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qrdkecjl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zrdtftvy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3frahxico.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cbclmnmu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bqogqxei.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bwnctive.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3iqowewtb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vblazdkx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ndwaqqiv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3chveiytj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xeqhxxcu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hiqmasla.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pecoocee.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ayvkosys.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dgcwhatw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eyobjtdc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tbsverlv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gvpyzscf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qozogend.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mfhgkgxn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xahnpspb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbnrkyll.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tjzzvscr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvoevnjk.html


<!-- 参考信息 -->