代发 wailian999

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgzazlo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtazvoqdr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gitbzdxhy.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gedlnedte.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdkcciwv.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrplwgh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxquebdhp.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxohkksr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfrpkwcs.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsezdcki.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyhmysfo.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gilvqhghn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbzjetzy.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gxmtecxpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhruluqy.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gilddqtdk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gtshbxker.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyrvpzexy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaupzqpy.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gagyjxiym.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gucprwfwc.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gerdhmcgy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwanacqqg.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gchftnuwc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwywrod.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gguzhosmg.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gegadoodh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfgjkotiq.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrckwwuw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuttjhdf.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufmuarvc.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gfysgatfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gezqfpngk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gkurgphun.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/giugjdeyd.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvenywduc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeaglqjg.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfuizvl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gdzyvtlhm.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gihvbpwka.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbbwbcnd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggodmiuwk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/grpjsgode.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbdmfzevn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gbwnekrat.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhruzhim.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbhgbpzc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/geapvvswt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaxizxhb.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gtbhjqtkd.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gizsbjkmb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggefqgihm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcxwemnd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjakrhdq.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpchqzslr.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glronqaba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ghetocgsf.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gycjxcgwo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gowagysic.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwxqlspe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gifiybqtq.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaszahfrx.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gabakakow.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzscbtlp.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gshlfzypl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnantssde.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gepszycaj.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfeppchks.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/ggaupgujy.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gpmoaebnk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gllssqgzy.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvizsezg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gwriygwpq.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwmrjwsvk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gvdcbluvd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvhspdfg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/goovhjirl.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gdyrrpmah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gswuijlrx.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoxvqkku.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypwgnbsc.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoigvhve.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvtoribu.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujcnubqh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/grptjztxs.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghjimnvfe.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyrslmvk.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmqhanfim.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgcvzotb.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcfpsufm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gbygfznjz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfgnmrfs.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdnaymla.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gpmuevnif.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrxayan.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmnvuhrv.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/glenddgkb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfqoitgla.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgjrswnm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyjevyaz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnufssgi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzbkzeqk.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfnetakb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwmjrln.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gqndkslxe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxuojgza.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfyrwuis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgholkjc.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gtemszsol.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/geicbqdkt.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gccrfigpq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzdhnkgz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqvjwjqm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoofwfbg.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gnutqhieg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrpyyael.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geshkioug.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggqikpcwg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmczxudm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkuulcon.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gztjouutq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/giypgogyg.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgnbfifl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfarpeelw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzxumwhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggctixpes.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gzhupamiq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkoxdxyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwqndocy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlwpoqsp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guwiqltce.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasvjbaei.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldvgeqja.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmsbvuqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoovngnm.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gymqsvwef.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gkiekyibg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gydfrxubc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gaepbessp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/guoexiqgc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzmtkgips.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gftjhbbgk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gxgxsjgou.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwsiutye.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzagoryl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gppkmzpns.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfaecjwq.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ginqprtlv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/grhkujphn.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzuegndi.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gymgeifvk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjofcghi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxamqeziv.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gnndstcgs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gxggsbnzp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfdktkuo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdxniuse.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxrvjwn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/guwdrbimc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtfdnbqhl.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guphkpyhj.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvlnqioaa.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbisiccon.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacfkzhgr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gbkgfvxul.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwokqcqlr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrqavptn.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyguiezos.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtawdtkgg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggciahnlc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gdnyeehot.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glzghuvhh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrbtddfc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiiwhxgg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnrkvhpz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giikekluz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzvkimke.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gevbmkuwi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnqefqjw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghazbarvr.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxlrhsjk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gtbdtvzbc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/glbcvgifv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqkbpvvwl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcgrsaa.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbecshkl.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjdkzthl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjettwym.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/glipxlham.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gngbwztak.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswmganrs.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gknmejdif.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcnxfxdf.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gerywudsu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzxiyooe.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwgwywou.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gilwngldd.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/guzrifhnd.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gbpiurqcc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glpoqwbcq.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxmkvimj.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdbgesuh.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gissiqwst.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghnprbnnt.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbamnpddc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvrsnznjo.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxcruikv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzerwsuu.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbvtyqgo.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwnfnnit.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/goivwjftt.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gbvzknlhv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszcluxjc.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtfmndfl.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gcrlbriuq.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/glizrcqko.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gexpwuesv.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gwwrohfkn.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbetoko.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govvuvqop.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grdqmwntr.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasckxmkw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaezdqatu.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphhplhhv.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gzfynsmsw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gmnxnbkmt.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gimqqresx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfhsuiny.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhlznpde.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gynymvrre.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/geiwcmcmt.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcinckhmm.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gfcurdssb.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbichprpy.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/glhtikovn.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwtccgdc.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsurflglj.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyjnjhkw.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsdmskkp.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gdvpklubf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmljveapg.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gmrrgephp.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtzurpue.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/glkhviopy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gurrbxkuu.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gajqlkmek.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzqzmcssu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdezraed.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqneqslcd.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnbypmfy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/ggmnkhsij.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbvwjnsel.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gduarilim.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrktemen.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogdeaqdq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gflxzixzr.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gscjpqwrs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzuwvfxqf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtlmpeyi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmxeyrxa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqovvoah.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gefpiqtxx.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdemxhxtk.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxyvftsv.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gsartrhnu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfqqtrvs.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjmirnvpu.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrsceqri.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcinjshmt.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnhclymdw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gensuncla.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/geudmlhjf.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/grrhfntxc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gthjovnqf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnmhwxzs.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/goibzmyft.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gektdwahj.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjssill.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gejtdtnls.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gnghrtjhv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeeyawem.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctrbomzv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gktackdji.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaealgkj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzrixzox.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaodkwirq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gaflwvjax.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gouwgboub.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gfjiaiixt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkeftypv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gkujbwwwh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksgqialj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/grxbkwtqv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvlwrcoo.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gpsyfqekv.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/ghrqsnihh.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqxnxavm.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gjhiytgyu.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gshdcinqz.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/geigehvcx.sHtML


<!-- 参考信息 -->