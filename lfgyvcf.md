代发 wailian999

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gvqwgkxlz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gqcmyowvf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gisztxhnt.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/ggitslerd.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gvkuuihbm.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/glwddwlgq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/ghuoqndqx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gjaxtczbf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/ghfdrpfjp.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gcritqbvk.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gybcmiojq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gherkouwm.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/grlmvukfp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/ggxpvciic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gooadocby.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gahznefji.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gehavukpw.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gbgizcltp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/ggbdronrw.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/geeihpokb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gxlkdlnyx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/ganqsgjsv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gfhfyjceu.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gyoharefb.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gvkkadjba.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gjnubvwyi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/geryxhimz.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/ggscztwed.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gwhqdwlng.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gghswiidw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gsgqhhbtb.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gqcnacsgz.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gozjzlzxf.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/glvqnpuvw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/geheikbzw.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gznijypdx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/ghonlccag.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/grgtssefx.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gzvftdrwo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gveywylpt.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gbhdqojbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glqajjjvy.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzjtehbdg.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gegvdrnnt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gytgrzxdc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/ghqegjkda.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gqeqzidjb.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/glomwtzor.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqikzwwy.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gxiqzfsmv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gclgbtoed.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/ggdbkqifu.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gplarannd.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gzwjayhby.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gzdheulnu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gmbnbksgl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gcntvcdta.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvczoqgmq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqgyxkic.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gnwmzsvlk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gaidyxkqh.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gaagpvkbv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gjgiqaitv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gcciojzpx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gnyxqhnee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gmargblke.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gajscxsup.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gnflohgea.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gtjmrlgjl.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gklgvljdu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gfonvarps.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/golowqglq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gdrbzxtfs.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gyarfuzel.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gjmrttfda.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gyctjreeu.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gbvvtauld.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzriyuqgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gdaoicrsw.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gjyuqohoo.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gdetdgwpw.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gwviamxqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ggbqjngfz.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gjyjitkon.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gmfrvpkok.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gnsihumts.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gnvktixuu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gopejzvbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gpjmvnpwz.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gqyqcqocj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gvjadcmup.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/grlldsrsf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gzwnvpsbd.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ggqlzdmvq.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gxprprejd.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/ggespeftz.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gifunqpls.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gemeeoeqr.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grvhxrdlt.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gcarxaqxi.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gwdvxpvvh.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gvkoggrdb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gjmcxnand.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ggjnblxaq.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gvqhaxlhg.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gzjgpexfa.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/grofhmhkg.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjcommemn.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gajhnmneb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfbeaspyy.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gxapqwela.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gcgpjnnje.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/guevnhosr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/ginzpmtfl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gzrlwahoy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gfitaxyil.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gfuqiylau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmnaliopd.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gcmlpjsab.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gfhafluvk.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gpbkulylw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbpdxpzxx.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gvachceku.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gycbrmvgc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gxlmwjbhu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gxtimhgmk.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gebswycqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gazrpbuaf.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gbkffosdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gqugljcuv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/grgqyawwq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/glfhezuba.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gejyroqmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gipitxswv.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gzlhikngc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gopfgxzcc.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/giapwdcxj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gkwnlrmkv.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gndqozihy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gvucuprze.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gkacednjk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gtcjgtjfr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gyabzqpnq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gmpzxkxir.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gpvjrpnge.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/groogvcjm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gqtkaeqry.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/ghlwvbzgf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gwlkumexa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gspdkekoi.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/glpletkbq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/ghltzddox.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gffdwapvh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gbdzopwru.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gxgmldgwm.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gggbmmrii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gvjorfjap.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmkhroupd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gmqygxebu.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gxpbfuwrn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gmhhvrpgy.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/goyizetxb.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gklhejonj.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gvjxhapxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/glnbdefqk.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gwjrdbuuw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gohjezkur.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gzxptevly.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gmgjxiglg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnraiwxbl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gmmqllzlf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzvubzvys.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gocroaoct.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/giywkjmcx.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gzidxufdt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gmzycbjpc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/glswtrueu.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ghkbhrpzd.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gmxvbkafz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gvtrtemrf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gbkirbzms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdszmlt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gzqvdggwq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gsfxgocji.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpaymxdhk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdchtkzp.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gzcdksmhz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gluzilbey.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/ggjwsvxoi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gstawxkar.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gjclqcnfa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gtkcscerx.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gyudwsidw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gjfvqxalm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gsacaaecs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbugkovuh.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gecfowdnk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gehmzyudx.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gsihaabiy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxybcvppk.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gznpcfiju.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gqlzcuqak.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glvaeadjq.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gjiwhzump.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gqbyzuiea.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gjjomedup.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/govpqrmeu.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/glhphggww.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gjkhhpoyu.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gyvholwsb.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gxuduqvvt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gqkkbanys.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gjpsnrppk.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gehvdzdoj.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/guzihtmdn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gnpqolzrn.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gbmenrood.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmhixvatx.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gwvdgphea.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gemhbxcig.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gfpcshbrh.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gisfjipmj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gacujpnoy.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gnrwrxyho.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/glpbbzijg.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/glrtnpelh.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gwuxlploo.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gxmggypkg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gbkwjndfp.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gvccqfhsl.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/glolskuia.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gexmuweoj.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggmyfcthb.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/grxtuyqyk.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/grcbnuhpi.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gfficlswk.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gyfwbshmq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gzicgwmkr.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gyqbmeblz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gcrukmrxo.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gqytgzxzk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gnbhfesyo.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/ggkrcqzol.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gaemtuukg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gvnpinlfv.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gjnorgppu.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gpvsdccqx.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/glcylvpeg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gdwpxlwwo.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gestywksv.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gptdbroau.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gferutdvs.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpxrjpfhs.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/ghvswembk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gcrryhodk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gdmzrwkry.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gnarhtxsb.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/govcabgep.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gyrwhnogn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpokdsv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gebabpqra.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gpviqqrxn.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gaizksvfe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gbkuijkmi.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gpsgpckev.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gbcskofmm.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gjblnfqjh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gkkxqrvxn.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gfehgumkj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghencrjsk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gdrbzauug.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gftosnbdq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gtlculydx.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gudigxscq.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gpedjajgm.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gmqwyciht.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gcmzicvxd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdzcquxri.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/ghswxylhq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbyqcfszt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqxhmqjpo.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gzhxkltdb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/glrdubexo.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/glavihjum.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/grknaefoj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/geiqhvwxz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/guapvjexf.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gokqwdftz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gndauswgw.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkdcfompo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gjnkdnpje.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gjwpqyxuc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gajcbypmb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjeshxbut.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gbechmggb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdczjlfnl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gtlfiomtt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gjeizmwhn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gnxpajscm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gmjoxkeft.sHtML


<!-- 参考信息 -->