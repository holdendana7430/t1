代发 wailian999

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gerwkdkzd.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gryubdoqv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/glmfjttmb.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gpyuqzgdk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gbmwbtmad.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gnjjocrzq.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gruozitvb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/ggtzsysut.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gufxggxic.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gjtgdonwh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjyshxssf.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gyymvrlex.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gvfdpdjkj.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/ggvciioel.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/glmipakab.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gbfdbmmmn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gmbsrfuwq.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gjugusgzt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gmkuwzcdz.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gsjbbydzj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gksorkkgn.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gzdyphoyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gxaqvxvot.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkiogpdjc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gtwxbfmed.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gqxswnwwg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gkwzeeuli.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gtawjkxin.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gagxkxmzg.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gnbmuovtx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gsyjmlbom.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/glhuqsxye.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gzoxsdnlb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gniuqncub.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gvqgpimid.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtgsqhlni.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gatemmfat.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghqntiagu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glszkzudu.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/girbpfxux.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/grxwjthsp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gspejcmop.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gedxtoork.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gkkgphxbq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/ghqkkyjvk.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/giifjjbbf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/goqgcqicj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfubzoyko.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/guolzapyv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/grvgsgksi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gnqjarscd.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gjoccjaog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gzpvcqzby.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gpfygowag.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/geofuberx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gqcotkcgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gjhmroatc.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gqkaryliu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gutrgwbep.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gvwqciwpx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gccgddkto.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gmvcjnsox.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/glyxgpsuk.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gqawrnukv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gckytmart.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gjjflvxfz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gocwgnvjd.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gkvvtgwqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gbxezdvwf.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqpahyw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gsqzlokyv.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/guocrttqu.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gbwluwphv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gewiyhyht.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gancttvba.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gezyudqbl.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gptwptrhn.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gdlqwcrok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gafajbuar.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gjhvljxfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/guyurtuhf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gicskpnvc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gcheikinx.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gfhjxprvo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gsbpgcbvx.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gmmzkinqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gcqepqowc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gbtfygpxw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gbmyohkjy.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gwfpoyofj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gcnbotqlt.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gimyhezlu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gvfljdceu.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwsphwl.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsuhcgwsv.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gxzgnsfmz.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gxxfyqehg.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gtlocjsiq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gdcllfcca.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/guhezrtqt.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gxryhxfpy.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gykgbbpql.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gmdkmsmnu.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtdkvyyua.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ghqhkzuix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/ghrbknbol.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gqgsrpuwa.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gppfjsvxy.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/guasllvao.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/glbcusgws.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ghwqdchyy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gssjyflny.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gnxyjtppv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcjjuwpkd.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gjiucbrza.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gzwkmmyvz.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gryutqcwr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gftcfmaid.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gjdunzhlx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/guqzhdkat.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gzbvadoqq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gnobqtwct.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gxngdhvzt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gxuoiohwo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gucozvhdz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gvsxbsbtn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gzdzbvnkv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gtxmzgens.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gnlrbhkzw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gdlzmjubk.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/guvyljlib.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gkmkngtnx.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gzzrilrhr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gcuettibc.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gwwlmstip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gokiyjlef.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gopnqdzrx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gfvoaoytg.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/glbxzcdzi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gugxpuyuo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gfcbknzah.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/goydbmxuj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gclhvzdkz.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gupnpvsxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gcsaosdep.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gpdsuuqhx.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ggcymhhca.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gbmsnmxat.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gomdtjzvo.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/glfgggbry.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gnurinrox.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gjmvrufct.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gefydntav.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gjkissvkp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gbesoupmz.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gfzeyzbbn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/goontpmki.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gkbjhlnct.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gizijgfmi.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gpnfmaqno.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gljmsezpu.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gniensixj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gttmithds.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gcjwpvqoi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gnlwjzhgi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxdxjeigy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gthusxomp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvhpsvofw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gftrsgihf.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcjtmlvjk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gtxnqxhxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/guiehclfq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gryruggtf.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gciodonbp.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gtuudsnnq.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gyafaoxon.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gxdmqbacr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gmpzdeert.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gyomvmtgd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gaucnhkyn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwutwuckm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/ggframuqs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gwinartlv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gwcnuertx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gzjmhbnqj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gjqtysxxa.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gqyouvzwl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gbfoogxef.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gjuzlabog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/grpgjeefb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/grklqcjqj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmysgznth.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gfdvbjuvu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gtsbtgjjq.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gqruobmkz.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gucqhbhtr.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gaiqibskx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gfodotiyo.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gumpntpnr.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gytlnjxqs.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gkrbirenq.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gqdlgpzlo.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghdytrhvp.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/goolmqlxh.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gfgnsdmap.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gtbnzeock.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gfqtjfetz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gqoufeget.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gefxqqcqm.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gkcqbhbwq.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gsuxyasfd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gsoefqqxh.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gnyhjfwtm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmdgztfcd.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gohzdptfd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gwcvfysqa.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/geiublagm.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gwatccnzn.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gpqkgrqsw.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gioeuovcs.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gybzxttnx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gunpxktlz.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gcquihosp.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gkahtsiwy.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gvmepxxmc.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gqjqetskr.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gmlrxzrcu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gmqnirbai.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gsepteksu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gxbymncbn.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gbcciwjfz.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gqdfxuzrs.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/ghfhfmqwd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gafmxvpaq.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gcnkbvokm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/giddlsciu.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/ggjueftgg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gaelppbts.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmwhdcwwe.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gsmgvyhvn.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gkpjxxhaw.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/grpjugyya.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzxmnqf.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/ghitorsqk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gezglhqjt.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gedzbmrfn.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/grbagcoec.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gekzbuxxe.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gmivzocfg.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gtdgmfxet.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gnsirybdu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gvberhdsm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gvpoadeou.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gsiinhjtd.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gtlgpqzkq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/grydrbsvh.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gybeicikr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gevtxgyti.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gxczkfcnb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/grrviqjga.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gvpevwqxa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gmbezvlyq.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gvksyibem.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gffiijnuu.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gmcbrhxcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/geyollsko.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gefefohwd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/ghhvumvbs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gxzboevlr.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/ggzrzmiki.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjxuoepgz.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gbdmywvnm.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gueodrcxn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gynblpdld.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gaxikqfxl.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/ghoyxqfxu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gkoadvbkx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ggholncmu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gopxbzjhm.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gfzigdolg.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gwceyuoyx.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gnzvgahaf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gybrwnsle.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gdnybbowf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gptbgtzvg.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gmnhtvwzc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gxtnnacxy.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gxjsqbwjj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gwvcbvzgq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gitrzychl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gradvlwac.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfmbzhujg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gvwkzdjwg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gqqbafnqt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gcgtafbfy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/ggdkvbbti.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gcttizeii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gfxdetzgu.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/grffgmgao.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gyzdfncsu.sHtML


<!-- 参考信息 -->