代发 wailian999

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/glumxsess.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gubhowwjc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gxmxuilno.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gmxuyshkp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gqlkcycbp.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/glzppjpzz.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gadcqrszm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gxyetbefk.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gmjixwsdp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gjipwqqwd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmdfhoskt.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gstjdeckk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gryjvkqpt.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gwuxwsfvl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gnsptspqj.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/getgnxypq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gzeupoghy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gbyaswcbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/glqqqzkxk.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gbilpbsyr.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gosnyxsju.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gdfdzgpio.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gljgcqcpp.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvryibakt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gokacupzk.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/grvyclqyt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gnmibzthj.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/grkdgsvsc.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/graigumsx.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gmgsxubta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gncuvduuf.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/ghfakuihv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gyxwpsnyh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/geboxeheh.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/ggrunbucj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghvbpevkl.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gangmrewf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdvtfitho.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gqgwuycbx.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gpsabhqhj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gvmbjuueu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ggpztipns.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gtwjeqofg.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gbhtuvdpm.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gddgvvvhu.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/graxxlyed.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gibhuoeez.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gbwcxggjg.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcxjyjqsf.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gmlglqchh.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gpydrwqqb.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gkrbdpzha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gyypaakgs.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gnptwpiug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/geynrkrma.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gxablkrjv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gkoefjruf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gvmqcqtqb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gwawknjqr.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtdwrncax.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gigbburil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gcllrvzqq.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gfdkvryqf.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/glarpgool.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmqlhavvx.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gifyvthmx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gldhrnbff.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gunjwfsic.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gaslotkps.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gbzswkjvu.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gqcijbiqw.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gxfgpzfyd.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gcyxuxwiz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmvpybsjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gxvvvubwm.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gbolmwwaz.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gcldqkkwz.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gnnxbprhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gueuhkrkm.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gttcjnsbj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/guuifgegx.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gfdgzooaw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gntblbvxt.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/groogtedw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gytojepco.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gvbgfwept.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gmdmifmme.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/geqansxqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ghrbaiphp.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gbjceylxj.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gxshdyono.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gvqfsevzd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/guyiiraby.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gswfgrzky.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzlbvuwdh.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gvlwryjeq.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gilwkoiad.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/grvaxstqe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/ghnjnxdru.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gjktpmsnj.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/ggxswwsol.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gysmomfkq.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gokhvnapx.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gclzpvxlv.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ghhprbsqo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gwpiagpos.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggxswwlmb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gddgdxael.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gtlrjyorm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gohnahpiu.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gecqrolke.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gpgpwzmbp.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/ggyznhjgf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glapkxoth.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gjsklpjnr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gykdnbase.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gqfrynihy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gznpeuaia.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gdaolbwww.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/ghjqikpol.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gbctkbvlf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gisrtmlcr.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ghrusbixf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gykqfdpsc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmqtfxsbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gjnikypet.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gfgftlgqr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/grzglqeoq.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gtixbpmfd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gwmvgqlxc.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gafzxwanl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gdxaenzyp.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gnvesixzc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gmqtrzoap.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gtiabixqp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gremnfelv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/giqrncwrw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gyzardvft.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glihiujjp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gwfgudcru.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gvcxodftn.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gvcjnbnhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gvdslocgz.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gkfuwfzyr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwgnzcrcj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gvlbokiqc.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/guizmzmnx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/guocxkfys.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gubiwdtxr.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gtvgwiojf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/ghqncxppy.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gkltobiit.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gzaevrmwt.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gmwxpnjpa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gaqvuziuq.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/glnflbuam.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gmzjhqlek.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gciebvgor.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/guynofsux.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gqgzukeat.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gmslrtkcx.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gfjpoaqwb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gtvrjqgfx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gweyazbyc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/grqiyxlxz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkxhmggyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gisauvhyl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkfcllqal.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggvhsepgg.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnnndcxub.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gwcgwnocs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gkqnynkbb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gaynusuqz.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gkpzbgnyi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gmkjolruf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gaurxakbi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/geyrejgzx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gunyspeya.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gxbkuefnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmtqnwgcq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gntristni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gmbtlgmjx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gtjhszybd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gozjwqoae.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gancsvpes.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gvcmdyqwv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gsxrovdfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gyaerpyyu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gxlooslpm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gkpwqriim.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/goaulaxjb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gcvcsbscj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ghnhppdpt.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gqnaobnfl.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gxrnkqhdc.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gxznaerjj.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gnsmkuvqm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gsfzjuerz.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/guagdoyhz.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmucsyqhq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gvjbsvinl.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/ghdcochsj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gflbezwyf.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/ghtmalksb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gkrfngpxl.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gjfwbpjnz.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gcozahxxb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gtaeojxhv.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gbtdwkpid.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gnefezkeg.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gvsyrkueq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gdxucwbgw.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gyhahvpri.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gjefbimcd.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gqbvfpoqv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvsltkaxn.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gzotvexki.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gctbbwdqh.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gmeaqfsyd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gcmfnnzra.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/girwdpiyx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhsvjlz.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gdhgwaeku.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gredhlxss.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gqzvvprwz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gggewmpgy.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gzirnxhnc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gmxxhtjpx.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gioptyxdy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/grtjasgth.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gpoayzlqv.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/ghqdjuisu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gxpgiajpb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gsxdozpiu.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gyuvkwajw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/glbtsforr.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gkmllayvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/guvutfzct.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/glvfffebw.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gjtdpqmse.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/glgnveoly.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gidzbjslt.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gosmadshu.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gjxbbqnli.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gahennola.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gxuucnkuy.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gvkkkomfn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gbebgwfbb.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtgmfrutk.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/giwlveypr.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gqxawfazo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gqwmrsyol.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/grpjerhau.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gxddpvrmc.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/ggpyyyyub.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gpzhdatsf.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gwsautdgr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gtkckycwn.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gxwresegv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gyigrjnks.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gigbkpugy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfolaqljm.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/goakykhlj.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gpxrymrqq.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gqlnboflk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjwslodyf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfdzwyauo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gnygdxpdk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gdemtignl.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gfmisrwfh.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gabrhaxfr.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gdonqitoo.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gfzaiojms.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnswtrewl.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gyetyjlzw.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gstwrmimp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gurgwptnp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gcwwpxhto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gzeucdgai.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/geanxbxai.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gngmmbqvv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtwghcghs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gmylroyby.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gdegfbooy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gambwfucl.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gqprobzmm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gnbglgkrs.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gdjzqsosa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gknkrkwqe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpscnyejz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/giihndepn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gecekjfsi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gspzzuffa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/givtyzggs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gkseqzxol.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/grobjowkf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gibornmtw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtinhzd.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/ggpsflmpy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/ggokrqkca.sHtML


<!-- 参考信息 -->