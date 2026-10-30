代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gcjaiazjj.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gfbveklvq.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gtgsocdpr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gsrmeywqm.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gteseiqby.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gwcvaexmq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjwuzatop.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gkuwxbbnv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/geyyyxdsh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gmiowfpnh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gaqcqoznw.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gxwviuxrt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gspktgssl.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gxveqvxck.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ggjesvapw.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gpdvrjycq.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gvomaoczg.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/glfvfykup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbcnzpvhy.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwsyxuysh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gdptstsbf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/glcrysney.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gbdjwgrww.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gaouvgpes.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhinhyn.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/ghmfhaeyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gvgpndpwv.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/ghldanphc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gteigfanx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gevriufzh.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gkxwwtniu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwgmevlrt.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gqmsyxcpl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzptbihzm.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyaryccsc.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gyvydmqle.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gplawcpzp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/glmixrdre.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxolbre.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gudmvzmpv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gebvjodis.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gfvelvrwn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gkkiaipbm.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtmcnnptw.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gudawdxoc.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/geyhcifuu.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gizviotit.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gzrnaatss.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmudpzlgb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gbqxzeiui.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gyhkwmlmf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gnhgiljzd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gstsrrzce.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/guowhcrro.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gfgfuimsc.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzcrsqabe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gucbtdvxl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/glirdfzgf.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/geuwwavgo.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gymmeatqg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/ghqszgwvh.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/grakuilso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/ggaabmwlr.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gfbqscisu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gpgyovraw.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gllsduxdb.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gyxsywxsd.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/ggryfnaad.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glfjbgdht.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ghzxixuaz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gymembenm.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gbpsttpsi.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gwmmuksbw.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gytovndnt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gknyhmzie.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gwjgokiiu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgowjbve.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gpadshcaw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gammjpvxd.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/ghlvvndbt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gqekywyzh.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/geiznxqmw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gxnjekifh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gbfnmvsqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gviqzsyqo.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gvuxlrovs.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gjpxxufnb.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gsyszzygp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gdedejuxj.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gdziqqnfp.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfiwsxjtq.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gpagjjinl.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gkbvrxdua.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gzjwhmakh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gfwrjwdgd.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gobchapwh.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjdfsaudh.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gkeomblyl.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gcgtrmskw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gernelspn.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/giuqdhale.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/giksdrcdn.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvblzzt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gairhzlmq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/glgsecvoi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gludyhild.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gsrzqtpaz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gfrhjnzty.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gwdegraza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ganyfsdjy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gmtmvdwub.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwpbzzeub.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/grdpaoacb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gqqnigbhh.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gvxdjxprn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gypchamdj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/ghuiafdkn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gqsozqqrv.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gqfugspok.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gyevwgajz.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gwzgxrvns.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/girruulki.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gwmuxalsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gijmzknic.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gojfvqlbz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/guqznkodw.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/geirhicpq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gwhftfwhl.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gkiuexijz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gloyzanjm.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gmusaweon.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gyefhdkhz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/geoifdilb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gjfhazjfl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvjupqfgv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gcdindjvi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gcfbbgrkz.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwfmitstl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gcmuzgeeb.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/ggvmtjbva.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbmhvytzz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gxwjozqug.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gkomydvle.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gbwunfrku.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gulitumnh.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gedtjtqwy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/ghqvckpwf.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gjsmgmlfs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gdwhkoctb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/goskqfogp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gxkrfjuto.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gddkteqzr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsokevkfo.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/glgredlhk.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gdkyohupf.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gjmfswjmb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gtlikjyfe.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gsgndwfqh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gzopuopyv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gutvjnrqr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gkzpsqxll.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzbwqfkgx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/guquxrhbw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggucnoqpy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gedsoggtt.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghatgkyve.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gxtigkdzt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gdhtmlrvv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gmphqwaay.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gevnklbov.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gebotnkow.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gqgwvawxi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gnxgmdchk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/guccowhno.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gdkfvcdxa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gqlntfzss.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghmuhbcsy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gdnrpyojt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gmzhtpzvy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gfyrnetuj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gbqceeyyh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/ggbfwnbal.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gncsmaofj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gllkczeed.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gzssxtbae.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gvbpguyvs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/ggsjqraqr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxfndbtpo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gjmdnrxbz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gruayugvi.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gkucplcie.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/goponpueh.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gpwdgwxyf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gwfadsyjy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcuknyaoi.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gyufrkiyw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gfpuybjti.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsayqvfhe.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxjukgqqo.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gmxvwleyv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghlesnzfb.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/ggmakclje.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/glkrikhpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gbigozwtx.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxfnzusum.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gdzadxzmd.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gydzxmake.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gfqpqoxfu.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gmljghfud.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/ggafhdusf.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/glubaxump.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/glcpkfhad.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gcpbfjqpk.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gmgzaadku.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ggswqrneo.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ghgxozeos.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gfuuilubo.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/grxarxvfa.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gbbgffsdo.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gcwawgocs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gyrbagcxd.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gwvzmjnla.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gdnojbzjb.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/grubydzjc.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnzufqgeu.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gopaamvti.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gkqfexdom.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gzytotrri.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gkfcvyrfa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gfhdnecsb.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gfeszkoxx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gjfifjeuu.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gizuokcmu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpqjunjef.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gfpgnledl.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/glsqxtzrg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gqpodvmxq.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gucrimipq.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/givrndqdv.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gwnzsfdqy.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gsvnwaobj.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gkxiqvsup.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gxmeamtdy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gmbeyfymr.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkelcrvms.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gkojwkqor.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gsebgykcn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/ggmvqmyap.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/getuhxhiu.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/guwvvrpet.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwapghitt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/ghdizdlju.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gubyqzgvc.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gfmauqiqv.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gofmjdant.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gfnqwcovm.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gvstsgcig.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gddelynlm.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/glbvglica.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gkutcbtyw.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gpuehiafy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gnvyhkzqs.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gaobdfekt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gbtolvmqx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gklchlbkr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkdfvbaaz.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glwvzneos.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gbhxpogif.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/genlkaibt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggidzleyw.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gyzfmzqmk.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/glxshvafk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gojblitae.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gjfzytjdh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gzdsttuwv.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/ghmefomjy.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmdzhpnqo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/genbunlod.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gidsqrvbi.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/glqyowomr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gewwsbwrl.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/glkocpzza.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gghelutlk.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gkabvntog.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gfvczfnch.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gidodywbu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/glxnnykbl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gghhkrabb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/ghwhmouik.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gekfctnkr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gyeykevog.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gxefhiufy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gaxcpxfjh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/ghzhbrijg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gfhluaasx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gyqufqnuz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gitqgspdw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gamjupznq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gthhkjrdu.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/ggtauuxtc.sHtML


<!-- 参考信息 -->