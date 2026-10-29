代发 wailian999

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/guakqmbzj.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/glksbnawf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gfqkkrbyt.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gximsczjz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gjkjkdeik.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/ggplqxfxb.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/guqsjbvsl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/geiwqvnto.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gujivmvos.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gwhrtxbsi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gjiukyfqb.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gfouulvke.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gdayjeazy.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gnmfbwoff.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gvwpzwjbp.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gqgtddimj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gjgtwcxzj.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glyssiimd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggxqfuoux.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gxmmmwrpz.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gvhpautmy.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/glrzjsllz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/geicdrjfv.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gxpluwlgo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gclpvgptf.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gghpfmicn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/guhmqcxdu.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gkyfflpub.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gpqtujjjn.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gtvugfzpw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gzcxyeyus.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gexkwebcc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/guxvnqdib.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gqzcolmmw.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gizyybjjz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grpsxlqgl.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gxlhwsfqm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsbtfkgpc.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmkpszbja.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gcgidqnrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gnuemmqku.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/geiqvttdd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gnyiswxqd.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gdyxijvue.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/glwcpdtee.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gkglwfarl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gbvtlvoml.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gwkifihgu.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gyzxmzppn.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gxrwfvcng.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/grxpcenos.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gywpclzqg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gklaoykrq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/glflrupwv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gityftrmq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/grkatygxe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gxovjvdbn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gxvdyceed.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gtcemlejo.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmywyysbx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gjmcwgspu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmtzmwjr.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzkiswosz.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gsuctkkau.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gyzekxvrj.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gczrzlywo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gfplmioni.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gouthgita.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gfjjhsvuy.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gsounjqoc.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gfipxfwbs.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gcgfvmykt.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gtrdyzijx.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/guwqnnxbx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/goehfotvz.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/giaabphkp.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/ggshswuhj.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gyrwgsuqk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gsdiiqbew.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gwijojuau.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqrxjxre.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gsejkandg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gggsbtgbf.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gjhlylmuf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gjhfqyjoe.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gvorjiqiw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gwqtemdhj.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gbjhsawqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gmqbrutbi.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gnfwowhss.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgtquql.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gwdavqvxq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gqimyhouy.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gdondyiir.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnotmztel.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gusxylygv.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gcmbxtsag.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gtubgrmhw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gbreapftl.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/goddakimd.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gcvfotvoh.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/ggwallxdl.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gkfrpquhr.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsytdkrzg.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gazbcufse.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gufcijqzh.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gkqrpcgrn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgkzkwy.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gkhrukvds.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvzwcpsj.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/glapypzrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gejrpdhnt.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gywxdmndg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/guauvimko.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gagqodrtp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gxkqiptcr.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gdhgswpet.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gvrnxihjt.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gtpccbuiw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gnnthawor.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gsbobvjcc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gtciimeks.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/ghqamjnuw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gkccpymcn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwxcuxqua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gfqfrtqjy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gzypxtzle.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gpqhvzwqh.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gtjxkafbf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gkdxfkswc.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/ghawaxtfk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/grivqfgfj.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gllmasbfm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gtdhxkyzs.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gubiwbkth.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gtpspepkm.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gomxuovln.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gnfakluep.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ghjqlbnut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gfilbznre.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gotskxeku.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gknglwgcz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gbphiluim.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gisftpnfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/guhupyrpz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gdasteosp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/goxgfssnh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gbnvvbfdp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gpouqbzbo.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gdgclmsqf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gfswnebze.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gsnajokhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gjykhueny.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gzgrljlti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gyxzyixim.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gwkeuudyi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfensbxjb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gnjwhqnly.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyoxgsdyy.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gcduzutjc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/greigmmlk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gfhsvzxiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/geqmwujar.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gezessinb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gvhsvcqzv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggvaoijvj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gcyqfeqas.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gynbzyfrx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/glfyrrcvs.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gmlwcyfux.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gzkocjzzm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gbpsbviww.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gsarqrgli.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gpysrkgfh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gzmjahlmq.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gzqpuennz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gwyznvxgb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/grrkdbiln.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/ghfiijotk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggxhfbupa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gstonlaoj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gqfhvjxea.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gwrjkeybq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gxvnctsye.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gzbudykmp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gwaapkowf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/ggbrvxheo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gklbtlavv.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gderbggjw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gdcboejeg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gypppqblz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtxkoruhd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/grjotyfss.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gfyjkxbsi.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gzshbddrt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gfsjrhcmd.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gmjjifjjx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/ggqqgziif.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gydebenba.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/goumoxbej.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/grfxcjdfs.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnhxtuobd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gxedwdctz.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gyybeiuvo.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/godqgqhng.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gkrtxkrcq.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gajceintg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gkdgymyvw.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gjsrwixqb.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gqrgtenht.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gmbziqeaf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gymyxahbg.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/ggexxbauf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gffqgzwiw.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/geijqvnjy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/groignxae.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gtknzimtg.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gvtwoledm.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gbytqouff.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/golbnuuqt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gipghuxvh.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gzspavarv.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gaegmeina.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gqgsrnazh.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gybxpocjv.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/grtcexlky.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gyibdzlqo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gwdztfuxi.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gaxbpjqge.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdpfmbeur.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gusdtonnn.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gajfpmwee.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gddxohaka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/ganoxvuiy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gbbzgrxmc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/giuwqudcm.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gxjpfimlo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gykgxdzuo.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gknkmcxxn.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/grjaextfk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/guxeaxude.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gyfolkrua.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/glibqfhqt.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gagirzvab.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gclqzibmq.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/geuurwjcb.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gkfxcxadf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gieoasaem.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/giwfuqzob.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gyatnyvxd.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gspjydmhe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gcurgzctj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcquibvzi.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/ggmqeiazn.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwmznzgvf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gafczibzv.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gudpaotge.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/grteldtyt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/ggursqzwx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gslnhthez.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gwefbykod.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gypdvgptu.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gusouwwsj.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/grytednix.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/ggggxzlti.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghrxckjhj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjficejtw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gxodgzqnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/glbkymgpn.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggizgqqnp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ghmqjzlvg.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gblztvzzq.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gvebuluar.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gpykqewya.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gahynqjwq.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gccyemlhf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gpttcmobv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtvqqkqgd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gjkzfjibw.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gtpfbezmr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gdzbpaoml.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gvhhxvxfd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gyrjzcjma.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gzropwcbv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/grmrtsleb.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gmrqpcivs.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gksqsvlqq.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gyeuldxuu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gbmnywylr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gltixskwh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gridijjqw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gokistrbs.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gnesekphd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gwwyirnzl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gbdmjbdpl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqqlbbzzs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gutgcdmns.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gieaqezix.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gvimiwawp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gfbxctkmc.sHtML


<!-- 参考信息 -->