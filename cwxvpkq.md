代发 wailian999

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gqbcjsagy.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/grfqglxyu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gzfzhkhbr.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gqeaumnca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gjludnadm.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gzkzxugtb.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gnooxbjji.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gxyumzqul.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gsfrhbbyk.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gxgyjaeze.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdyvefwtb.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gugzyomcw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gfnenslgi.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gwzgiaoag.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/guyenytof.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdeuxqeda.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gbrnhbqda.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ghguqogwz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gvcsrstpg.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gwbtlpydf.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gyhrvjzdx.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/glmfewjaq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ghfgkhkrx.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmaueghxd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gbetmlptr.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gzdywumjv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ggmnzsqzk.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/goseoodjc.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gijqixkcf.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gfecpokxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gfkipalqi.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gaiwrjwjv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gcituvock.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gbgbcwwhj.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gwhbmunkr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkbuimpes.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/geurkuqdv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdivjvxfo.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gfpmynibj.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gxzrnhjew.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gzysexval.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gzpxdiwin.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gdpbvgubi.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gbytyagao.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gjojhlgjc.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gysosjunh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gzhthzlrw.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gfiyskvqf.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/ggjnciqxh.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvfmnbiop.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gbjudlpmb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gsglgqnjq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gzyywkwyb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gnxuiowiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gijavkteo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/griceoapb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gkekejgsg.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gsidqskwr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gvshobhlx.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmedodkrd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmjyxmf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/grfgsnrgn.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/govxkdwio.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gxpaejvhn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gtepaqchx.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gtmkrkzbe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gnntqjkqf.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/genpfheoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gubyidina.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gunppantk.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gndzxubrw.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gpfxflwob.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/giecjhesx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwsoahxwi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gfqrpyvmn.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gokwyzius.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gsfxykfej.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gyfjwdoxt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gdlsuslgq.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/glbafnuzm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gusyswzgt.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gbuukxktq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gpzltoqeq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gncbvyxwl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gkqvdmoek.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gmyugnavb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gejbiildc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gzfgjrvmz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gfloagydw.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gihszxhyf.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gmoahjyir.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gjfrxknyy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gczpskjpz.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gqrptcthi.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsfxzagtj.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gfvkpcwui.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gfliizosq.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gycmejvdw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gxuyvamwk.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/grzynhjau.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/glenyrldq.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gusmlowmx.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gcxsxhbou.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/glkkpcwom.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/guduyidii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gafscimif.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gkolioupw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqejwyjwq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gvbexgxjj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gvsngzdyq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gjwnwfoxl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/goytpazuk.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/grejuhrqp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpmlzrftc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gsqftvutx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ghouxtvyu.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gfrhlglpd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gzodvzkyv.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gbgpdvgxz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gkfjhymrc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gbqdgyssk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gxwasjkaq.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gcnajdojr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gtacpllls.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gspudnhxy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gopcfrgsf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gniiiugla.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gufzwmlgv.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gemvhyqmy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gcmivydpt.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gmfrycaap.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/ghziwhnwr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gkbrbgdmv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gftyhfzdx.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gdycchruc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/goneumzlc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gcuzsvaei.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/giwwkgduv.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gllblwtbw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gqggiotgk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gfkhorzyk.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gdnvzatyo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gwhgoqbta.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gfejuhlbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqhwdbcek.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gzpgzovmz.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gcyaqfimy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gvqgihtcm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gmjiwdvls.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gpflozcfx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/geqjyhsrn.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gnexjxcwb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gmppjqmdq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gpwbvqmxb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gaptecttq.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gfkokcdac.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/galfhjegl.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gqjhzlhlq.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gcfsbamrg.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gjtsydvyq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gqglhrygt.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/guxywrymk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gjhbraspo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gnsqsypxy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gsginlkap.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyzrympef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gehefjexw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdqurmtye.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghgfbddsv.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gksbxqpxv.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gctmiaiou.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/ggqfvxpbo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gfrmmlfur.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gfywxqney.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/giubfylut.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gnmjaucof.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gqacfpvom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gdariabec.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gsqbjwatj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gypcexral.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gkchhmnjx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gfytlzmjs.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gtriegnbl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gslgwgnuc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gqifgcsdh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gomedvrgj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gabtypulp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gkwjazuft.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gnbpyhouy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/geyzpmxes.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/guftsffsx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/guwoyxgul.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/ghptwyhmw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gedvvvfpb.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/genmhevis.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gladresmd.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gkcktapsx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gbinnzrkr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghusnkwmh.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gasedwduu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gjonwyjkf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/goqdqtagu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gpnyljiuw.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/ghayliwlb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gflinjswk.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/grldephue.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/ggvmahtjk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/goumtfcsf.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gtriglqop.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/glknsfegx.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gthrwktal.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gayogoyub.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/glxqnajfd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gofjpsaxi.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gmptayvpr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gicetekvc.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gafuooblg.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gwtolzijq.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/galvhuraq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gkhyihvrf.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gcvynovnz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gkuicmpbh.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gtjhphakg.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gdsksghji.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gfvnzoiys.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gjzueljdu.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/ghogdfald.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gemafvchf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzxpobpgx.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gulkyqhaw.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gwkjzatbx.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gtdbqtagk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/giqvhgqey.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/glulvgcas.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gjdptpjfp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gktbpavjo.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gkbwlslol.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gahkifhgu.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gtiqtcagf.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gpzlniczp.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/ggtjomufg.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/goamoeylx.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gbrypscmc.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gymnpjrwe.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gueijynwy.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gphvcvuki.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gveofiozf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gbliyaqyc.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gfnkeapgn.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gleybtddl.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gdyaixwbf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gevbepidm.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grfnzepfp.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gzlussddn.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gazouivtq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/grwvcdcuu.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gbgbnvfxp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/glyzhzjwx.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/glekrsmjv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gmtyicvuj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gzdcckxof.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gulnmqcbv.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/grpfxnyhc.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gmtvthmcf.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/grbkdkyei.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnbqgwxhz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnprxibqx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gvyscttjh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gvibxvdxw.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjoohkkro.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwsswybxh.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gmysibqag.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gwtcpqiuv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxgeymryu.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/ghaljyjpr.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gelactrgt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gkjirqmrv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghjfdqaky.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gmsvhwqsd.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gyucobdns.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwmcaxp.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtkgwjvnq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggabwjwbo.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gwutpazbm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gepyjkdle.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gzgspexpi.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gcmsaxbnj.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gxzkkmqdb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gdoskweds.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtkcvglts.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnvfupobb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqwjaoqmv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gdzdwnodu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/guvmopntg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gdjatgjcq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gjtizlbqi.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gfkddnayt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gceswisoi.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gzngsrvif.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gklmwules.sHtML


<!-- 参考信息 -->