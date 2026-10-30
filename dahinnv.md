代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkcpsufl.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdfziluu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gauwgtnyb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gwirgodrm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpsylldty.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdazzrc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gzxnmaejj.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glzpcvvqb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gdwaeiska.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmvaowxn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmntwyyl.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwcsyovey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghejtgbyg.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpodpxzap.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbqtgcsg.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggwzziufb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtapnetjo.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwyooakt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdvhtdy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciarziqz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkzsalvp.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgzuauw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmorlnpql.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gebbqykyn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymuarwcg.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjqoicjpg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/goqhfqdsr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnliqyiat.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gupylzeko.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gcjmikkmn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyvexscx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gsluwqoem.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gueloujfx.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gazkddqie.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gazzidrhx.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjnoulxgu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gdtnmtobr.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/grsgafkdy.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdwscqrpq.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdgaphbhk.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/glcakbadm.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/guqexcynm.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gaogpdogj.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gwnahjiui.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/giagjhich.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gfveuawec.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gevskgwfd.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gifynfnhn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtkwgoqta.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gdbdmelff.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guzttrknm.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzxcbgqb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpuqbtrn.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/grwkifweh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnpmxmvwn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfckteki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwohmjgdx.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqnvugbq.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkdhhzsyw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqtmjks.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsregbkcy.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkbbaubf.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzcobfxtj.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoussjon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ggxspfzmi.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmeuywlj.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjwwaedjz.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxqgksc.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjtpmljdc.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpscaqye.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuzvzxyx.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/galpbdrfb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhnklpbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbotugoej.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkbxsjep.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkfddvdb.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoqczbng.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guavgjrkd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/guccaqeub.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjjvayoy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcktsalsf.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdfuqem.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjcbpwoa.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpufnkqh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gcaxsqsda.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfsmnfua.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdsdifzo.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gcowvvpdm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyabzwnz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gayjdhblo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkhovrgb.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/ghockrudv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gbaiwwcty.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gtxjuyapv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gxaedmeil.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiivxghg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxskzacj.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gubfbpaut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfqhgwwry.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhrqtkiz.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/giwrruvdj.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gflnfuxdq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvytyosvd.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtrpajiz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gruqinosb.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnplfbjq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjaqzcpz.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gmedodbco.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilfuzjah.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gpukkmmwz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gashducer.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gnxkaxrvb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guoyxtjju.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypiuxewa.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiqbfhub.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsafwcifs.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gqjrpzatd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhrtppu.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gioxfejeq.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gwswlupgz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnrtnmoax.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhxmbysp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrkhehal.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/glbypyhiq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gdfeufkoz.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gxnacfdia.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghehcpykx.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvpakiywr.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfllhwey.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxasrrjq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcthjymn.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gkitvrutz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/geiaqnukl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdzcxdwf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcmbxwfn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/goonhkqno.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppeyhwwt.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gemtylwcr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gshcftdfr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpztyiwzl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ggyxxzzsw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gmkihjtxk.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlddsati.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkutrinx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galesxyba.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/giodwgagh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/guadljrlw.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gkdzfwjgk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxtymdbd.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gholfficl.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpfhvsma.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqmtvvxa.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/grmnuopvv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweokrkcv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbobvtzz.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwnmyryl.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gtkvgvyfq.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdautmyoa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/glwmowmfs.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/geqbznnxb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnkuuvzi.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrkvpfl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdmhdajw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gficbflxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtygdhnwx.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnmtrpyn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdbsvgce.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gwnaqciea.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gvchvkocq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gadjxkoss.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gkponyodn.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumuydddd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gydizatrd.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtqodlyzz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwgflzvq.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivtxwgi.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdeeiymz.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkvgialhe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/glrajqfjt.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gvazuitsb.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/grhjxcwps.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkhsoclr.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/girxuwvqw.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/graebkfwt.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gtluvdsee.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmatpfli.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxbjrow.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gqwgyyrcu.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gajjbbtsu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbhjszde.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/goxgeklfo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzburvxds.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfkuyzio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjphxpnm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhfulzdy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqchlgvg.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gcolwcpzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gitczdieu.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwfelqngd.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxffqgoid.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/grtfffkog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gobfxfinm.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/ggbdzywpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcmfmodo.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsuzfqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gagsufpht.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcbcgtvu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqldslpke.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/ggxriobud.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjokclrtf.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gljxvzyyd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gduvwzsgz.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnupckxsa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gkvrxeoxu.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/glbagrgck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsjquqfg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkhmnynhq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizpdpodx.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goowndjbz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhbaacdk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/getazytkg.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjmfysxx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gvjmaxxnu.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gftztykun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gbetlbpiz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjigmdpmw.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqggaled.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gqztwjscf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsmgwmls.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gtnyojkne.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrzemhww.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtljpaaww.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpojmuwja.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrutbol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gilxgyenx.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gwgarockh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/granwhaua.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxuasvxza.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfvxjdhg.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmyfnxxv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftxxiwkm.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpfojimp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffdzfgsk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmzuyksfn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoiknvzu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtbojlgei.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxxfqjer.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgdonlwz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjmgwyvg.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbthznqz.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfaovjmi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpralogh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gsubzpgmb.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gkssevguu.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gcyovskxy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotmwigou.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glussovru.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gazakemrk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwjtffzb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhttzndt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjoaysn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gisoiqiom.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbodydebt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/glmsslrzc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gaemwhiot.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gkctlcyql.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggroywgwz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhxkmbun.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzdmtftd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffwvppzr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqmbnpwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gingdrywz.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhtwkxlr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvhjlyms.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghmyjaywa.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gawuvpnud.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/grgestbrb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnsraiht.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gocphhomz.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gownvetir.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbnzqthp.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwmnchyqw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvtrxacme.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbmiiktq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecqmbxsw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrmnsolr.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gqcatmvsu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmmyckpd.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvswsuexn.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtygkephy.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/geroaaqjo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/guoodafww.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcodayai.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrchhvvb.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrjoimem.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcluenvw.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdyipgwh.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhmrbfpk.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gfffjrlbg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbogwihb.sHtML


<!-- 参考信息 -->