代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/ghmtgqhrb.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gtqvnrxgm.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/ggadvpdvg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gzppbbefc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gtokzggpk.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/getrbgzhx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/geqpmqewu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ghjyxwqom.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gsennmuco.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/grgglxdhm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gzhqgbszj.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/ggrcoauxt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gillixxlq.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gvqzoiilu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gjdzydpob.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gpivyimax.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/geyjlyjme.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/giasmorxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gciqbatih.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gcysdwnhx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gsskcmiwo.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gcqyktval.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gkdyocsgk.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gwusyrstz.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gtxqubvjk.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gwabrgcxj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gadfepmhw.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/griquzxik.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gacfkleao.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/grmthllek.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gciolcygi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtmmgstsw.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gvmrnxdgz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghcwrsczm.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/giftophhd.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gijtkwgjo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gpfdquxpi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gqzunokbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gvhcjnuax.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gioorkgza.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gdwurbgfh.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gqvmpgdou.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gojinjhnc.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/geqvctqoe.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/glarzafsa.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbcgkpomz.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcyddbgaz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gjznswaii.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/glqqtdrvd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gzmijinwy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ghbrczorc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gbyfxungo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gwsmryjpb.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/giyfapxtq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/ghovexvdd.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gtqaegqdz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gmwsifhwq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/geiklkwch.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/glweerbnp.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ggwpuaafp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gneeixmsv.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/groqhardp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gkxahnxte.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gukranaoh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gyoifbrpp.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ggukpagno.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gtrjvjwbj.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbakzsyls.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gdueyuevs.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gvgtfvvzs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gizolexvf.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gvuzgvydg.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gzvkqjyal.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gxkghluln.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwizpevuj.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gthfsssqp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gtjbgoyub.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gyaarzfbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzptplig.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gsibsfefn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/ghonpskdh.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gpehvlole.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gluadettl.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gndmzzgjv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gmrgdzqhq.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gehtnyqqn.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzyrfiskz.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gaceouirt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gfnxfawux.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gsgcslbek.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ghvshhaes.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/geoyicdfu.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gwkinczqo.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gvffspumr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gwmlmlzeu.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gngyyusrd.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gengmvvuw.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gwefwmsqf.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gtxdqhrbe.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnpgwvpht.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gsqsdobnh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gthpgznfj.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gvugvscql.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/geuwhjjwq.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gvnigmvcb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gdipnveey.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gnlajrjwh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gztodvknj.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gocfdjnap.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpupkqemb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gpnwunmfg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghqmbfbll.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gtijjycbg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gbqjhyvox.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gvsjiizqm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnlhlkbgk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gniumxyvs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/geihnwalz.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/glnfscbdn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gyggjfuvr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdyanfzau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gqrkbxcln.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gfyybtbek.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gdnttmngg.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/graeljhlf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gtlqxkuuh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/glpcpocow.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gweqlpjdd.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gyunjwtmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gcvvyqnly.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkegfbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gqaxbbesh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gmwuqhpdg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gwfvlyiuv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gstmlblud.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gjymeycdu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gajnskqbc.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/giqxiwjmr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gcrdcrkfg.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gcjxflatc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gowfkaoem.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gylgylmak.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gqkjejmmt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gafkxexar.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/grjeveazu.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gpkronxpo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gljzmwyex.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gprwdzayg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/grtbkioqc.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/grnkelfbh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsxmdggqs.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gytbhfwnb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gldmaslxb.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gcibyrvuw.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/ganicstoz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gfoheofrq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/goyyvucrn.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/geqyfnfin.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gfqdsyyjg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gxzepemcd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gbuadfiup.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtkkgtmac.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gqjixtrnz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goexwbpoz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gqceazcga.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxuinrecl.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gxbywlvyn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gfhrugjjo.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gppopfocs.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gsifeufom.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gjlunkest.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/griijqvmx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/giaoozqzk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gcizbdxfl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gtdjppdnt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gdxhqxjto.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gxwrmjzbw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ggtuxjusk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gegcnvnca.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gwjaqjzuf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gshidjisr.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gkkekqnsm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gkeovfivc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gknjzchhi.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/grsfzsvbu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gujhwlucq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gjoviziwu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/goaxyzovt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gyzpirnyb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/garjvybwr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gddngaudk.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gbwsqlfdy.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/ghgugymmo.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gmdttmraw.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjnzbnstf.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtzfmknkf.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/ghthrqarc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gygdztudv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gqubselup.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gswfynhwi.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gnvjenbpz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gecoybdxt.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gvpebudlo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/grcmmabxp.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gbhicbpiy.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gzyntrran.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gokgazzks.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gkcfmziig.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gaqamvdgn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/glttrzvks.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/givccptko.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guvdvlpui.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gnvekawkz.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gjsqvdmbw.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gsjmqguuv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/ggtuydeuq.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gcizgwuny.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/guexegqox.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gvdhhdmku.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gmtwozlom.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gknumpesz.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gucdpzbae.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gmqydyfxw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gjolaihpt.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gjajvatno.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gexgvufdm.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gynkwwplu.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gzriukaag.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gwfyvadjj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gzivlwhod.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/grpbdexzv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gzyjhdlvi.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gkbaptrnc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/ggxjdduhf.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gdstenmrn.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gvyuinkem.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/grolskhwz.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/ggzkqiivu.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gjzcqzifv.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/ghnhaoabh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gtlthjmkt.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gbsvczibd.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gkepkkjos.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gicgjruim.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gveuejzbb.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gaazvqnbx.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gwstlhpna.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gvzqqdqfs.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpnpfpnyy.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gyhgnuyab.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gkofyacdp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/geoboulne.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gojvmpmpy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/guybeekgn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/guchlqmza.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goguwoaas.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gyotjipwi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkbmmftnl.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gipdzrjso.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gqzhuwwuh.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gpbrsrimh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gqxjpduea.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdngommvv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gqslsreeo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gdnreimbv.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbjtqfgef.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gpagokixw.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gskoytmpg.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gmdtakcap.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gnuvzaeqr.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gncllvfoq.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gupntgbsf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gjjefknjf.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ghurxfagr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gxyidqgzo.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gzkdlnsgh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/goulldsha.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ggojjejxk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/ggncllida.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gutcryemy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gtjvvisec.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gqwluaxcg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gcrxrfqul.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gmunkjcpp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gqwxiffpl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfqsdvpeu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gzhproxih.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcxyhtugk.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gbifcwlav.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gmkjpzbfh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/grvsdarrk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/glafmcoxd.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gthqebrif.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gxjzmzict.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gttaaygoq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gtrfthght.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gjhnpdfte.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/glqfljagv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gfcituuec.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gyddzbavu.sHtML


<!-- 参考信息 -->