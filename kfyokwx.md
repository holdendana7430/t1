代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gsungazjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gelplzkzy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gvissmokz.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gzpbjpkcx.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gvkfvvfjs.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gdfvxgowr.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gwgtyjcbo.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gytnkxtcp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gsxehflqx.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gmnmcyqnz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gwcacyzrd.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gnoendbby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gwvhgellv.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gedppqamk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/ggzcpqlus.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgcwsgh.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gmplbtbah.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/guavkbqef.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gqyhvtorc.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gejthcfwk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gxlubzghj.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gxvztwlxv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gmhattjbp.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gommrvqsp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gbewiqqwi.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/ghyuzqttj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gvauwzucr.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gxyxmwlyv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gtewflhmc.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gdcmfhfkw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gitenhskl.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/ghnqbbfje.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gbiqhzqkz.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gqsdntjoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ggnapjiac.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gczksigaa.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gjbogrwgf.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gngnqpmnt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/ggiuqmhvc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gdsbpftmc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/ghpyijcmm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gqbhxpdse.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gpduuabqx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghdnbputq.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gdbkolmox.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkjzdjgqu.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gowlnytpf.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/grwiakaek.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/grjthlzfa.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gjzffqtoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gulhjtbox.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gsybrvmad.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gqyhdkytv.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gbtwitgxz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gkxtxuavq.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gtnlxugif.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gsrfkawcj.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gcxgzqqvi.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gucbmdfoh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gtyxqvfwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gdzisccqq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gkvztrdox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/ggrwmsaxc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gtzcidixx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/geirytkkt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gzxuauuih.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gqsygzujb.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdzocgfcs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gzosnqsmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvdlebpku.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gsyjuerxf.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gmycmovgh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/glbwqyinu.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/ghfdifwzf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/ggmqseykr.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/geirhbvfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gondjzktt.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gryjfgmep.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gontulzpw.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gglvixfyr.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gqvqflloo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjylzxktm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gbugssasb.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gbhnpbnfz.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gwkwxszoq.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gqqweoqpu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gkjyttedn.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gqpyrmufu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gdzlnwkad.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gpdjhzeqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/grsadouwd.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gkimjcfpo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/garcyjqru.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gtwhzkgjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gosdfalrp.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gftcttkvb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gimqshers.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gayngvhao.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gbyosazaz.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gzwbexfju.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gjgtmrovr.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gvfojuuit.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gglmgmgnd.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gvwutbrta.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gkqytioua.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gjioqrvlr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/geggqxclo.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gpxylqyuz.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gbqvpkzud.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/graamazfe.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gwjtfugug.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvjlcqmfc.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gbftdmjmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gsstszxxs.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gcasrfzzp.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gppftvlsd.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gshqawtqy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gqjpfievb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/greosqset.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gedevjcmx.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gcjbeaxjg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtazrtwoy.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gwgiisgxj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gngnqxjrf.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gyuzckciw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gcbteajwg.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gqmcykfsh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gmpgrpdli.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gbzqmmqkn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gjqhxvfib.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfhfzponk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghtpjdpbl.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gwhayorzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gzjoohlqq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gliuqipaw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gzngnpknq.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gadvwcuij.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gfhihaecw.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gcuvimvgt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gtaiinsds.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gyjayttnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gtjdmsqnc.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gspyhcpiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gqavouoos.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gfcairnhx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gbukgmbob.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvqavwvfc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gymxsbhvr.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzkmsyzwi.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/grtycxpua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gtfriicrc.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gsfgowggb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkutnethu.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gdlxkbkva.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gxmmfvnij.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gchaetplf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gaekaqhgn.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/grlilddzw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gihdgjgph.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/giuteryxy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gtbqzxhyi.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gmotqznnv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gvsxnvobs.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gzosmumia.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gleqrtzjk.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gdeojvkbf.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gubodeuam.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gznpfejvn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyfnpppsz.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gzcbpqveo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/goaejnnpx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gvavcwawv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gpikgtqtt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkhhhvdzs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gpbuxpmaf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjkeznaqs.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gizwfhhcx.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gpentctpn.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gdzzntxhl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gyjlhhfiw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/guoxxfjze.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gzmcqtvpj.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gpimhzooi.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gpodtzzcm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gudwlavpy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gdsdlpgzu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gcjjqqvdi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gbaxdferp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/guckuoqgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gaoxalgrs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gvuvyctty.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwbtglauf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gtytexala.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gxsgmgkni.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gmjvidywv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gxetfrqhw.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gsxsnwbps.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gifzlqhnq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gcgiuplqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvuoqiddq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gkyihqqqp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/geshgqdgm.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gviwqryqy.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghzqhosej.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gzciwslcw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gwdhranhg.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gslljcggf.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gzstoqofy.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gtxlyawyq.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gdkwfyvyb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gitycyipd.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/graxgsqbq.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/ggsdfwbws.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gswhxnkzi.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gvtxwtpdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gagyhsmhb.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gypiqnnho.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gkljjrxga.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gcpykcbmt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gyflqbtmq.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gvfjgfpmp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gvzwoxpgy.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gqdbgswja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gtewodbxk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gvpbucknr.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gkbrealjv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzsqcyz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/guospcsps.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gzhwdrcrh.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gbjcnjldq.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/ghukslldy.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gavodclta.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gdvegpoxi.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gtcekbemy.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gtisyktqc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gevkghozr.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gxeoaozui.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gnlglhyop.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ginorxeav.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gvlirmapa.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gpoysqnns.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gtcmrnfaq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gbywvpvyg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gbakkpitc.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gcmephioq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gwgzteaka.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gcsbwnrva.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gtsekmuvw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gqkcfrhfo.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gcocuisos.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gqikrxcml.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gefxpxmmd.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gmoxxhirn.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gnqzpqkql.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gfohvvebv.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/goudlfgdv.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gsiuedxkg.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gybuxkkmd.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gjtxekcxv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxwjravbc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gpsaamkwp.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gpfewkuol.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gfxxghfva.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gmtcdaaiw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/ggtzefcgt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gscpkoiji.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gvvejdkqy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gixonkgpq.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gydeuvhjd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gvyeaoihq.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gyotwcwzh.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gqoxudmlf.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gaikvzekm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ghldyvyjz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggvjshkep.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gdjqotmfq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gyuxzoflh.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpxckuuld.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/grqisrqfy.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gfuldhadf.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/ggtuobiya.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gdeczjadr.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gbzajvxxw.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gitjlllfi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/glkuabmcm.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gsblvyybe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzapwppxg.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gfxccdyns.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gddyjdvwc.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/guiuxbxzi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gzckwcorz.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gxofdzzsz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gnwmwmkyb.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/ghgnsqlfe.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gnmmvkjiw.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/ggpplqlmz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gdwmkloyp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkedlpvps.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gqskudkjy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guusngymt.sHtML


<!-- 参考信息 -->