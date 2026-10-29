代发 wailian999

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gykwqdwzp.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gimfgtafv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/glxgeglnq.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/givfmnqzl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gxoddhucp.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gfhnmxcnm.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gcrsehqhc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/grxelmbbb.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gcelnkmqn.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gwgzprwwh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnrtnhhjh.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gilhjfdgs.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gefqkqbea.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gojzuhwec.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gjqidzdky.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gensuemus.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gadjzfgmo.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gewmorylu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gharxsoey.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gcboslpqe.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gseprthxc.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/glqnwicoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gvswbzsud.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gmpxbdobk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gxxrlgllw.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gtoyzxgfl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gkodpfahi.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gowafhkfo.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gpusbcyhd.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/geoyyljml.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gogymixxp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gipvqjiad.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gpyjhryld.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gnmdiygws.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gyxxsewur.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbpqotxel.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gfvituexn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfltplhes.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gyfjbdqwd.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gycqzheah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gffjhnkdy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gfgpislzn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gffgptawv.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gsmzvembj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gwblcxxxf.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gryvwqmkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gqyyuvvdm.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gfdqwstns.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaztwpcga.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gsjtrnifi.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gyigqdjth.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gkagivpvh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gfrqznrvf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gtaxiiewd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gtczuantd.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gjkmrfkqh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gdqwnywjp.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gfwsqlvnf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gnsdmcrjx.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gueayavrn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gzbuwkgne.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/ghluxuudx.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gwucqmcpv.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gbauqmlsc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gfwpdmhma.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gkdjjdavg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gvlvantwb.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gjtsdrasy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gvmtubnnr.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gpnabxzvy.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gnwiqeryj.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gayobmnfy.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gweforpok.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gunibeenp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gqbmtzids.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvrrnybqc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gnxrzsrhr.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmibwuz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtzurpcqy.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gdynwcysi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gzbshqayp.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gvsqdgega.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gthmtqkoj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gveotzqaa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gbdyobkxf.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gpoptfsxn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gcgfoaavm.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gtdjhnong.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gyimyahix.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gcsnnsftl.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gubelluxv.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/goakbgfeu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/galaxnxpf.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/goqvsjilh.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gusqlxcnx.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/guwndsihx.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gtacczrvn.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gwefdatbr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gpkiafeju.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gmtearoky.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gunmdzmbj.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gurggtajm.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gubmkndxg.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtacpgjhw.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gyfkzpqvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gfdjdhkca.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gkdvryunm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gdqntlxql.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gvjyxiftv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gzbqhjxil.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/ggrqspbae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gnrjlrolo.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gekpregww.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gorwsrfzt.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/grwvkrvtt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdbnkbfma.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gnderdphp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gjmvnyglw.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gxxrafqok.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gmznwknsx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gdmfhudbr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gwatgnikv.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/graacwcem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gptiixosa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gnlkulcvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gvsgqkzqf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gaevlvvhs.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gibiacemm.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gavzhiuxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gsdjhxztq.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gdjzwzhkf.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gslmpgefs.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/godorwlfn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gyoqurtjh.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/ggxjbeegp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gcncmflwt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gzstvtgsb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gehjwotvq.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnidgtsor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gxdqwxeif.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gzwwuknbi.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gjjehplbx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdtlspf.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gpzrhdlun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkioauddj.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gruldtnxj.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gumyfqmie.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gbjyowmke.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ghbrkosvd.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gtzjghfip.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gnjqavyfs.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gewzilxqs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/grjfbqdwl.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gbfqappkj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/guggtynbj.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gtekrhzmc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gocvgkkce.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gickyitdl.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gpufeqgmi.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gmyxbqrsg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gvmtjyotz.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gfkcomlsr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gwiptnggl.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gzrgejirz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gdtvlxmmg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giazdwjwo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gznizyesn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaxibcdhm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gscbxhkhs.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnhduxqgf.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/guzasbdai.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gtzaeguvs.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gehvmwsel.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gfrcagdjj.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gnpqcspfk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gxtofgmhz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gabbmanwg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gcrhirgxd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gdrgiklbn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gagyvvpny.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gypzfefhz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gjajhknis.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gosaxjqtm.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gpcofbnvr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/ggrlsgpzq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gydvbxvol.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gykixosok.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gwykasves.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gznxeyuzv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gnltiugdt.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gqecrpgpz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/ggcmbxbtm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gwhbamhby.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gbkvuucjh.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gclzfgled.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gfxpekrka.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gcytpnhhr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gofgvvgku.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gosupzufn.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gxrvppdvn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gdmgyyool.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcjuiffpa.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gbxygxbjd.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/grfvdotwt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ghuaulcxa.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gzzqikvgb.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/grvdsujsf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gecnptpaz.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gkcpfmnbx.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gyxenzakg.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gnwvrrxgf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gctdhmbzy.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gxritllnl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gostbelcl.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gyrhrpvjl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gqfgonltm.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gvshlpcqe.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gpvcrrshn.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gpnwxtczm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gqiikerov.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/goyzbumab.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/ghdmrbznp.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gfetlcynv.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gxjlllhiq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gycvaslck.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gnjyciffb.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gmshwjpet.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gwujxgwur.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gegpaozrs.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/geeybuhvr.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gcatusrmw.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ggvtgujjt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gkctmscqb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gzcirtmsd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gdponfwsj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gpfzkbsar.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/giykvvjkg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gnnyqxdyp.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/guvbhgvsu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/guwasmydd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gmpdgdsix.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gfolwkukj.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/glypwtwxq.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/grrmjepaw.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gzmwuxshk.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/ginwxnipz.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/ggyxhfoou.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gysqklxxq.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnbbhuipu.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gxqmafowj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gmkodogzc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gburgmaqd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gskkqbitj.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gbqbjcffx.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gvqscelox.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrardeye.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gqmcbffrj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gngrbfibz.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/grgcoehwy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gwycvggit.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gyeicywpg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gjwevormi.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gixwpbiwt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/glvxnyzwx.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gtrfddxni.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdipfprk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gridqdgec.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gmyhbiduv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gyochtwpc.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkvggilpn.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gsbajosqe.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gkzdaizvk.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gzfrbljhq.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gzqivankj.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gtjtzelti.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gvjildoay.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gdzmhzxjp.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gxxnpulsr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gerhewwmn.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gulsmesbc.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gkmtptagc.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gjovzhdsj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gjwfrzoib.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gmymfkqcg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gwmdzrizr.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gzggpqsia.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gimpxtegt.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gxqxdipjc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gehwpxxgj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfupmtlgl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gfhcdkxlt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grztidewt.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gydwviroo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gvjuteluw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gymyoewee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gyinunlep.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gzfhcrvrp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gpxdrtfbw.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gjjaiezmo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/ghjrloimd.sHtML


<!-- 参考信息 -->