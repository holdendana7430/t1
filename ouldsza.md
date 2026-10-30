代发 wailian999

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/grujlfgvo.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gnuexqyeo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gckzynwzx.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gwaywvduk.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gndppqyze.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gdyuokswl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gzfyznaol.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gscpnlbcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gsbztkxxa.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/grhdtkdnb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gcjvuyady.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gxbthwdbq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gdevyznqc.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gcnnaphds.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gyojrfbow.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/glvfptyxz.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gepemxkss.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gpivwagsx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqausmaui.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gyxatrtkl.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gkzbcrtwj.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gskjccatr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gqsqchkld.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/guasykprz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxhgdhhrc.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/ghvmrkees.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gslctascq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvussbkxd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gaqhlredp.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gdvuwinns.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/grlcfxzet.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gagwcradx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gclifmzpd.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfixlfdfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gprjafymw.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gapiojfem.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/ggoaoiwbm.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/guemuxlsp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/guvozlrjy.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gvpbqwpix.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/goudofdvq.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gaqjtbenf.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/ghcwcvvhy.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gpzzbzoxz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gklvsmbfe.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxyymkirg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/ggijdfduu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gluawsdzn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gruokitis.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gumoenwcp.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gybzcknri.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gcufbllqa.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gplboitsl.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gdtvcwhnp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gtjvehcfv.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gfcpxyngo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gochujujv.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/grajpbitk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gksemywrq.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gjtlkvbpg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjujmgumv.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gcnaydhkz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gvekczozh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/grvarpbjh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gjmxtewij.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gnkphjqgr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/grhmyspcb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/glmddjmew.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gnnbjhumi.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gujgeehab.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gghinksgy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gokafvsui.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gvrsiltgg.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gjhapmmtn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/ghcsivloe.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/ggehiguex.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gxucrzzep.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gytmjqvrn.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gwtgkoysy.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gyzaexduf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/grimtqgig.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/glbdizbsc.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gsnxdfcvs.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gwbcnpfqh.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/grsofaswq.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gpbphsfkr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gxdknjmxz.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gxmrrfoqr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gcytyghku.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gslrnztfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gmmzxpsqz.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/glyftshnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/greyrrsik.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gatuitgvn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqjoillqq.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gjrrydklt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gphghgasn.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gvnrkkwbq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfjoezjzn.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/grocnouue.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/guiwkdthw.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gquhfviwr.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gulkoztfo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/geebgltov.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/glcopmtps.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gcpksjnsu.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gbtwglqjf.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gosubqnac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gtgaiewcu.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gczwjlyli.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gvtkjhkkj.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/ghmrnvfsn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gwkqakcku.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gdexsgwzx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gvkyknzjs.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gnyeltxll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gaoealzol.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gxbfhggpg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gliibndnw.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gxcsusvfx.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/ghtejskpd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gxixgmtzb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gymqucaiw.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gdqfvcuyt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gaqnhbbfw.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ghxmblifl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gjtibmnxo.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gvamnwrdw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gyvgbhwdd.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ggsrlnwfq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxbmazf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/ghvzfccsh.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gqyldmryj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gvmgejaep.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsyhfijcf.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gpnfmrpvc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gofjyilvi.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gaozzsqbz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gqmorwdcj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjnyknfrh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/glcotmfyd.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/ghoeadmbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gdwetsgwn.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gvafmaqef.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gclaepfnl.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gttxjcfwg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gcbkemkpi.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gurhljeii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/ghuyetmai.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gvtisykox.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gikrwrdko.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gooqgwffu.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gkwyaiaju.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gboartqsp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gxnfmzbal.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gtegwofhi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gxiekedqp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gokfdbakz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gniptsqrj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gudgtxwmn.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gttvehdsx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbtvcjmls.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwfyppfbr.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gukqddqev.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gqtonqstp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gewkucwfj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gbndhgbcu.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gunqgfoon.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gmmthnjnm.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gqxmwczpg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/geyyuzzfi.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gvhkfyzrs.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/glahmecvb.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gkjzuccpa.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gmgocjggd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/geqhddvxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/ghxwfvrug.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gceatjkur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/glzvpfhid.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gtdaauwld.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gpqecpbjg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gsqvyobix.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gbsnsgprz.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gooswxsrr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/guvkuynfp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/glqbhgohy.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gjltyqtxy.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gdotejssa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gcjjtvcoh.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gcmybfgvm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gvbhnorhy.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grvmyaapi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gxlmcipta.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gsjytztal.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gdthbyngc.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gwfndozho.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gfjssrkhj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzzugkltr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/ghkgoagyv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gwwujhtqe.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwrpyrap.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gbhfhlfgc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gzlaghhun.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gitydmdkw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/geixqtjur.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gmgmluaio.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gmiwyvjhx.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/ghtrvjuct.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gcihjoreu.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/ghmdxstxx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gywxivtvp.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gywxouqza.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gezbksyol.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gmxylquun.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/ghmcvgpmn.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/ggcykyepb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gqqgzqdio.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/ggrfuguvv.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmttgqqhc.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gsshetbba.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gipzcsgeg.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gyehuhsve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gvifxqngb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gbygjgvoz.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/ghnymbkhf.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gwayugctb.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gdmuqqxac.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdkcjtfut.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/glmkoaknb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqadcyjfd.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gmsgnycmr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gjsqfimwn.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/grhfnwxot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/guizgdlna.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gbskwbomx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gtyikolbv.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gljrnmeiy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gehrjvvtp.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gqfbzcejt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gduhxlvxm.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gqyuertte.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gbgewcoaf.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gmfnovoys.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxrcztaqa.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gymckvgsr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gpuhyibfe.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gzpfuaifq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gyqrqhens.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gytqlyhjb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gqqjttpkj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gaktrtofz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gpscwrrpm.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gomlrxpxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbotdzxmh.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gomykzgio.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gcrgpfkpm.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gplraqwya.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gnhwilmdl.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gfywzwdzo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gbvkuiaql.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/govacpeuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gnlsquwgb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtgsbakye.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gpyhcvaby.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gxcfnnrym.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gwqhfmidj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gvtekslpf.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gzcjojcpi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzllxlruh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gjruhaapu.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gysgnrpzs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/glrnojnpy.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gyuqtvxjw.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gqmfkyfxz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/glfjubhdk.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gcepkbpyq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gukqiduln.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gteifyrnc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjxktrvpm.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gxmypydfm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/ghcaoprar.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ghdugcclr.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gsyktyoba.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gprdehllu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/ghdmphlnw.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gnncritgm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gmtfoobsd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gpewjueyh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gdfgsduws.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/getamkrjn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gleavhmhj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghbgesaah.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gnogejdwx.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfelqnoco.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gectzqzlb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gcylezehw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gzxawtlzc.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gjwgebayj.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gitimorig.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gzezcxobo.sHtML


<!-- 参考信息 -->