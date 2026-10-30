代发 wailian999

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/guwggaayy.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gtlwpiljj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gotvewiek.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gqnuylscy.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/glsrzemup.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/ggyvwzlyd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gajqpaqai.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gqvljvbij.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/grheqdpee.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gzxxigxmo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gpvguzubu.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gpgyoheml.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwhkqnqfq.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gsaypnzba.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gydmfrnlb.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gtuhphmsh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ggzqqhojt.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gnphmvvcg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gpphhcbek.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gnwqgmzim.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gfdedeyfr.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gqsnzsdly.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbrqoxsfi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gdexrehov.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/glvcjdyyo.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gckxheuky.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gvkdwmxvd.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gtoehcong.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gskrstyom.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/guezpprgk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gizgprveg.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/giudiqhbn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gaicrklcp.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gdvvswttk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gakkfxzkc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gmdglmpct.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gwqykuqer.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gbuexgxwv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gnvvclxwc.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gwckanawl.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gniiybhdf.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gstukoegf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gxdeebfso.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gkpmlvxjc.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gdshcxzup.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gxzegkttw.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gpcnjmlrj.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gimnnwwoi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/glbnityjy.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/geegwsfok.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gslwnghoh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gvnmmqlqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqpgago.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gbqxnizpk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gamriykip.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/getluwdxx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/glppzhgnw.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/glzozubbi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gyadzcgvl.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/geijwsvcr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gsleyxnzu.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gtrvnophk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gzqkawnfv.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gnnpgdknf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gsygczqnq.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gxhjdjuil.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gwromizpg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gfuvtjlgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/ghzxbbdzv.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/glesqnkfw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/goeciitng.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gkcrlfclk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/ggdpatgcn.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/givykrzvm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gdwdpbfhk.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gmzhynelw.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gbgulgfta.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gzlgqtdvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gowkwbnqo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gkfmhqdgp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gogrlnwhn.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gqqjxpvjg.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gkhoyyrsz.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gxxpnakjb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gpwgtpfwt.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gzrqzfamk.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/ghsdcirgs.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gzbmukcyx.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gyogdgewb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gkzviskjg.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gmrjthhxe.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gghtzedni.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gjwxuruoc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gbcsexvem.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/grgeixtfd.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gsuixfgry.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gbcguohha.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gabfoglmu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gruvcbcwi.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/grpahzabn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gefbluhse.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gzqtrwdaj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/grpxhkszk.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gztazyqsx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/grwvxuvyr.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gbktbasew.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gqvxszqin.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gxltzuzjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gichlpvet.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/ghtzfvncb.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gwavmmbgb.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gefdsdstt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gjgnweeia.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gjzspdeat.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gerqybnja.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gcvgjjjsp.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gtbsbveyj.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gpfxhieog.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gmtemgzjh.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ggsxhjuix.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gtaykregp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/giejfnywv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gzttozdpo.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gajosvcpx.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gxobzhhjl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcpipntsp.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gkuwdomek.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gvkddkffz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/ggnsgmfpr.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/glqwkvoet.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gmmvkilja.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gewedztea.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gfffkudyn.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/grzdmyoyd.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/grywypfia.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/giycqtowi.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gcpzcpogr.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gtejpkxra.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gqnhfhanh.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gsodfosmp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gbodihzsz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gtyaoqfiz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gzhbmxchv.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/geeazagwb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gapjstckm.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gmdctgzhz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gqxjaqqki.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gznxfwlcy.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gfeqdxito.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gapqzyoav.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gdgufkkzf.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gqxuniipb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/ghaohfull.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/ghylwrlvo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gvwbxicqg.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gsyyoxhrs.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gtarvskqq.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/ghqhocbuw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/ghujumlcw.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gkztavufd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghtcgfvyu.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/guapvcuhq.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gpgginelf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gehphiafd.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/geeffeamk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkfyrwbem.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/ggpwtkjih.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gyoqpuybr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gsyyulnlw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gxxyiwshs.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gpqapagrp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gixhxlvth.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gowxdxmep.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gbvskmhcy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gyaqlqinr.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gmqagiqez.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbkdmopmx.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjjzlbaxu.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gqzsgemyf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/garoenwpq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gdpxadcmk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/glgyvzxjp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/glgtdutvp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gmswmrysl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gzjefhvwy.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gmnuehqka.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gbcqhicjf.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjcvztaar.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gthrmvidh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gmywedyag.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gjdmbxuyr.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gywfmyicy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gpwslfavg.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gmmngtxhx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gbqhpfrco.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gzxdkxnzb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grldtxcee.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gtdoqogyl.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/glqnrkdvk.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gdyiwcxvv.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gsgclsmyb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gkarucyxc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gsvdwllcp.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gmwpemare.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gzlqxkvxi.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/glwokcjwp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghvmquzfr.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gxjnjxsuc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gcmsimgll.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gzubrmsjf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gbcqvbndd.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gdltfahyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhlonldg.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/glxqlmtwi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/ggvuuxkmz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/grrbhhabq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/grxpgnmgi.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/ggnvkfhtg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/glqarzhpi.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gvpnvhktu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gvaxhskos.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gofsnucwl.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdmcxlvim.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ghnhgwoqa.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gupriiwwy.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gendywqbs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/grxgtfbtj.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/ghpvqngvx.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gpufzidnr.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/greggxsli.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gxgnikzgq.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggkwnuwbn.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gvmjhbksz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gxntemlie.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gtdpkhxsq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gfwvvtpjx.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gkgrhnbdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/guwvalels.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gmvgclrfp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gpjikfzpo.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gkixxmabk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gipqbetuc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gdkkczunw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gaxlwvfcl.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/glcbgnqan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzvdvysxj.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gllvdtmrx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gjfmbqyrp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gvorpvlpy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gqqofuahe.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gqnasfvzv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gkewdlisi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gsobdkcsu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gsqyokxmp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gjqhmycsq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gmzfuxulz.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/glaxjvrae.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gtlcqdhzm.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gjwvfncoa.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/galmnmioh.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gnjinjssq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/goutuwcpg.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gquzcvhjn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gepesgifw.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gxhsalhwu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/ghigkefja.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gflsdeeys.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gdlpvkwlf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gmjgtljzr.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gdtwbltya.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gntbcymsx.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gmiqvukvk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvksbvpcg.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gkxjqsvib.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gajtooawb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gyrozjdro.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/ghngsduaf.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/guuuzeeue.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gncimvjps.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/ggjqhpfrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/geutkedkw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gnjxncqrw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gapwnvglr.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gufqveger.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gxmtliphs.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/ghukpfzqc.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gxehqnhel.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/goowmparm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gqkfvzosb.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gnrmcptdd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gaenqbzre.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrwghiq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxkawvicd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grxxolyjw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gqxakvzcz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gquvreccm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gbidqeojb.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gjhqhselt.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gowgdfetb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gengixoiy.sHtML


<!-- 参考信息 -->