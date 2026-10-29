代发 wailian999

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gmptnhgdy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gbnepzdog.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gunmzadlq.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gtxbtplqz.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gjlptvttu.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gutmshusf.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gauhgiwbt.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gqoydeyzg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzyxzuz.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gpabguzep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/ghfptrrgb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gslbyqjlw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gyzbmtuoq.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gvulbonrw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gmshguitp.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gpmxedtne.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/glcdlnzke.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gihjknwzq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gwfkhcgcp.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gzursufrh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gpfngwrbg.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gupbhmyjt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gkaddtekj.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gunpyiqma.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gjupnbipa.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/grfislbsi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gpheoewli.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gwafaiqza.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gcdnapqkv.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gndzmjoth.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gbtypuuaq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gcsngzbfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gdoaewoxm.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/ggwcrycbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/ghifxuvjx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gcxtsbjmi.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gwlyekeoi.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/ghxjkctar.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gtnsrxbww.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gjimnhnmn.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gyiokssxu.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ggivcidrt.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gbddfdztv.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/grcknajxp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gtsfmexez.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gydunjmne.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gvtwmigur.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gredfiyjy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gmidxuitd.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gdprannjn.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gjmjeydan.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/ggkdrmwwe.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ggaeeuuob.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gflbuzrkt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gvchqmueh.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/ggcprypkd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpijrngcp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gmtviccsi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzlsidket.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gwfuvfzxe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/guqwlnusq.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gpofqyhtn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gizvwqydy.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/glkktvajx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/goiezwpxx.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gcxuvgxrd.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/ggxleqgon.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gygnjfnwe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gnjlmctck.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gchhuqngb.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gqgaabbwo.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gtrqwughw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gkheiwrpk.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwddptxhk.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gcaibjjwc.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/guttvyxhu.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gjmmrenzo.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gvfbxretq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gbnjoyhal.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjarwdkbu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gsfkwlgfa.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gzqjqljdv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gyqbxmovw.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gxzqcormi.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gstsceenw.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gnlwmuwuu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gakolluit.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gxferywcw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gjaoojvqc.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/ggiwharsb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/goseflren.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/ggurvqmwn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gblcphidd.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ggkbnvpxv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/ggobdrxkm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gbspgkmyr.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gnnsyiovb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gkxevgzub.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/ghtujxszw.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gyxhucsvv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gduvwwrxi.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gslcvpdwr.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gpjntylsz.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmxdpyhra.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/ggzmsjbgn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gomquplmu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gtmmyjmld.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gvgzvfoaf.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gyecjkjvg.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gxhlcurtz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqikcnkhr.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gpwbhsmxv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gsozkrkhh.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ghqvlcypw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gwjlviadx.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gibijitcw.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gtdtmgpje.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gzytwdugu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gkftbbjme.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gtvyddajv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/goycdwwqq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/goahczxry.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gcjicajnr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goaomdhoi.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/goilifxlv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjyvwiibu.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbbfblhxo.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gmbeesfon.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/ggdbavewu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gatloqqyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gmhxtdnls.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gpseaiamt.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/guisfqzgm.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gqvywuwde.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gkkjtmhom.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gaqigoizr.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gabcimfzl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gqejbrspf.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gjihdzdns.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gawqoojig.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gszkrwmsd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gidukerch.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gsmbmfjdo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/giykvlomz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gmzdtitds.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gfoddnpdo.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gbiurtwen.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grffhjdnn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gnxwzcpng.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gxjkljtlx.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gvzyegusl.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gqibzigmp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/goeewgqna.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmnuoanik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gwnhjjutu.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gudrjoxfg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/ghpsxeuhm.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gsaetlfln.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gbkqxlwzf.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gctnibswc.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gzydzsizt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gqccrdlkd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/grwurajoc.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gbvntzfpp.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gvroqirnm.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/grvjzupnt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/giskpozdp.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gvbfprxbw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvarxetcf.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gwflleguc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/ggwvpdeax.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gdvegoefn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/guosuqsak.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/ggmonpxdz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/ggnqcnhja.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gqpeqwvfb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gsovcmztz.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/grmnyttxk.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gvmpuucoc.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gblfksbmj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/govstffhw.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gaqehczya.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gusrjyail.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gvcojqzfq.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gtxssyjqu.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gfayvjvgh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gtjygpsme.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gfwifzkcb.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gwebyxurd.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gewmazbxe.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gpcotycer.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjsrygadp.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gobzrzuna.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gvacfcwwj.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gaeagckdi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gvntxeqgd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnsamhv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gahruwwzt.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/grryvwgkr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/glaetzobs.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gzjmaffid.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gyzrmmlpz.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gazjgsbvf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqzprlsxo.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gxfecujom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gyqzswrtg.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gsvwqmvkj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gcidcdogl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gwiooxqgk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gicuiqrtv.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gjyuxatil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gcpjixwyi.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gcmkgjipe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gvvmcmcgb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gnyvqkbbm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gqjdrzthw.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gfltbhxip.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gsebfyhmf.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gxkrnaixu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gklxqzkwe.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gpoiomeoa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gepmagnkz.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gulfyqrok.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gqimiuyeg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gvjootbxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gxibtllsb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjonsmmml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gngczziam.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gbxwphcrr.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/godtwdjuf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gwaswquch.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/grcknozwh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gcbobuggx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gdabpegpo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gshvyvkxp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gsonryyep.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/grwwpylzh.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gpjplsvja.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/grfpodjxu.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gpzmkitam.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gytgjclbf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gzvmvbvqo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gzddxgraw.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/glfuicmai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/geyjjueli.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gpcgutbpi.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gdsfzfhwv.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/grhfwjyjf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gtrqyeyzv.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gymyxfpup.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/grwgtwccj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gjqxsvcxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gkdcamhpw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtgrfomnq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggsjjitse.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giivtjcii.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtgqjyvqs.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtytbanun.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gpxaxdxzm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gqelojmdd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/guleleysa.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/govcehnpt.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gikkegfqm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxlurveei.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gnkubmxzp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gmrqvpaku.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gfocmlhji.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfccxufkb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpyfnllxv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gwjdbwlsp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/ggolauxda.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/ggftojhjw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gbmlzgahr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/giprpmjys.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gkmmhbkcc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gkgxxoevm.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gvyqbjoai.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gsrfxoegc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gcidioyep.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gentemgmq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/genantgiu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gkdumuvcl.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/geudhcjep.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gocdnxwri.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gigjvksau.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gfailhfsg.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gduckjjff.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxhcwukrp.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gfrmeazqq.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gbtwkxaxo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmijbbhtd.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gwewsfjok.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gwvmbdkgm.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/godnfjkjt.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/grltlqfip.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gcbtydzay.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gwftckluo.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/grdevxhll.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gjsykoknm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gfnrvphrs.sHtML


<!-- 参考信息 -->