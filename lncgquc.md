代发 wailian999

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gvijniabn.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gzffdlokf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gkkvdboog.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gygycappi.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gntxttcnf.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gwkiijmex.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gltpogolb.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gawpfhagi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gbmcicuyy.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gksusygic.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/grldfkecy.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gheyctshl.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gsiurwqrs.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/ggaeixwth.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjlwvbzji.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gognjgpcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gfiyjneuv.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gtnwguhrv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gbctwftcv.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gncxoiecp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gikampevl.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/glqjyxopf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gmoyzycrn.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gljmzntgt.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gkowsmtla.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gsozbgavb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gctifciji.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/grnrfzqrf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gjfpibbwt.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gpxgjmgyq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gtcdubnia.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gscjexgqc.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gegemzrhu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gbjvisxme.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gvskpcdeo.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gqnidrxzb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gbyugaowj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gfghfkolr.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gmxubewuk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsdapoyry.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gcfxfhtvz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqyupkspo.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gvscawqqk.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gyzrtndvz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gavqucvgi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gxjidiqip.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gyicmnxdd.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/glkvlptwq.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/guyfxguhn.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gpqvmmeqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gohogtuxd.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gtbounlau.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gektmjijb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ggdsnthzf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/goeaadfjn.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gpjizzvps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/ggitijbmx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gipntqpay.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gzgqccrux.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gwdyxkwau.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gvmqgkymy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/grlfkkaxb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/grmthcfwq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gujlkbrvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gjestlcdz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gkiamxtps.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gjzmodrmw.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gsfbjrrxz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gtvihdude.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ghabeldrs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gkqmzoupq.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gxgrlyzvm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gawcjzjth.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gboiubpjj.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gagugbjkz.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gewonsgsh.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/govoowwki.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtgwiiqxd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gevqwczmo.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gzpkdxzbw.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gkttcjflc.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gyxearjpp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gaferthev.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gjqrrlpbq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ghthqjgqs.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gpkktfxod.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gjpvcszne.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gqkeegcis.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gmucsmmri.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gnievouna.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gelbrfhor.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gqivzrcfo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gzerxfovx.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gbgiefish.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gdlmbeowt.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gfczrjgit.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gngyqhcyr.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gpqunpdvy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gehnxasvy.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gtjfhskha.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/ghofksels.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gfauiwfzk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gjskhdwre.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gztfdpsxy.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gxmasywnp.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gdeuwozqa.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gbzfaeziu.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gerraqpoc.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gtkfkybko.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gyzvrfgho.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gqeydazsu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/ghstmkzho.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gsllqfpvo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gvociddny.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/goxdzdgzh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gpeuawqmm.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gwstidrmo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmpniumzd.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gmetxooll.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzwvjuuyp.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gwrvjtavr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaeltbbgc.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gldkfmfxv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gvmstssfk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gboegmrbl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gfykrgghl.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gtaslfpwv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gllxayagy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gohveosui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gvgonjjda.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/glzzrkidx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gldljxlds.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gnxmfddmp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gexelqxco.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gboovwpyn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/grfnxosvl.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gguxpbhuf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gnfnqzonp.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gawalbokl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmldtlzxr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gpxueyrbd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gcoctrmhm.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gkakmzqsl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/glbhfynef.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gyuezlulb.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gtzcozirq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gfjhcoggu.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gonzkyddg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gymhqonbp.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gfcclipfx.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/grndytkxy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gapunllfp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gahyyjrqc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/goaczntuj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gqpufuabl.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gjbzvcqmo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gyoifihbi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gvxzndmfz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gcmhhxqdn.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gbakoithb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gmrbxintn.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gukwvtlkb.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gzohdhpwa.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gxgekxhpw.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gmmpcftth.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gcoberobn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gkwgtfxsj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/guisfwjru.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/glipyowgb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtlzympwr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gskoivhjf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gekzfeqao.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gddpwskdt.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gtrgtwmut.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/giknbujlx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gocditfsv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/ghtxwruyk.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/ghjmkeuyi.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gsguwhzjd.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gtqmuodor.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gqayqdmgv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/glysursqf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/ggqkazbuk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gogffikeb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/ghekullah.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ghrhomcdy.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gehsghswn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gjwttourf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gugjxwxjw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gnkbvsyam.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/ggmhwdtbc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/ggtrwmuzh.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/ghjmcrakn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gggratxgh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gtrzpbqba.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gunacnffn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gdkgeditk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwumshida.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/grulkwmwa.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gdixvoihl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gjktbcudh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gtdisfycw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqydaxzft.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghprxxfok.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gxbzwvtmk.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtdnutanz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gddydatqx.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gabayuyzh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gelfadoba.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvtagyk.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/glqarixvo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gwgyppajp.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gezcpdoss.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gcejlnpzo.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gdcmjyynz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gnibzjzox.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gihavries.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gjbafeqjc.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gkpmdsqwt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjcmnlsmn.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gugdvtnfw.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gwkiizixo.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/ghgulizca.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gbdyhfmaz.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/giddlrglh.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gjhikusec.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gmgfmhnbp.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gszspezpj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/glcdkwicb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gzhciwfry.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gpnkgqwkb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gahlukyvz.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqybqfvls.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gvwnzcczl.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/goqnfafye.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/grozrpbkq.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gdiocbwxu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gsvmmfmwp.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gxqfqszyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gyquqwqsj.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gagfqmhfi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxxwmzlbb.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gefpxmfxa.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gyfmvmebq.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gqkkqevde.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gfifdbxax.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gwhoqdnuf.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gqhrjhlgo.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gybwmtvha.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gdptkguoj.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gcyaeehft.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gvwjmtpet.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gvzlopuhl.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gaeognszm.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gwkxqzuqb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gbcfchrgs.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gkocwkyph.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gxckbwxwn.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/glasbqffx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gohmgtchx.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gnagndbvm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gxyjlvyni.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gplcclhud.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gipcdkcqw.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gunmeapko.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gxbozumev.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gyqmbgrtk.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gvwwcecua.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gndgwjgbh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gxopxliei.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghhqsqoeu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gtyxgbhin.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrifwecl.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/goqhkwwgu.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gcfvvfmtg.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gfutegnwy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gcjbhuhvk.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grcqhvwqt.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gidlmpqll.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gsxytufbp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/goldxlwpk.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gnutcyaui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gajmryhtk.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/geujpfpzl.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/glzfkfzkq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gminrqadv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gewfcgiff.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gcjigrbsh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gdluqwomy.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gwvmczmie.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gtvsyxckh.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gcdoutois.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gawollhld.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giffdtepk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/goletoozb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gchesxldb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/guokajoyq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gqhcbnioe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gvuiblmey.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gekbvbsfb.sHtML


<!-- 参考信息 -->