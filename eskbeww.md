代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzjgwjfk.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbubmegu.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giekbksxc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gdpkjvmdm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgctjose.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmucovglc.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gniatkyps.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guobifwdy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqokcxdn.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gritfshqj.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaznynegi.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gpcsainhq.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gpgynaxaz.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqkoyewxr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjghycf.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gidlfdwan.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gapmxjeri.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnrdkzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilybvjwl.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaixfqfg.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrqbdzdl.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpvpndtaq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvaohtts.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqatrbrk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gysqmeqhw.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqtvtppha.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/geoshsbmf.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqygmxxsl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnlulhop.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gmlzhyrbe.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gcgjksvrv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvbdjqti.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrwnampy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpltyoumo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqftzcmc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdsuikak.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnolbsrwg.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gkshobjfg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnexyeqd.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjswqjns.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gvqbtgwbu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girbeuzom.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhjuswcx.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gplbbvvma.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfigrqw.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginawuymm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gavawrtqz.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxtvtuvt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gjnodzjzd.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsloriqjm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/galfqgmyf.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqxtyyjb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gnbmjmbas.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnhtoqtt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gonigwclj.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkoyqku.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grsrblgzx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gdumtmsot.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyphhdny.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvajixfbw.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnsgkuad.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfeetfojh.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlpljpw.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gyszbcove.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthbgrkqg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gnhuunpza.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjzlhhoh.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqtymvlb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqxtevcw.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggfomswxi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmtdxehq.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gevlgfewe.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giisvjqsq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawixnawm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtfhsazj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeaptepq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoqvpxpk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdobeypu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwomwyx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gmwguwszo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ggximmcjh.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmizeyspk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbcoyevf.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gteebpelu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmafbjhld.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gaoaukmaz.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvurtzdp.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gitvfdlqj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gljaaqpyh.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gvuecavby.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyaqbmbc.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtnzccyzi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngariruy.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcthtvfa.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gymikdpok.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gfpqachxm.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gcodzdzvb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmyhvinpy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxblkxdni.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzugkaey.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakntwnff.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgegrrvo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gcoehkoug.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjeilyy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ggaetjhno.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuurggob.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gxmvaabpx.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzwyecfbx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnwmpsbl.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/grqnnwoef.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gckucblfx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxgppclh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gocymfmfc.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbfawdcub.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvjblrea.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gxjlkllfq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggamynpgj.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghafsotfb.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/goonymlja.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/goyvrxjnj.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gdilabtda.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gabwzridq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gquzgadps.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gaegkyxfw.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gyjptbtrh.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxxjqvf.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnehwouv.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gipogarrx.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpplifn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsralubkt.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glglheyaz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gohynxdrx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdmofwok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gepblasrl.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gzqcveykq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkvqlrrze.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmptxmsip.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqblldadg.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdmxbzwov.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdldikxgg.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gafdgbvsa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdufnxnt.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/goiruubdp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrwvamwq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvlrmmkip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gnuqfpehw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjkdvzax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmfkgagd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gilpbcgpd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/geevxhdvs.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxsmhowi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/grwkxoyku.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvxkcwva.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsruwiarw.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnynlavn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbquxumpj.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwubqqott.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gckcvxzsb.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrfjilfy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgosdvfa.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnefglqgv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gncvuqcfm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvamcuxd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxnkpijn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gbndbglkp.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwbevydn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/golpauebp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeolpqjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gaoxazfqk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqxhlpam.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghciirzqb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyvgfxkg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxefuvwz.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggummfftq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ginzjudol.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdsltxcmj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaifvzdip.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhavfyr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixdrzbtf.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyagmzac.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnkjbiavf.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/glgnmbizj.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngbvybmx.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gwleazbef.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpihqsac.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gtvjlmihv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/ghncgzlzx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdywnhaji.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/guukgmcpq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaiuzgeyl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxdrbjwh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzwfgkge.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgvggosx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvieclyx.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjfmckfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gacvnjxuv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnsgkkpu.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/glkbvtzgp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqbbzauq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbivxgdor.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfdtrrh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxrdzrmk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdhnbbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthboworb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlfgqvtf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/grcmfiwpp.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/guvprbsqh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galkvgvun.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gieheanhz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqflggzpy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grlnmwpal.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdecynope.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/glbmawnuh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpweatao.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/grnmjdhlu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvjoifob.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/grxroecge.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxiviibxj.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdxnchny.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ghbapxsfb.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gupqdkrfq.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gevbelnsr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxbbwtyu.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gukzrqgoo.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrlpdmfi.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gygzfakhz.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnpgiwhcg.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyirjtmy.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gypklylzp.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjhzanlwm.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gneflntkd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklbnfdfk.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gheozrzhg.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gacjopmzf.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllswimca.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/geayowomy.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllgujoih.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gucjebbxt.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gyaqmmkxe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnbakyrss.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwljpzpi.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcapxftql.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkldgafyt.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gzgyvjicv.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gsakqzkls.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwkcwnbj.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gidneynny.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gvofsylqb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gaxyklxyn.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfaxehum.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gribwqxch.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/glgiuavvf.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdvmywenv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxgriiafx.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwybetxnj.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjlrpgnt.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gfubiwvwb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gcinjrvgo.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnarnedi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjhcviu.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gljotblcp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/goomgsmau.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjplvotj.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gzvczjhgo.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbnkovet.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiflatvt.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsagpoysn.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwujweqrw.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gvejxrtbb.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxjnhjpon.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/garcraozb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvvgipww.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcdjtkow.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfiyxsfw.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gickahhum.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gzpljetaf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkchqnuw.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gouxzwnof.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmezfmfog.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guooaaxfi.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkpomytfq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfvobmvd.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gowviqpxk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gangcjrpl.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gklbwxvub.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdjejajp.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gohazwxrx.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gltcdmnoi.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glojdorfb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmbpwig.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbudepizp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxemixrmd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxzoizoe.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gigprqueb.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaplzrker.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkenatjvv.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gugxyjvav.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvtzzjf.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjzrxrhm.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzsfkznv.sHtML


<!-- 参考信息 -->