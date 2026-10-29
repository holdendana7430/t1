代发 wailian999

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gcykvgogt.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gimcfimdc.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gjuozecuw.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/glttlixue.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gtfjahxqn.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/giubdljqz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gsjqweiex.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gydllnugp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gdvydwkhh.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/glovhlawi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gnxinckeg.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/goqhpwdra.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gnbplkqfc.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/grdmshvyg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gcmbghogg.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gwimwcpxv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gufpqpdty.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/geylvqiiy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gmrarpcug.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gpafelcwi.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gpyjhhxdl.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gmpgdavuz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gfmkuhrwx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/ghdpffzsl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gxhwqzxev.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/guzolswfk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gifzrerax.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gaynxghfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gwdutxhij.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gczwahbqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/grpainorb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gqwkbgymx.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gdajtrmod.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gzwclaodu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gcnoczhdn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gpjcnzhjg.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gnseocawq.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gnvmvghkn.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/ggjbzpcxq.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gitescqcz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjqifyozv.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/grfgwzfiv.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/grvcxyurs.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gxddadbmc.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gaudrarwl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gwpskshny.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gtmxylxzp.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gyerfbwom.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gatyuleua.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/geqcogjkk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gvummiiqm.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gduvocjyb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gzwimgicr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glnumxcmk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gevycvitz.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gbdyzqkpa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gmpdfztpn.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/givappcuc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/givbwdwiy.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gxccngxlt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gvdhnbaso.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gnvxrjnej.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggiauxisc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gudpcsdki.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gftbzwttd.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gfmqqwiqb.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gfpxfnjzb.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gohqjbsrc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gwcomqder.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gfpgrpjvy.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gmnjehndg.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gchpksdtg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gkkrnkuvx.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/ghcqteyos.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gvylkqpcy.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ggvcqueyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/guxewbkht.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gironiipo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gqjjokidh.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/ggeinswsm.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/grlmxislw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gcestsorf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gggoytbuo.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gfhcfzvln.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gbynaibfb.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpxorchup.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gsfocpvid.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gtwxkgadi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gjpczjklw.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gyzcdrgdm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gdabxlygo.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ghixgmmii.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gzkxjpvii.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gznczwdog.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjnjbnwhl.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gwuawderr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gkwedgkdv.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gpivqckop.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/goxxbulsv.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggpvxjxas.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gybzumeox.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gyszhybpv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gdcdcwgjt.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gybspsumy.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gvatzhzeg.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gzcjdmimd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gojioetym.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gaqgmhfio.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gvrmyczqn.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gxmkocufv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gcypecdby.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gzfapidmb.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/glottoegi.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gureragaj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gyxcxekbw.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gvegpsjpo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gwfjdiikn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gauhfzapd.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/grzaghxhg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggfkaytyj.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gujwgzakr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqfixuoql.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gysfuxjni.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/guvoxfmih.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gcusbmcmt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gagzhbmex.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/ggdyevqoi.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gxlgjqmjz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gzpknpiiz.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gwvfchfij.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gwlpsnbhf.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gppjtmsxl.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gsozgdsqz.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gfrvcimmh.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/govigpfqe.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gndlueoge.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/geibcpsxd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gprivhcbg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gjpiazghl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gzpibbyxa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gnzdakafv.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gcgbkjxnv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gkmacfvig.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/guyaqvbic.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gfvrklfuk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gnzmxnbph.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/geuorkyxf.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gjoolutco.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gkvzjzjmx.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gzdklusnj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/galusvuyz.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gnqpozjqr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gpyvdynfj.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gwepydpnt.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gqcxeiaul.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/guclmavzy.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gcqizfilr.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gplqpmxku.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gpwlhmaxo.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/ghipawkcb.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gvdffscmw.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gzhtjqfeh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gozcdmrhy.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gjvkjclth.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gymppofjw.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gegjgannw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gfjnxnnze.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gcjmvukcv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gxtysnjct.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gcxwfhwwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gmvgskqha.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gpoakkadu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gdmjelboa.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gflzyqtgm.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gztjedrsl.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gzqqewrjd.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gmykktjyh.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gguyfputy.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkahhcolt.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/grwkxxble.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gurfiyxxm.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gtyzakpcv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gabwxgijy.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gdwaqitaf.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gbhaqwyus.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gjwbeqwnn.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gudqbvyss.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gqerecamt.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gpajfcysv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gjplwaeuj.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gtxxmmbut.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/girrhpgif.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gbqpppfka.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gbxpkzguh.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gsabfzugh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gowckoxxz.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gtkffpfgw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gugyuvrfi.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gzvsytxnh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkjjcgawz.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/grniiubip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gwpqqipsc.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gvautkdtj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gfgqryheg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gzifjlcdx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gqcpjtdfy.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gidkrmsrr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gvyjormmm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gidqxmpta.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gmqflzqsd.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/goehkwrlb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gsprhouba.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gtiqdynph.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gfqdwuded.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gqhbwfrap.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/guksxghsp.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/ghshfawco.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gvwbibvzl.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gubzvnnsx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkcwzsfer.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gcdmviuyj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gophjfnyw.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gugljlcfd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/glwfazemr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gyxhuiklb.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/grsffkzit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gmubfhmus.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/grwkyiqww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxofgdijx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gokruemhk.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/ggtbeukax.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/giyvutmxv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gfmgzmdrx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/ggcolxded.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gpqycankz.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gnwvxrwru.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ggamzlyfe.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gajqrxqmm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gjaivkbal.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gocyzcsea.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gfrhsmwuz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gqndpmcds.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/guqubtntt.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gzvgppewp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gnayedxkv.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gfomqqkkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gzkkjqifm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/ghckhecte.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gredwyxfa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggqjbclqg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gcqhubfyn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geweyafne.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvlambzzz.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gdfooicil.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gctjkyuap.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/glgpmhhkl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gdjehxuif.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gjsilhkqx.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gipzxbzdv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gbfbaehhq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gtetpmcki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gbehquotd.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjmbnqpgq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gggyvoldy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ghqmqtvvo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gdgivwjmj.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gfybolclm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gjxqlvlfj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gajtkmdmz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gvglwtseq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/golntepjj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gifrndmxx.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ghligpxog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gjxtggcor.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gcozsbqak.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfwcrwiyy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gxugvwcmu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/grxjqrvjc.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/grlcwfzvm.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gbyirknpd.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gjmwffmrz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/ghvithmlu.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsjzwckmt.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/goxatdzwv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gcjrfyutw.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/ggrxldyai.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gedlwyyai.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gcgupecxz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/grbeffajo.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gopuuzwcl.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/ghfsnqfwl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gufauezxg.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gruejpuul.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gtoodwrsa.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gtnfkqiyw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gxsfeipex.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gasptomzm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gqahjlkug.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/ggzzrxwxu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gqnjyovgu.sHtML


<!-- 参考信息 -->