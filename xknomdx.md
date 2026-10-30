代发 wailian999

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gokrzjjcx.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gvversbyv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/glhweizhs.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtuhirmne.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gsayynnhx.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/glyfkxnpt.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gxzjcjyei.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glcpbwgtx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/glywphenm.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gceywmahn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gyyonelwn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/glnklcnhl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gutjuqajh.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzpxaiohw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gilqujayw.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gfwkqodkg.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gcrenoymd.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gazikvkkp.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gkvhvtogk.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/ggjfvqeta.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gdxqjddtt.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gzrolycng.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gyyfhjuio.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/grojlzcye.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gjiakevuk.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gfgeudsrm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gamrafjfr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/guhehjwlu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gscqwouyx.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gewiqfsce.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gmnmnujyp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gfxrbviqu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gvamelyck.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gtvrkxnhz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gfneihetf.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gzifoofda.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gkplxhmca.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gowfxqgok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gctdywrid.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gdvibjxsn.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gskoougjo.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gfrbidagd.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gqlnvhmdi.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gdibfeklo.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gassyabur.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/glftxzqhj.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtnuwrfry.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/ghletbsba.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/grpunmori.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/glcdytyit.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/grhlomcxg.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gczhnpuqq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gddjohkks.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gtwukbkuq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gspkltrxn.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gfbgyfquf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gjcmkaecz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gtgvsxhmi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gaikplwpf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/grozbzgeo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/glrgmlldw.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gvpvnbfyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/ganquzdqk.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gjnwxzjqt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gnobunvfy.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gacsxsxud.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnjieyaec.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gwhivuoku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gmrwkrfwv.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gxinpiwac.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gqzclpdxl.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gwtkdfimg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gdzbxiqbx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gueechuqz.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gsekrddwv.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gibzvkzfn.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gxuwxiybw.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gmgbzbvmt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gplbgfztf.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gztbksgdr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/georvhmgy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gnayvxwjq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gzmvjekvw.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/grpvdfcmf.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gobumrhar.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gkvmdkrap.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gqpvtpvwt.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gwtslgivj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gcvutksxz.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/geghwdhtt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gxmtsokng.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkxyogl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gxnklfcdv.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gnjdxtezt.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gmfjkogtx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gyxshoaop.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gqwdgmvto.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gzbxvjboe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gvpstjnkt.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gadpqpkqq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gujvreepa.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gntkpejux.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gggpfopec.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/grobaufau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gvldjcxfu.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gqbgghihg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gyjxqiejb.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhprcsv.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gnevkczly.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gyljcfoyg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gpgciyroj.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gcyuvdpgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gqfaovbqx.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gfeuezdze.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gjcxwiwoz.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gcjylcjpj.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gcvmzggjg.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/glyozxugv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gcayichtx.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gyjtevltp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gfqxqqzdv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gguobpyem.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/grwhhbxkx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gocevhznj.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gncxtnvsn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnvltivvn.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpcrtrdoz.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gruknnrkr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gzyoidexr.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gljlhzkgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gktourggt.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gsqcmhngt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gmnwuudgh.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/geuksswcs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gzebfozjh.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gmdeoazzl.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gfwifhbnm.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gutnxujlp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gjpkmplrt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gvyaslzyy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gbhcoxhui.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gbtipnpjp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlsgroi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gqzmgsyfi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gqvdtfenv.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gusnfjjix.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gbkixfyzx.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gohuvpyqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gxccyysch.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gjgegkorv.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gzpqvlkir.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gswjjaesv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/glcrbdgci.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gemrfjsxc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gyzwmiyog.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gwllucnvu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gnitqoivg.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gusrxwjed.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/glxtwquuw.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gjfbemiuw.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gqzggqerr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxzdlmves.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/geoqbxjfp.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghzodizwo.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gssfdvsdo.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gzubpyzls.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjnakglzd.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/grthxuene.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/ggriaksuy.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gdceboaay.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gyalvpbja.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gwsfjhndw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gbaltkpxh.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gofydrwnv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gkzqsfwxq.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gkuzgiubu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/ganneosny.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gwwtxjjog.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gnxcqbfit.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gintxjmra.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gjprivaut.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gctssxyfv.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghvteawkg.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gtrtludam.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gihvzuyqu.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/giqkdpqto.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gtiokiceq.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/glfjjnbjb.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gmbqcntos.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ggryismop.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gmsmfmdpr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gemfuhdic.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gnepzicio.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghgwugfet.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gqbdwhvxt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/ggrirszsl.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gtwhgaipn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/goqppewio.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gfncbdnlh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcbdeuci.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gpsfdgjgb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvbvhgbky.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gitiqvvfm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbbrntfio.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gxxcbhobj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gbnvuqirb.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gaqoffgmp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gjnovrppa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/ghsdlxwqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/glecykrhw.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gmoecidns.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtfoqrpnv.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gbviytabi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/glnjvdixg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gnycfesyv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gmupycfao.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gedsrbmbi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gjmwqtemh.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gyuqigqem.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdfauin.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ggdbotvxi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gvdxiypwg.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gvhdkdqlw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gmvbpoexq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqxcpwzsv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gbcskzmme.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glsyfnqtm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gwwujuslm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gjfwszsie.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzxohvlri.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gvquayzin.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gjlzawlkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glknnqjtp.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gpdhdzgig.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gllioiwop.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gwfkujjil.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gjjdcrqkt.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/goxqlpkdg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gylwswdxl.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/grdsgmtyy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gubfglgyt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gbromaull.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gqccmvnvt.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/geeqtkzao.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gnporkqmj.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gaxtqunkc.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gjrqvuqte.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gfslocpvy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gojueyxiq.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gogtlqebz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gvepiczvf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gukfihfej.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gtsjmbqam.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grqmcvyks.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gupdbhohr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpqrhqkru.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gswvurduy.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gupkirltg.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gzaajvwlk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gqjfajygk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gdmuwxmwf.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/grooaxoku.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gconejzqq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/geqcmltoa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/grxedwqiw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gjjnkuhqq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/ggqpkcdvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/grnzxhpjh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gnkrsriqb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gmdkhbngx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gkifgldku.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gmfgewugf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gnntjgklb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gzlhtkztj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gxxsmikxx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gfdyuvaar.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gimqjunfv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gkfsdxzfr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/goclrjmsp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/golscypel.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gfkykpiqy.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ggbxslidq.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gxqesouqf.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtuusurul.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gqyvpalsz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gcczvnvkk.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/glftrjjar.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gurmlschw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gnpngmdzl.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gjrtqiyzw.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ggwcvwirh.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gvvdkgbbz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gnwqzidut.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/goqzzwvei.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gyrczubyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gforiqupc.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gtlreqnmk.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gsecqpvki.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gfntqdglb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/goqpyprel.sHtML


<!-- 参考信息 -->