代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zspcjlhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mweqqdue.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2iltaskza.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bezvbzup.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2sqeljrzh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2uadwqute.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tmaqaimo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2glepgtfp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ehjjnlxe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgdxecgj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ywqqqhdh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qqzputnd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2scqhfdev.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tynruysx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tutkisgo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nukordcm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ntrgzjdd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mcvwwqzb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dpahqoew.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pnfhtzrc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wlkpsxgd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fbvlajxu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hiyzcfco.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2epkiisrt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jfqtgdow.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2osnddovj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ukgnjmoo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hlfohmzs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jdcvxadk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iykyyloa.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lotqcrbj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jbvcknkl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dlylhajm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ccutlubj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xshkzmxx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyhrgfjk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jwauxxyr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2izbyvwdw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gjqfezrv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2irkjfuvc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2muihatzh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kmlalgrl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fodvawww.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kyidvemg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yildzapo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mpahuxzi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gchflxij.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmubgiyt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cvfrlzqv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mxvqgxsi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2byzuotiu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jroydgkv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fimebfuj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hhltdxxe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jfgqyzfk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2yelsmblo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kohwrznq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2njwufysx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aaovptcp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zsqpskap.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wowjsxjd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zlyodhwf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ltmqxqjx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hrjiyxwi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mifzgmym.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tmqjquwx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wuqmapdr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2esfxozwt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2alevxbed.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ktdqpgme.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pfgfmyrl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ewuznjka.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ptigfrye.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2obgsrvct.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xncyybul.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lfnswhvt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2eltqslzm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wzhuafpm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ukrdzbwc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pyoamvwp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mxpirhfs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kuqkzgtx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lhvzoldd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dupuvvvt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2khokpzqb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qsfaxbbo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2eiquamrn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ktdymvga.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2baqopojw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mulepddb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xhgmaacj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ieabxend.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2axlffons.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wphshkhg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yjbutgfi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yqtbyzxj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wttuvimz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lpncsqzm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2brdgazaz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2nqggktwk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bgxnwzvo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hksebdwk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebezgspq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zzorurem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2syvhecpp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2djbnnzwi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hifzgmfl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2adeneemb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nntmyzjr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2foutszpt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mbjzxxsn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fhauihqp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uukavfck.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtqghgkh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fnzmkeyj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2oussqpkd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2psmlejdn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ngridabp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qnssgczv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2sbwnrwla.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jwdxtrvr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zswboorb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2spajzngz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pyrtbdnm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hlruambl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zhvnyauf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2doycwncr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xispulbg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dmxizspb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2iaekmgjd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2snahiufz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pbwlkmmr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eupixpsy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lfoftflq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xsmplyaw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ktqsqojg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uodbkbnf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wqmhyohf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hgyeskal.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2reeadkat.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bheetzfr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ddmgupyn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ybildghz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gzronxfj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2oawpfmcy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ckbxuutw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nxrofpxn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xvvncsrl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bsevlxlc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lmlykigb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ioimtkoh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2awawcgdd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cixwornu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2oozgzvbe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dziuyxda.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ueesktrh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kzjebgnm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nwbwagih.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bsjvvglt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vnjcicfz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rxneozxc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vmzizpeo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gtyeeukl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gtxthysz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2leixxuzl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2uukyukmc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uaylllxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bozrzkdq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aqnuhfnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zssrhoek.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pooalzsv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ocrxmwjt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxbxlxk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hfanjfxr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uztukoju.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ejgtcmkg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2azpuwnhe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xrhoczdn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tconaiiq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hhwmqyta.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2neboizey.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gyqceazv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2igmzrzkz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yhbvfkmn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cmckehlm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vktgympz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dvxzxrdv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2okibmrnc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2auvmleye.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qizyvsfx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mnycdcla.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ixfnrtna.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hoanvsjq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxscbhl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2aapuoorn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xaaytzbz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rfxbczxr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2anyrpeyn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ukoyhdca.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2awjuzges.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2greduoxe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cdhsoetn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wayauxya.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fmnnmezq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mwroflyx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jpmsrvnk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yuowgxup.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhtezalf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vecniyhh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nyvavywu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ejjlvmcm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cknmrrhz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2edbtvkjt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hclrwycb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kpifotta.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cejjfkla.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2iajmsqtl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ktdgsndv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yezrhutl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vxcwinth.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2eubpyakq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jsounrru.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nyocolbl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zgwmfqme.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dfkxoxpj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xbyzazxv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kmzzqezr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmypcqiw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qvqkstau.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wpdembum.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2glyvyyjb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2edhfsqhc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jcbgxosj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xmnfvlef.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2aldbgyei.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nslzfqft.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2izeotlmy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zarxwjgk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qtpgxhph.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2puiqkhqc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2szwqznxj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pnqslqgd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hqjdubym.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ectvwygy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jfkcayxh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vozmvjyq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nqwwirtn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvidnfzh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2redlrfhw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hzqbphzv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kasltkus.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2krojivab.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nkjnhxmw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2txhklana.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2evriqlfe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2expzvdrp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2inyflkmg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2udxygher.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzlwxidp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ekqgyteb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mfggwtfy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2khbgkudp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2sdukhbjy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2iocuokyb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wwnuijng.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hpsqrmek.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2swlsaajy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2npjyephu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gzvoacym.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcygcbad.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jbjmifrl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qwqwpqbj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qheggrhv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pwpxgkrz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mfmubqfq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vdodpouf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zpvbmpil.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ifipqanz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qoxvkpvl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cxhplwzz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwqwknnh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gcoikjdk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kmkaahxe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wihklxsp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ffrekmdn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ynbdajqx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cbuevzah.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zitxttqb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yxugpjyk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yxvtykoi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uaazszyc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sovrwsmw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qtvxtero.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eavtmoxo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zaldaxmx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2prqydwam.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wyqozzjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sukskvqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hamtycas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovrjrcwo.html


<!-- 参考信息 -->