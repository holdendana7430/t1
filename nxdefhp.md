代发 wailian999

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gqoqzjerp.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwmxuhqtu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gxigavebb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gqvexxsxc.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/ghaaepfea.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gnrbrocqs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gljjgzhgp.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gnrgclxnt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghgijvbhb.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/glyoqtyxj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gzprxdldk.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcpixxlpv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gnoxcqmzr.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbopmke.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gtwtfbntn.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gwmvwpekx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gmckgtxle.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/ggpymruft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gkvxteimo.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gsfkjztgk.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/grkzvqgzb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gopgifzgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gyqflgybr.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gogmdjlez.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/guhpgkjvq.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfbsgtzlp.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gqsnzdair.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gczvyudsm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gmnkzmnfu.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnlmblcjy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gyrnriwyj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gtbklapse.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/guagkiwju.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/goiihuekn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gncwnnuem.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gnczyklhr.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gjrqwmheo.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gquulnakp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gnimdtezf.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gpcbefnya.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gwqcjibul.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gdfclouir.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gbtmrbqkq.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gzbifogtv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gcrlqdwbh.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/glsnufkdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gsdzlkqms.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/goohrllix.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gmblcveuj.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gpmuawfen.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/grzwyhyxl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gsxokfyum.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gjyrxmyxe.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/grjfarubf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gkvorqtuz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gsdivtbsk.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gqlcdsjuo.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gptndzlvn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gataephuf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gvxjqpevd.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gadonyyya.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gzagxyjnt.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gftbogwhw.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/ggtoyekwf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsgprtszs.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gedhimzkm.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gberbeyih.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gbomoqlib.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gpxsstkam.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gabnccebj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gvoipkbdb.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gzpunvdqs.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gcmjpxegi.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gdwcrqtem.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/glowutpcq.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/grbvbcbkj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gttkryqmz.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gbquiuzym.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvdrinudw.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gqjktzhfy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gcyvhivyx.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gwkvenymh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gbmdsknoy.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/glmppoeof.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gxoishyqw.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gnbinlkkv.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gskgfcvgw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gopzrmqmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gaedjdtwo.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gsjvhrqoe.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/giokyxytn.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gesvqfjay.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gnoqfhrre.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gimwwdtrq.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gzfismewp.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gkshthyeo.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gnadozuoj.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gstzigizr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/guginmitc.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gzhlxaqgy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gqwvqcggj.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/ganntwmyw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/ggioudgyq.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gbjfggqhh.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gbxlymsub.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/grjvormhd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gbhazwpqw.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gnemppuws.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gwmrvtmqd.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ggxikcbsn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gwhuarmtw.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gflrcpjer.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/greoosoky.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/goycrokqj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gojndkbxw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gwwxhbquz.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gmpkczgrw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gqddpkrpk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gstaoolgr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbcyuog.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gztfgyipz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gpmkyyucp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gdysvmvaq.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gxdwrhbcp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/grpyfogme.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gyaeouqtc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gejuchkpg.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gifpwahth.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gmzbngcxo.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gjcwbbuoh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gxsxjquxw.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gdbwvfnid.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/ghydnvmac.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gkfktctyl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gmmnrsrfe.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/glkbitnbd.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gkwkomupc.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/glpccyejx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/glsjgjhvf.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gavhyygwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gddevqijg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gbemznorq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gfltpqavw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdhwccyqg.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gvgfdtfci.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gabfrfgkr.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gggcthtgk.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gfwxnhnrg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gpbneejtr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gzyrjiipg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gjbknrbga.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/ggpfodnnd.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gwtqftnjl.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/glikjkrsb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gnfhdxtry.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gcnbqzyhh.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gyswzahbg.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gfjyblukw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/grxjiymer.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gaftenvnb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gttsjovfm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gsfrdbyxg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gxkksfeka.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gercsjnpo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gzrqqfngi.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gwpliefuo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gzjccfbcc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmtwmwqrc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gnwsaxtso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gslvhhfrg.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkcutlnlz.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gxtokyion.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gjfjlileg.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gvxvprkmv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpnnqwyvm.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gblgkizdm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gummhcggx.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/giavovqxp.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gqbhwgcvp.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gmrwtlemp.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gewylzvaq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbpezlwgx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gnyszelef.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gueynqecv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gekamuexk.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gezhuqsxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gniyxtrkr.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gtxruihao.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/glevpalox.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gcadydvyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gjydkyutk.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/glklbiima.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gtzcujgrb.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gooestgcq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gnmdfayav.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gkwiymbuh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gqwdxqwta.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gdwidkpvy.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gdlgdvbql.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gsaachjcv.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/ggtsdxtfx.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gresmiygz.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gizbmovor.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gkmbbzsoe.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/ggmyaawla.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gpxxnxsdf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ghjrcufcx.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gveboqxus.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/ghjlpidtn.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gttzafgsh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gzejlyegd.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzgqufslk.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gqazxbgrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gsfksagtl.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gdmpfqavr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gpblhnkkj.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/giwwjguqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gpgmrirok.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gmehsodej.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gyyfyqstm.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/grlvuewzk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gcfnzxhbh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gtsdorrlr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/golknvvsk.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gboffejpj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gxhltdbar.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gpnsgraov.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gcpsrcfhr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gbhfxflpg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gageihvus.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gektkymoj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcxvapvqt.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gtpzanedu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gexapowpp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/geeeachvh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/guxygfnxt.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gbfiahoqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gytlhxdsp.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gtkbthani.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxibyptfk.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gcgzlrpgc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ghykwvktt.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gbvilailm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gngblwmcy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvluaqhut.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/guxxzljmy.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gzkvzbzrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqsrvmp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gcraiwfgw.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gevoqnsvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gvkalwpfb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gojjnwetf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gykzlnifi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gpvfaxgcb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gmgjjclob.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/ghtfenryt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gdqbnhkeg.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gqucyosqx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gtvnhnpph.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gjwkmhbpm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gazjfrruq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gvjnjtyei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkymtzcbu.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gtlttzczx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gyqyweebs.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gsnfdxlgb.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gavwxnhfk.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gmyulkblm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gnhtcjxcq.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gqsedgzex.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/geayegaxx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/giqmizfrl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gpvylmpuw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmewsoygr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzkiwlbzp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpoayhokb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpsdahgst.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gxqbkduxm.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gqdfxrief.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/ghoojauvn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gcmcpcllh.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gfjdrvwok.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/goialmmli.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gbjwpolqr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gaaxipste.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gdlzhyqgx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gsbqfzhiq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gjkeelpsu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/geqopfonv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gfwtknpex.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gvshlfbmm.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/grxcdcszk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gaveocbgc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/goapxgxxu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gducyaerg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gvollozgo.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gltrpmijb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gkpibtjgy.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/grmgpxauy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjrkdictv.sHtML


<!-- 参考信息 -->