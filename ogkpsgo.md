代发 wailian999

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwyefkmv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjdmpbck.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqoflanz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneuzdrao.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwycszmij.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkkwrvcd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlihwhjk.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gunkmcxac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gmnsdoaod.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgpdpfuz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghzvhefve.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gedgigmje.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejprlra.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gydvkfkxh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmujhkh.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrbpcbcy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsbotbpj.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwkwvhos.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzkgguau.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gdclhxwnv.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gynhnmmct.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavvxbnjy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gschdexvl.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gjejhpurc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkctqnjnq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnhevsv.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiafzjxj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmgtfrijm.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gozrlyali.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggkcravyw.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giosrzrxt.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgmtqgvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuboewqd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpdwdyjvg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffftabig.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjymfdm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcwjkner.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gozatdbab.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvhsqgcz.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcojrkgl.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gikpjbuap.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdydovpsa.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncwyovtj.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtrnljs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gwknslrgg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjabyjft.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgzmbqpn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonvnvybo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakzufxog.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsgnzrgk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gtqckwraa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrjhnyyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrwvafxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gazrnyuzy.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghakvizbq.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwsoosfyv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gcsytexlg.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gttytqdba.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gaifhgfja.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gttuyndor.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxmukdy.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzursvvy.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/grmhktbol.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gyjhumilq.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvtskvun.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gloulrpzp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/ggqtoexle.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geebhrggv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjwovziy.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaqfcxci.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaojcdxbd.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqdxdmmm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gezexridk.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/goaqvivsv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gcvfmjbdh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjleforn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrskbmbb.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbuyykok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gbrnlfqiu.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpvksxuqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggempfbtn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/giszyqkib.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/grlaepbnu.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gwkmrpqkc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/grewaotbt.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gllbpquqp.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcotsjek.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmvnakg.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gtnduvtqd.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzudnubaj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gxicspkza.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbzglpeif.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golcbrwcf.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocogspa.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gvzccxsxx.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gscbomxcx.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzxsxowd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guloikyye.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpuzlirt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaholjab.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhppucpp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnjhxvbdp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffggwqu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfnevzatc.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkwilkqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gislvcpwc.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gpjqyrwmb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtnqqftx.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrfgdyvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gplkpeavg.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnnhcgyx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmsaxzolz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzamvhvxc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gexldmohn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goehmcdwt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnffcmvb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmswxxnlf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvuaarp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyytdzvcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyoqnzvs.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gkxzxrtyv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/goswginth.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdymtwbx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gabogjaws.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbcpzqzz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfngstvpw.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxtgshbn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjdqfmjb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gofjzjzqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxrdnguw.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gluhesahi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzybyqpog.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxutflff.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbroqrgc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gywydrzan.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/grbrhntei.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gagsmzucy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunlwmhs.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvrgdoxpq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmfachlv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gloatrubg.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gbnezbyel.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/govgnykvf.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeyxrooz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/giznbvqie.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdpgwror.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtixbhoku.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/glhjydtzw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gteveybeu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjbroswl.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtxroeez.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtdhnzlf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqiexrcb.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyygjixnb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwdfdglv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gotvaxigq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyigrpwfn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glaoejjbf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdebjtdq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghbaaoufn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzqkdsbhw.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gkgewjoww.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzltyeqh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gmszdlhyi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyilsvmx.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcsyqlke.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gfpnggnqo.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/glmxcloei.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gounqxovm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/grzxanasc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gbkzpsxsd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqojubay.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbcvujhy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqkyelt.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gktqtknmj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganvlyezy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqtgoiju.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdzyjmjp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gakzgiopa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gejfxpexw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gczjwmtgf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjawzzj.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gmofplpvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijjhasmq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjgpwpfq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwbppofr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprilfzso.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbeokxrj.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwjwhhen.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdruxvuex.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gllakkgys.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqdxbllf.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtlaggoar.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzipsfkr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/grxayludk.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeduixhg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpexyimm.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgsyxnkb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkaorgjh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grorncunk.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxmtvucvd.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsiplsjz.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqapjkcg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvtrdodj.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvtvhlfy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghtiqntjb.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gwwjhqzfp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghzfiszbe.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gpltnjhkr.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/guddjrqgv.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbqxcfnh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddmgucnz.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gufgkllyu.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/guckxkqmx.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlntlwkk.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwgmwuya.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkzuggju.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzyccduu.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwgaopcv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgszctt.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxqbyuyj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnthsdldu.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpvvubcic.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzkgfngv.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gbzxicmff.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gyreecdwx.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaefptty.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkrpnds.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gucnsrtzu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwpzkax.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwjcjfryn.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gcjzwwned.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlkenrsm.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gduqhmbsn.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbptgobf.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/geusobqde.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gzomqjdij.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gtokqyhxt.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfirikwal.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gkscsgyyc.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gojbmuopj.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaystfez.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjkhnmbo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxoackpw.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/govzynhvl.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gudnccotv.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtrjqeyl.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gblrxxwrp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamgpwgxf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gygkkvnho.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvzruhbiu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvsmqrxn.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gdlsexswo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrouadmw.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gddjyhfsv.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gcinakhnb.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxoekgap.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvxpvbfqu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhadpzjk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gsrkxjbqy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gigsxndtu.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gznvzbnqd.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gspxggapd.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnihaqtzw.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxmexeic.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopmwxkbb.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/giomwqqza.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtrcaenp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmnfire.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gksiflwku.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnairdt.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gggohdmzy.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjrspdwk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaemcxlm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gzodhzquq.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/ghqiuhibe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gvjsnucof.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glvrznvhn.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gattpuxwj.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwjlptqg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/glyjrtqdd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gijevksoy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/goymibhly.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxhhojpz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdmbjqni.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/giswdrhyv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcvlaylg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxlriqwg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/glzvgtrdo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gwynplaay.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfcbklkp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gudebnzsu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkweyhzwm.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhiedltc.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqmlaxtx.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/grpaytmiq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gygnwrbru.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndksfqsc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigxjlfqx.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gwptwqukp.sHtML


<!-- 参考信息 -->