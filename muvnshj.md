代发 wailian999

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfbgjjkr.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gjaxpjoak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqxpgkq.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitwodgdn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/ghowxgklm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglpeiwpb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/garfxedkr.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgylmbyj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gkvvyqusq.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gdqsszlcp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goftnsarq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gphgprrph.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvvxeamu.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gkqormjoo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmmqeqfwk.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glqvyixce.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/goymltfat.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gspthjjzz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/guyqamhoh.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gpxcjfmlq.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gieovhwak.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gxirmfdla.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpderwgki.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbjexbld.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glxmqxlet.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gqqlgjkmv.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gquqzfzgk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpkmzagx.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gcquufhhs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylvtiehu.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdyrokxmo.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gqgyeitcc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjywwxzl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/garnnsenq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssfljmr.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gacizzqec.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqeytaeu.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gyjzzqpbu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprjifkyr.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gqcjxtysl.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gipkbnypv.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfejjvikl.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpfdehyqj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfmrcmrx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gfvyuzqsl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhfwxyiq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gxvukqxfo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqrisykz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gsncsezmq.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/guwiowfhj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/glftlymyb.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfopekhez.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gvdlsqfcv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqyxmszq.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gwkyrrycp.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoyndvkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gimazbite.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzekmlsz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofzqeajy.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwdicipk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfibhhiwf.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ganpqgapu.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcekkerd.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddekrixv.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfjryesp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbspxfjpp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfvzdkbg.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvagwqgef.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulqtdguw.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxwbtgwf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzgtnxymn.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gayhpesht.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgpyoxps.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/grgjdawhf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcktgwjkx.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclqswyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghglpwshh.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtktorcxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gmkpfogxp.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gleyfaojd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnevabemt.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gujzxnuuo.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gwyyfkxzq.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/guuhvtqxc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guibpjutd.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/galywxfzh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddaxickc.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gulmokcyw.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgvuuna.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqectnzfd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gumwxncvh.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwhsreul.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/grovxfgdt.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjsajihrk.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwgtyiap.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glntitujl.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxruygea.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcygrpbed.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqowayqll.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gcboqooem.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbksogg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/glinvdzvk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gguhdsomc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvuatcrx.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gfaztqfly.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqrauyxv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpttkfpth.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbqggct.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gjndacrrv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gghdrdweg.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvikohanz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnclzuke.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzbamzvrl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrnstsjo.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsotqfdqi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grpmltuiz.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbaiwrusy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwxljokeo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gikhaidzb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbckgwcir.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/geiptagzi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ghumlqqnb.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/geivswdkd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/genadeshn.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/giekyvmtb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqwtbsyi.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkzbstzxs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjslvfug.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfevsqiw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmewdpduc.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcerakfqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshgpgfgq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtpbjwqw.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdxlciji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/grhotukxl.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviqrrpzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/galxjsnrm.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzqherjyb.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gezpstsfo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gufosiytf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaodngiph.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gwcpavrqw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnprequuw.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojquzusr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeioprct.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuxjwwng.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gaofqhghf.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkitwuetg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcdipmwhf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grkhmhpyo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grvjfwrfr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpuxfiqc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlwloprn.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gqyefwsdl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmudbacr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyakdjoca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkhczkij.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glbqahjiu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzfhkqxn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gblcyxgpl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifopbhgz.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/greruatpt.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtjrzgtep.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gzwuhellz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbcdbqlza.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ggblmeyuk.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gbhjysvts.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/guibotthx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiadxrex.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/giqocnbih.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gconajbhn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gppegkmct.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvfulknt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glenqzueq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcnfrrgm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/guzloyict.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwlbbmed.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoqikkdg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grjktinkg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gbcmxamwf.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gwedwltng.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpvlmzgv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/ghjvjdqiu.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/growamdzb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gcijkynmb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohettxy.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/garxaefly.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gdtmrkypq.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqnkqgup.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyacrbff.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gylfhlvjj.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gayogfstq.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpsvime.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gibutlfns.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ginitmtwh.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrtvonp.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gwhfvutnz.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjmsqoxs.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuytianf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrlphavb.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gryiapmvn.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqoyyytgh.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpswuxpfx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnfnttcz.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpacbde.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gwcfdnncq.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gtzmnyhas.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/givksdthw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgjbzdhl.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwamlnrh.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlryqub.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaxrajku.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfuzvrwfm.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjswlefl.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrtkjyri.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaogphqxz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gtdbcmuqr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvldnenif.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvjajvor.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/grzgbapyg.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvksuacwp.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgxzotgc.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmlhtveg.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvwrmlg.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gifvbvrax.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gqaqnrbft.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/glsgztchy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gztvctwna.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gourwohsi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gakqeglud.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjfimzlp.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/glwnutgsa.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gwovojbkw.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnkmlwxs.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gprhvyylc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvskwucnx.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gormyyzca.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/guzzprqzj.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnmfodts.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gjowyszvy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbcxrlyg.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvjvkpzv.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gibfkibsm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwvdnhyb.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gmbrywsxo.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gacdstetj.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfxseaqhx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoaetjmi.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrgjnppr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guqzaaqsi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbxabglz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjrupka.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/glvtqtqcd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpnbwmedl.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxntussu.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgvmqxqr.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxzbjaip.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfujbwhvj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gngfxquza.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzxtgxmb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkucgrldw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyicnmycp.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzyjjqnvv.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmrmqtok.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjuojoddb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpdjhoku.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyyewpkz.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsdbizuv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glynvncds.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgqdgle.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdcrpoit.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gaijprhtm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiqxaydn.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gklvbdcre.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gblqymdzm.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfcmxojb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikzoxyih.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqewmtgmm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzwnogqe.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhdjozeb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gynurjzxa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnukubawt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grjqfwhje.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goivbizwk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgqvqgon.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gzkndfkgi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkauatarz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjoeelwyb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gjttwepdb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrrijpjp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqtlutex.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gtfhyoorr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gagxxsjgr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gieglksnq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gstcakich.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gffbxhbrg.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gqqoncxwn.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/grsgvnlpq.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gzzdclhxc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gudukgcfu.sHtML


<!-- 参考信息 -->