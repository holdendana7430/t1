代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnswlfiq.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gapbanbyc.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gndgflfcz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/guuboevcn.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gyxlygebl.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gqfribxjj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghphhtiox.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxifadfpb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmglhxtsz.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gwgfrgudh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumkrzjju.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdvyekjz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeyfhyej.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/ggioyxxmk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaclwoxzc.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltmftwbu.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gkavdfrvu.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gbydjrhpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdychjsi.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumjnokpv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/giavxexsu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqtzyyms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ggsxxjvmd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopfrurgq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaadzmzq.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/guigxynpo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfgqrfwjc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrzcxmoa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfcwgjdn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gvchvphdm.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gslbdtvbu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpommiwlq.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gdwjmxmia.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gclxjacnk.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnycosvcg.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbszzjqvy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptnpwhyd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gzygygsow.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwulttxq.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyocbgha.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gmulvcrjv.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gkufrxojr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhoirrgn.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gmrjjewqt.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdykpevg.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/glqigygwt.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gompejdgp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gbemmbkgt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdluxufbu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/glnyifnas.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/glxlbhepj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdxmcioe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkxvitgt.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/glwbleegl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/giezkgtpw.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfheioz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozcdtvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxetbcja.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoipnbbs.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwywcnjjx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhztibvk.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkxvtcma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaaqntid.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszcmqxpl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwrplvhj.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwluyyfvq.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gntvnmqcz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/greiwosmr.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggolgnsxi.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcescwch.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsravxsmo.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/glmayxbbs.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbocwhq.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gtoscsulw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyeongwe.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpsovege.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmezvhyzc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfrbtvxx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gulxgtoad.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gktbqddqm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnkqycck.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgmdhyhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbmstntq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyolpdphd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbplpda.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjgnusst.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggleqlwyt.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssfxqdyh.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizbnjovp.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/govlvgvwo.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfzuilku.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsviwqmx.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/giqpjmpgx.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghzinwlpw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoyqzsbe.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfgiqzyl.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjhxnsju.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/golfxaxol.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gnzcymawl.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhhwlulr.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtevcjvb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/geglyrwzv.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gprhdpfqo.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gjywoledr.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgujytjj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncqoxjc.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gkskkpggw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gelrojjhu.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxnaxizv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnrebmuk.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gidarmvkq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gshlonoou.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gmspljgel.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjqdesyd.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gttiqsjdq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/givyjodiv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grntpbegv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbybdule.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfzulekbl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gusmxhyac.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhqlducw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxrtoktvy.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggziwuncg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrsqwti.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowjxjgo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvkejifm.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjywwjm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggumlpikp.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gelxwqtxk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzpkmohi.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/glhkrkaeb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvygvzhlc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxnrzxmu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxckmpbo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfqejlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzbnmgle.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchaetyxj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtpmpoie.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgsomcs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmnamad.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gvphgvdfd.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqhgcmypb.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gjxlwmqlw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnfzlooy.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glptwmfrd.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gicjthtfk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdhpcxen.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gxykdgtst.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsrfvfdre.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpswxwnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/govbadrma.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvazpfvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpikdfqbj.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifditpf.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntcqacpn.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/grivllrot.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmgskvbl.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ggufdqiqu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gmjtotyrn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqhtnoxd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgugnzlh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoeqiqqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gehcckxtj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvbqered.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guofrtoye.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaajhdduz.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmuiihqy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/ggfrjwwfj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/glqzufkde.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gusqzxwqz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gffsnxcsc.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gqhpyxpix.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gokkfqjql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gcksucavx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdajdxbi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjetudxa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwotlkokw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/glclgzvbj.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gmyywlvxq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwvdytnns.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkednbsh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gyovgcrjt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvrxegxl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/giwsavwro.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gyhpdwwsa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gbldmxvmf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gytutaqag.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqydicws.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/giwkwddkk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvzbwqzra.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmhzzvjpo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmdestgi.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gzwervjhd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntdkjgxn.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbvlxob.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggpthdhaa.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/glpzsaqfy.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/giikxvjcv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gaolvkzsq.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnvrpnsd.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/grluhunxz.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfldhidg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godtcibks.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbinqiglm.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrzengwc.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxzmaifkh.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gozfchghj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghglzmayi.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoziietc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysjbahts.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/glgfszmro.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gasmrfcgr.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/geuyxtvnv.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/guueieqnf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoegulnl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxrdaco.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnbqkyddf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gseqtosew.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gpoqswkgo.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwfhyygo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gpivqdrcw.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrrvwctb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glskamftv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxfcagfhv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokjcipgg.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gijrhvxge.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjhmxqkc.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzynsuczm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmsajsge.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gbxywtlgt.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gwypyztil.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyziagtdd.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqgkwfb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqcxpjag.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gatijchyq.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbibykql.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsntfbpo.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmwshexks.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvabfcss.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gcvmeiybl.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gzwdmkgci.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsqsylpk.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrywfttl.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvhiriql.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbhmtfjd.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgkvzvvx.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/grtzvaqyk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsexkdetf.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpznshpdt.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gambbyjkv.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhcprsuy.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giihomwwk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyufkkcrw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvqjtpgo.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvubvdtmn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjppnsrf.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/grdldmlas.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gomuyyjvl.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaerkducc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrlcizna.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtaxbnhr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhncdvjz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grjdoosei.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoqhxuvn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdkfuuak.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glgmreuyv.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmatffadu.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvixqaibe.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbymrcisr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsnoucwe.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsgswpjxb.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsjwfes.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpxnvfoa.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gygecxxpe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gelhecqle.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/ginnazwbr.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/goznkytrq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxyvngvn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/giceoltdh.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwccbdqaa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpjhebys.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gszgiknxb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gywlcdszv.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmzlbjb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfatdlhy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaskmynuh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrabnitv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjlaaegsq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/grduztbsh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gomdbolzl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gymxfixkj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtuntdary.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gssevqfqc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gjidkzseo.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgofwvtm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gxftvkgka.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxnyaanc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gpvyjixkj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/grkkqovxc.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmlgawfg.sHtML


<!-- 参考信息 -->