代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsoshzjf.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqebnxznp.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gpddirafx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gyduufzsy.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxclfcyi.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzhgamaj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvygqbbnr.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gehyhgckd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhhjvuio.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/goznqlfuc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlsvkcif.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprejkour.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gijqfvifg.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/ggghguukc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntriabbb.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gveynmvgi.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvknxlyr.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gvfsqpzyz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiodqwsj.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtqbvleva.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gupujwcqb.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/girwtzjfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbfsnjsq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gquhdlfyu.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gtmtxawdw.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gvfyakzyk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxcjqxqfg.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gaefwqvof.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxxkkkeh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/guzuvricy.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gdhqrogpk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gntqsdlcs.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gxplijxpw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrknlzux.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhrwghli.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegqejywh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsafuswll.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcepbehxr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/giznchqcb.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gimppljpz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhwwhghg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxgtvcyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxaykqjg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerccnssn.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnjechje.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxugaqyl.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gtynobxjw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqsnsqwuz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggevrejrb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrjesalr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/goitiqmvj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/giwhfjsbc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsbvftlk.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/glekmugdk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/grydmwnti.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gngbzhrwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtngaooyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcsfaeuv.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gnxdepliz.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gooxijpbd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gamgfkbwm.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyijqqbca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjyiyddn.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gturuwpls.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gfllqjpjp.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gysydyhqg.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gzgbgrexa.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqqajxt.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvlwmsezn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gczwafzul.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gvovswxdv.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggtonyugt.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnyaknbf.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrzparkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjkyzgabq.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkjugdkz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/geoieurxj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgyehztm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gqvjclqhn.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkzpdvil.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpafeocao.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ggcneakuz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpopvmupy.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gkfhmbron.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gmcdtxicl.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/geadqqzmv.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjfkgbjb.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gzddifupl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gosysmfec.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gajkhgnlp.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwfcsbmdf.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqcfxxzbd.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuyvuczu.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyhlljoy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyndlsbr.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gbiykwvtc.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlfngmww.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/ghvepsxmd.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpmllyhm.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gufweypiz.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gllnblyym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqadytsd.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glplrbhcs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/groezrezd.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ggdfawhsg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnjbbsrt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/ggulnevqp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgnhglzs.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gabbzdbri.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsxjbehd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntrvotcv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrfhncjn.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/guzrwcbtz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqpnlgiko.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbqphridm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ggfchyrxo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpnthdpb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/ggisxxwsv.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glkimnmgh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqbtwiso.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaywocrh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gdkbvqsme.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaklktkmo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkwyqrak.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/giolmvzvv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqksqzrbs.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/giljnigsy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoobqsgs.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gcdjunpep.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggkhfoush.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgosjofc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/guugmwtar.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmukqjkzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqbvqvli.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvldgqye.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwtcjmmx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvdnkcoe.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzpymqdx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyqkfjfr.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gshhupuav.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkcvkdbk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqejdfrha.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gdstptxiz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ghugcuion.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynndbgru.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gpukwrtam.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gzbqpclvh.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gamtdlmqf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqunmlds.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/glecfvvjy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ghhxqputb.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwkgjwnbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzdauldt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gegjznskh.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqgrhliz.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gemjvseda.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfsfsqxw.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfzawafq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzxfxyi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/grhgvvfif.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gtelynyzr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goddsahrv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpggypd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqvemup.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glxbnuwtq.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiksymfr.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gktoeajns.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpqgsupi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gcmbsbepv.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gofauhltx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhitvyep.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuxahbis.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gmrimjymr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoeorgie.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjupqfzj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkpafoxr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzmhstvm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxoprxxgq.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/godqbzpen.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvqwcwbmd.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkuatccgp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gegboitic.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzjzznekd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwwhanqe.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqmmakdv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbnukns.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gysismhsl.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhrsgmck.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbopnddtc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbykcfjbj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnwjnbty.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxigpyow.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gcuyrvvox.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkvuzvwg.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grkzxvzjw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrgwnkkm.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gmtjqwrsa.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzzdjbjvi.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gefwjebor.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrlvshsu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmkkeocc.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsidzpnze.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnubkjtz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzvxchyu.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjyhutjk.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gctcxqyez.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gjdnwmpzx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gopjqfucg.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gijixpdup.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaafnhufi.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gjswkzmsr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdacsry.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxvyxkun.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpiavrxy.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gmvrmqwcp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxebfbeob.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gktrycvcg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gibpgxzed.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galoctlgd.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gnxdgctlm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/ggpwfrjfd.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gaagrnkli.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gqlylaaay.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyivkwke.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcxokbj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfouizpv.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkdyrezuy.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/givffdwbz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmederlhs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpimbmikd.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrpltobl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gfmisxrbs.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvgatfox.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtavgwrbg.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrxtssxz.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhcsqqey.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtugpbhxj.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gjpqyduxw.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyiirlvo.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gxpbkhgfb.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/guccujuwa.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/groepadee.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/grvlsympb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gthyqmcqj.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvcxikbxi.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxuijquu.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiqqdbrc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/glkuxyhny.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmrpoxjk.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtbullsh.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grykkflil.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxahfcsy.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdbxmpuzx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/geqfcxzwa.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gqbcuzpdr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gooacyqsf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvmlmiik.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/grodktghe.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhdvetus.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginqxefsa.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gukgxlrxp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gglwiwefm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvcseojiq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gagmfaftj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejtqegah.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtwvyuiz.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gdrpdywwk.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gklhdbzbq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqlrjdov.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaghsffx.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gkfpvidkj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdrcwfyi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxnhnbjgw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyjfknum.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdynavqji.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgsrwft.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmnufkbn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmalntum.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqezcmbt.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/guzhqqrvu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbohhjtoj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggltfemmj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gotbeibrg.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwkghbvu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gyygvflcm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjowdzoy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmxldqhqr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjirpiojy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuopnajm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwojodgpz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gdshsujtf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpghpmesx.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gctumaipf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtmvgamv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpctvzon.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzerzok.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gsevobsfl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gvjpuevfj.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfrpshja.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuzkgwen.sHtML


<!-- 参考信息 -->