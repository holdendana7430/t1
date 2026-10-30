代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdexcvaia.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/geqwybniv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gqsuaovix.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gwkopwggw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhuwzmlx.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gyjwxrqzp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvgnnuie.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gphsuomdn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutmqlfie.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdixhktwx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/ghvxcyxil.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmtwtzmgx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghponktid.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxqsbaor.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gesjrfjxf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gleochxan.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnyvjgiz.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/guubnnyub.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbtzauwh.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlkhkdss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdbufdar.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvisdmai.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gxevahxja.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/glxrreqrc.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjvplxao.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeexjkys.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyeydwxd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gxiupmjok.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnussbgso.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwpyjey.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gtxgwqzmx.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeryzgpe.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvtsphwe.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/glwtfcygu.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwfjnlby.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjowlojg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnryzlpy.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhrbtmjf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipjlkney.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhvbarop.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ggrlynnwh.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnyrkpyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapwecvai.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkufhgggj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtwasxjj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvjddop.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtflcempd.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggcryqpzo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzmaqnja.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwohgdjl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goxyewaiz.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gbpishmgc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gsslpgynw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkvkrrau.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbvwmmxnx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqcmkqji.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/geavuhdhu.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmdscpz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gswznmwtp.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/grvskzahr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gbcvirwdf.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzewxyepq.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmytmnygn.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gdaljtenv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzthinyxj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnopzcueo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/guzqpihmc.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/graknievj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gksbhuewu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhxlibek.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyaidaoc.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpeylrfff.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/glxwusfqw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwaxrush.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtsodkuw.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginvqncvx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gnyrlbsjs.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gliqlesht.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqegtrgp.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gztnhrtzf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gblzizlyq.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gepmlpgnc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvucogfs.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkagtslna.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfcpfcmm.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdohgizjb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gotpnlnph.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxniksnvu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getielkbt.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gjunbhjla.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqthweka.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggxtuflld.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkpgojal.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyrzsrcp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grlgrfnlm.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfqcgmzu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyforbxz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gfflqwgux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnxncluw.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkknenhjc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqjxcxmd.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxenblteo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkldepii.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/grzpdrvma.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxsdrams.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzrdrkyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmzjfukq.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gllyqyoze.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhxuvhlp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/giqsfuuly.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gvflcqkta.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmymlgry.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvluyflfg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjccyhqg.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbelggqna.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/grhlxnicx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gljjeldbn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/glcbczktu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvzakpem.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/guibattzx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgxatkxr.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gforfpanz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczaesyvx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldcuptrx.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvucfqthp.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzzcawyd.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gokchjxps.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmavsqqtx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gwtumtxeo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoznulra.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ggqzkwmyg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gkemhwylv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gacorrldn.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyzimyvd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gifezdgtc.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnlymlifb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcepekso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjevemzy.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/guzvmhlxg.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmqwtglry.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gugtdtgaj.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/grkbohzvs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgdyxpfg.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gfniqsvih.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gatwxdpom.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyepyelqv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdsnbohq.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtluvwxqo.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkitmhtkt.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacojqzbs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gytmvskgl.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glrzutmep.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjmjhmpj.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvveygjkc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfasccrm.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcztcdngg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoeayylk.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/geewvcncy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gygfidlno.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznmgjoiv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqcimlrw.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gcknmhiae.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdmtoeaxn.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsigxevrw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoetiphk.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwqrcjc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukjceajo.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxwapmmv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/greqnonzc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gipxvjgoq.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcihmzqlt.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntcqekob.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gfhakevnt.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gaxmcvxbm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gffbpancf.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gqrrmlbqo.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvqhblgt.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gabqvykjr.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjunewkw.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwidetkyf.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkvozpf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkpubunug.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gupdsznhy.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmfrmxk.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvouaiqm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliftmryu.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/glrsbupjs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gelripyqs.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhtdfzav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtjmvjdam.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqljykhf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyettcyuo.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gnqxeoypw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ghvfcojsr.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxsugvajm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gbgshuqwf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzztafcuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwidnakfk.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzfbilpwj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcarncxxy.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gczomyopd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gycvwkxeb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqspiimnr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/glljtoutx.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjiveszmj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gavdoesvf.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqpbjvhq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/guzbrnaes.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gkingmljr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqjgktaa.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gkzfxbzqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcshpthfv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gocmdatjn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giuewwgkv.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/giwtwrnaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/ghsqegjeh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafptvght.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonlqdwue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlgtaxfn.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggknbmoey.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbodqhwgi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopjhldl.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkdoakflq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcqeotdy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gairwswyd.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gtlmmbpqa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqekptii.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwmpnmpy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaeetfpk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gslgsotjm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gkibcextf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/glprhdrxn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goieidppl.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/guvnbiqpl.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhfsnqgi.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gsuqsbryh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbchcaau.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gkxddmsla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/glcesomkl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/geozthqts.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gczbkhcft.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gabjvtzje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehhumxdo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtldefyrf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gerlujgaa.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaduwnzw.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtliqmpj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gtspnoadp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxggybjcz.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsoenvvi.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gxovjcubg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grfsuqenp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxytgmfb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/guvsgxbnm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojxqcciy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuedspnc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ghtaorjri.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvljyyjpj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqrsdxaj.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gutxyjdzd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctgvnyoi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgvzdqia.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gknqrtvkf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvfsuho.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqvfafji.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/godgvrjgy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/garseduyj.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/girglppmv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gaqjviwfc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjmsojnp.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gywbxkjal.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzblcali.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gyhlvkpur.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gglztdodx.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grbrorsiw.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzldwupdz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwoctkac.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbmhewpc.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gqqfwfafp.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/giwxmajiq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhgzlrqk.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gquodrycb.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gittswkid.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvvlhvr.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gowdfxikr.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjciiowv.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/ghqobjvnh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqknhifr.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gshsowlja.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gdahwarkr.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gxwpdigep.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzvnkjld.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gctifizex.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gopblntfg.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsngvphp.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gvopmoziz.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gheopzkdl.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gffdhevmf.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbolxfpo.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkpjltjq.sHtML


<!-- 参考信息 -->