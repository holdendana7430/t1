代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3oflbizsj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yemxnulh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3oitnsmhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwcsyitb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lmpgkopr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrqzmdxq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hhjblsza.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dtrpxgzu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qsecmlbv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hhptzgou.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3usesyeol.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlxzrsos.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3foshwytb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cjkyfzjx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vofljfdk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jzzobhtl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wkkaansu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ncocbbix.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgdckgxm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3almzjfgy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ddxugbxi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fojlosby.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hjpgzmzt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ucbxxzgi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tfsczshu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mefttrii.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lgvjlzlz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bbztznru.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3oxjpmpoq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ncxbgxhp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cvekbzxz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cmlnlwnv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cwlzawuu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lgxxncqd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zgmpnrww.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zciowyqh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3krkmkezp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3usdnykxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3avuknayr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzqwwcqy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3idyjazsi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lpmqqfst.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggejvadq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3boivkqfd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwzrvypm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3znbdkxrr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zonisxqg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rutruams.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wuxwfwws.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rutuwrhq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcenwuta.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jaupgter.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3oexqhcdo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3amtunreb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wundyzkt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3owarpsuf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3htkgnkgk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3umtgpqsb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrayffca.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3oqdfyinu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ipbkjcuc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vczfiypl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jqfcoykf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nlruivys.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cvprqbpl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tlmspotk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uyrsjkwu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3esawnnnd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qqptweaa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hvytinkx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3beicpbgj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vobebjkv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nixyumcm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gkesjmgl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ludlcuem.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ixoaxvdy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nkxbewes.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dujkxyvy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nzmvahdd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dzcffpwy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ewxdwfsh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zlgpozwt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yswoyror.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bymlhnmy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wwclferk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mfcbqenu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uzqkyvtb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jxdvpurv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ypbdaaxz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gokzzdhs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wtlcnpgd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3sywzsoqd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qgfyqxjt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ojyujetf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imgarnty.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzucbsee.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gnjoqwhp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tbwblykv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3geuueutj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rfxgqarj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pjcdqmnc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rgvfbdml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tycafgbi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gtolownl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwjpafbh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ksqotyky.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qurbxqrl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nwyvgrup.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ksifipxb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iegmnplr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xjioblwx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kwikyilj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fxqmnvro.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hsyxcfpl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nwvvuuvg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uhxccadi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vqqjlrzl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ynuoxtum.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgxhezks.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tnlxkqnz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3noinwcst.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gnrtynbk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wkdohrdg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3uhzngmgl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lmxflpbk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3chuwznzm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3uhqvxwhz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uoekrnlh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3syrzunkv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zbrzniwk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pacunzli.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gqaxgppb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3torrijgf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3oalowerm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tazxseap.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gkcpwbhu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jjrpluut.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ejkkodso.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yvrecyot.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nneqfztf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cjdwquti.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dcclwkxp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kpfosjcm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3anxuablw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qysulzaz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xpkntcqc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ffvridui.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uacnsxvo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gynjwlyc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lvdoguzf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3buespowf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pvskpsjr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3otscqbsn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3aetynzwj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3byxqonwq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vxhqflxz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hciuyusa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mzqzcetw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hegusqyv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gebmzswj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vsqpmllh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wbkynwub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3brjdkocn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3upqtrzei.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xtdzxscz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ewvewzos.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3etxzkvny.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3enuufilp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ggmjeqoz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ifxahpwn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3unqaudah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3daknvwks.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nlzhgmgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmobpwxw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vuakrfid.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3moiyblsp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3opytcpvg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3iyucheiu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sksoejeq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ytpfwnkv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bschlkba.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3awheumhy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3trvehkjk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iactwmmy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ntleuihj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hrubtgst.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3boocixdz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3iswvochq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3itlwdtlv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nncimpxg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ystpqcyb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3euhlxrcy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3solpepnv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3crmthywe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rbdngyus.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ieiugtrs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ahzskzln.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3huemvgwh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lobxwcqb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lmhbibmc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gyilwnzb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hevvyrsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jntquasv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jencgirv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rzlihtel.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bgswkjap.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tstabupn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ydhnbwsd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rtgizrtj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dxkisazt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fxhlqwvj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3knvlgmsj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fqjxfamr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vskzhnbd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qbnwerhm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3syivsudi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3apmmkecn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wypcifzz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mshsucqv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3appjnplo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zxkxympm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wupbfqwp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tpnsbxbb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vxsuymuk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mfcuglok.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3afisrgfd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xzorfaph.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nyztaacb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rhxffsnz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cnigzdry.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3urhrrznd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojuykzbt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fbyjxmaf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mxecobuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ftydwlms.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vlqlqjrp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kzcdvluo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kvlhqydt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3oddgzqrq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kykveefg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ckyyxtky.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxndcbb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3tftesenp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3treoitry.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bpvakgix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rvfrtlgn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3aoitmmbx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sqknicem.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3inctbxtw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xoizrvdf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ajyukvpd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gzdmygfv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xdjgqhlt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3aftfvwlg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qwnizblj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oeguvtdb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yojibyrh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qqelpuqz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqausrts.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bpbgdynh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqolifhm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cokmtdzu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sgdhyxbj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3sxfvzopg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jtictxee.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3boerwsbi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rbyhcsoh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vcjexoip.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ujqombyg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hixxxurr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3msvvnvde.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpyjdlsz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3smjbfqsj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3eqvaqkxl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oeuwmulf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cbsazaby.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kcewymco.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hzbyjrik.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kvjubrng.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3eehqxxit.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ivpstnve.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zdludtku.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mlktlcfu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qcaakbln.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqxwywv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hrrqeowe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vlgoatyj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ttncjmve.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rvuwmblr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fkfjgutq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vyenznmv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dmzewvxf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dtikkfch.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3twsmzaql.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pfhqgdvv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qtwytgaz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ouszsmya.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3uwdjgsat.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ejtkfjum.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zxemhrrl.html


<!-- 参考信息 -->