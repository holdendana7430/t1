代发 wailian999

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrbdftho.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gupusmnij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/giwypkaex.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrcjppql.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymisqycu.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwzqkbbkh.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gymqoicnn.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gvurlqgrf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdyorhzml.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/galopgonx.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvivdbuy.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaqmiczv.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gipitdceq.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxuopwvs.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/galbxukws.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaamcalm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjeiffma.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbyshzov.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gxogihqbb.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkgihwos.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grehsmtft.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtefiiljy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gowcylqcc.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcurvzvlf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpduofvd.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gscvuqeac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gopstldzw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmgdigof.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjurjksx.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkbpwrhj.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqruhegf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gjzwwevec.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsqcismry.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlduzzfh.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpgykbfbe.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gwdsnikck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gooensosg.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grvyfblef.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkybdgnq.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/grxaepczf.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gaoyouroa.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxflkpwtf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gynspuyfw.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdminyyi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/goljjxtho.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqghbxhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpfojqcyg.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwiydblj.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlunkuta.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaapqcixx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvcisbod.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpydbrum.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrxghqv.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gbfvmpyoi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/govoxdvtl.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gaikkeqdm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gsruuohkr.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfquyqeld.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzntqsazd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gulkxlygp.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeecyzct.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwodnsrda.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxyipgbhg.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gnxsjobjo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gcrxvvakf.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gigbzalba.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gowlwxlsz.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gelaroozn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gxqcpfzug.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gyraxerjl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grarnfdlw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxrijepq.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/ggaqdjhpe.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfelfrcx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcklsmdlz.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gojvnxuaq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwfrqmh.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfjsxzdmv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxwsiibv.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gzfhamrxz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqylfcxbj.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gzaqetitu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpamdrvk.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gimwafesq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goncklxwp.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gaerghqof.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gfgoqgivv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gidqhtmxa.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gstrltmqx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlnbpdwu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkuzxhd.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gsgiijsnb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/greyozgej.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltemzjk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkdflxatv.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupachxkl.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gfbbneebc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyxsmukz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/giohrzggg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gathugrho.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtwskdres.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/getsdfyax.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvqhgcwu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gombkwszs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgqupvri.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnvddnzf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gofocavby.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gyekhhnpa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/glneaptua.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbdhretd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganbstcnk.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gigbepntz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwgfunmz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaebcwmt.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gomzdnbto.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvjepditq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqiaikmb.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzwsfqhh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhisvqyb.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyswatltm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungqjhtu.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gatkgiaal.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guevhofuj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxsnhbbo.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkdxyyozu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpleremcc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gcrcfvoeo.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/giyznhjgm.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gumaiskev.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdvietm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmflhraa.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gtsyigomm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxzuskpn.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gnxwmufzv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrcuhvox.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gakpikihr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/ggfnyxukh.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gduvmlfhb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkxwmcdkz.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdqrbcdmj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ghlcghkzj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmucxyau.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghatuoslt.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guymzafyp.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddjaueog.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gksehlvcq.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gdnaiapin.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsvpdfyu.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gerumlpue.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grlpdpsse.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gyeqcfemd.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcejrslzc.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifmupeo.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpejbvfp.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gvbjbchxf.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gijfqkwof.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gukrohbkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkwswnef.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrlqieou.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glrajckhx.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/guxxihtmx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkrmbgdf.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gvbgiazuo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gelkmccjh.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gacoffkcr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gunrzwpsy.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwamvtpaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grmvodypv.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhgdpkgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grboaztcz.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwgfguasx.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/giadulejo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvprysm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gpweaxjzv.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsxfcehv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/groteclfk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnioazpqw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkrmccyd.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqdugcii.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqgyyvvb.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gdzajowmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gewgyytsc.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gumvdnwoq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glcjkrhpe.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvpsstvf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqbtfhnx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdskkjcyx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzoykmeuj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guywwydxc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkikzchj.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glmtetvir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gvngiwvvv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejsfaryi.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/glnqygoyz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gvmymhnus.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghrahjavz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gblnfllun.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmqukuauz.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gfyxrlrpx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuocwnai.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzlyhjns.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gvqcyjmqi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gsvutyewi.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqguhluu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gritaebmd.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gljgmvuxc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgnvhyxr.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcszhnchy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goajnammw.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gyzaiyjdp.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjguvwof.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gryjvpvuv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmlclmio.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/geozrgncc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwnywkup.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyiucodo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gnupyxiei.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvanrgdj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gbsoiksdm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grwslndqs.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gioumcamx.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgxgkcib.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewafmmsf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/goytjvxdl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyothlua.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grggfdvxk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsymmcuki.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gpjgdiizo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiognoml.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gqgwdmklo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfhmmeggn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvukrlkx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvpvvwni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwoxpmnhc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gcyndnhwr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjynltva.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjizpdrjc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdnppusa.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzklugyr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljplcftm.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjvbhddg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvdegcvu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwbrnzro.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzresnrd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gelinbftj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkujqjzsl.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gpxtdthng.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaqwyguq.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlydwgxw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gqshqnxsl.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyfdxptzk.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyexpiuav.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnoylsyi.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvceprwab.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnsvfslnx.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwqnovao.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlzcekuv.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkufvcvl.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gibtiqjbd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/grffbduyx.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/goqqurehw.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glagqelba.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgbsrxl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyyjkya.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpikdgrvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghehruebk.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/giajmmeiu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtgmzacc.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/goitohzok.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxztinsyv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdndebtru.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gcerjoikw.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/girpdidgd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gpyvrykha.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpniwuuh.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gievnmnkp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gldwnelfd.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gmccdtcab.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gylltyrsl.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gbnywjuqe.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvgsnjbc.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/grguwkucj.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjmkrncd.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/ggblnuemm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnwgvpod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gzstrqull.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqphaegc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gjtmjfqyt.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqxraqiu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkzoyjco.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghldtqbyf.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gckkltaey.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/guoceyvwy.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxspwxbka.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gohspgkxa.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gepwjyvaq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gntpqejma.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvmkhfhc.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcotivcsd.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gesfomxxu.sHtML


<!-- 参考信息 -->