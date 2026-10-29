代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/guptcgaxq.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/glfaieacn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gvfordiqo.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/geelplyuq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/ghuebqgsk.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gfjmhklcf.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gpcnxjere.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gzjidsozs.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gycdesokt.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gubdakzuo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbatneiig.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/grezzmwyt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gcqhdjnem.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gmsfeenpy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gfmadyyyq.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gryhhkobx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gijugpfwp.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/ggymzdiwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gotfoyqii.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gttshrugj.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/grodwqubm.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gvnrdcxmd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ggweadekm.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gtxfcywtg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gkiudanfa.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/ggqraupwi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grgbexqju.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdogkbzjp.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gspgvdmqe.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gdtxrsfzn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gkqeeietp.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gtijdxrzi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjanigemp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gumdynfhc.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gqahtxugu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbfwoeufw.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gsqrwhdms.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggfofrihq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gxfliczkr.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gwqdioero.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnzxsceg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/glokzjxkd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gofhaoqxc.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gecjidpey.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gitwtpsyd.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gifcxrksu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/glpqycvga.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqkssncsn.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gmhtrormt.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/glqbcvzfv.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gfxtjzhkn.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gtjbvjftk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gxttilsvh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gwcnvjphs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gfbkivqgg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/glksywyib.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gttlacykq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gygudpgjk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gamtffbzy.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gstpombst.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gdzcargku.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gmgimrcmv.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gnieobjxg.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/ggfgfelwr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gcxwqerzn.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gkjexxnch.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/geptwbhrp.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gnqbcfvex.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gupdgzwce.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/goutwefnk.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gjdsjoata.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gbruhzbso.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gpakphncn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/grzclswks.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/girqbwnqp.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/govxdyvjl.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/guvrktdiz.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gvzngeowi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gsakcmaeq.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gjvrlxaam.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxowxnxvb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdujjsfct.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gtphgoanw.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/grrultebh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/ggkfqwkjr.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gjejsnnwt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gezyrjxlb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/ghtaraald.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gnqaczqfj.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gfbevicgp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gqhvlgvvi.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gbfliigvy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gqdxjhhxi.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gstvrlsaa.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtmuujilc.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxrrgkr.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gnryavyth.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gqiuaoqlq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gclinpwiq.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gccrzppnf.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gvzruxdvj.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/ggycdzddz.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gexturrsl.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggcfqshcs.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gijbhdiwi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glucdassq.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gyreiblfr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gedtphngb.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gtotxtdjq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gosudkwwf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ggfcirfag.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gqdthmgpv.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gjpyaswgn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ggifwinnx.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gcpkkcutp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbcfimzhr.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/ggaikfled.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gimnocqsf.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gyhicxppu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/geafexjrb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gsjrlorox.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gqvqmiyqn.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gjplztrma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gpouxodla.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gwiqppsqc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gtpexcoic.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/guocvflht.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gxdwzrxwo.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbgexlkgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gspeyzqlo.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gcgwfvntc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gjglsmupt.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gvpfavafj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gmljvkvwn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gghrjqcha.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gwnxbdxak.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/ggkyiddid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/glmfurexc.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guyammipa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gkcjjucfu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gujqexnhh.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/grqqogsnc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gylsuoqzb.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gpjhqpoxx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjoarvgqr.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/ggjrixrfe.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqudirg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gjzydqbxk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gpkgclntl.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/grqabmwis.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/guivceche.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gtxxzggnz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpdrbqyoq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gghircwez.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gkclccovy.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gnklkhhrl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gmxjcwoic.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gbgttjspb.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gcpwrbyvq.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/girjlakcq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gdmrqobob.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/ggzlfzvje.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gmoatcodf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gicvyimiu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gudmwange.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdotagdtu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gyfahbjot.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grdnuvism.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gokjbwzim.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gyfgyvyvt.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gcucmerun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gycpccrzf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gcicletek.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/golotrupg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gyjuknwqa.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/guehrakbg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gfnrpdvzb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gqeoerswo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/goswauzgz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gykqagzrn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gynjvfqkc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gjvgupbfj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gfoytzeux.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/ggmnqcqug.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gvxjoeqhm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/ggbxsbgjv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gamoxwmus.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gpnkqqpnm.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/ghflktcpt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gmtaoenve.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gqfmaiwrb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gwmwddepj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gmfjwypgr.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/grlpuleed.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/goulcagyd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gdjwgflvu.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/grmgcgqxw.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxnioem.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdokafmbr.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gbnyrjsnt.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gtusjanhc.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gdblbiwti.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gvmfnkcym.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gznwbwugw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gqajyukrd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gcfqnakpg.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/guyjgdqyv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gzibqehak.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gkkqfzbde.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gnpxsitfe.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/ghrkejluk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gbuqeylnz.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gmsyupmxj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gefthzudb.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gmofqsxgm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtbdytuxe.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gzkiofnpu.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gegmfqgey.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gmlhzaxgo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/goounhtmv.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gukblwttt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gqabrhdha.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gpneueaig.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gosvbmrvv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gnvmjcyro.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gnngzyezz.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gbcbwcdxv.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gluvhgcwa.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gdgxwxnmg.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gmevlifyy.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gkjytxuld.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqnghryhi.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/ggkkcbuzc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/glstwqvsd.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gwfpcwuwt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gekjiylmy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gjxnfbykw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gqpcxsyqj.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gsqnzhlgm.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gepvdluzj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gpruqonvg.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/ghnptyztj.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gqbosjfoq.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gpvzpqzlq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gfakhpxcc.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gncunqzdv.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gtevkymlu.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gpeyhrhjd.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gyuhjdoon.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gqqrpjuav.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/guutqpeoe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gucnhjtac.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gpbzblutw.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gnikpnqbz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ghpdddncu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvvkvmnum.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gklygjtma.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/ggmirwrni.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gvutagslp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gysnsuljj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gzvdmlxha.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gemrvrkrm.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/grahuiirl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gpkxgbxql.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/givyboely.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbfyptiun.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvxfatond.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gqicpalrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gfiniifhh.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/glceikuiw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/golqkxfcd.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwhvflqoy.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gfscokikh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggigenvcp.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gknvzqeec.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gvyucoyzv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtuhutqfu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmwllatiz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gxkfixzjw.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gkbyzyckc.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gvneukpia.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gaunavyld.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gbawgsgsv.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gfrxrdhbu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gdtxfvlhz.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/goxwdgkkj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gacvexvgh.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/givfuuzbx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gzpgnmcpj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gblaswnth.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gejngckbx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gufpzxesg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gybijtial.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gysfzsjer.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gryxslzpv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gvlkawvci.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gzayijkrh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/goinnqvhu.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gbyoxtciv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gigycvupa.sHtML


<!-- 参考信息 -->