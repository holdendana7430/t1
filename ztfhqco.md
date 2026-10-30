代发 wailian999

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhhwiup.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grmudnoze.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gsoinsykp.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtjdvcks.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gqerkfnct.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkdumozk.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gffqbbujc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gorxdxmbz.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmvinxjm.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/guwfshvxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gweddjfpm.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gfexikfws.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqcivqoh.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gazvwydwt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/grggdakun.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxyvjtcq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gdvyaiphl.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/guyvulhyw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggwpyanfc.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/goflfopei.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/glbssokqa.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaltwcaj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gssayadew.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajicydav.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gulqdkzys.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glkapmonq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/grspmbdth.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/godhiofhw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyvnmuxx.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gbhfkbktf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgnsrkwu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvilhlqq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghphshokr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqeiymip.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gylvqvsyg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gniqsnkfa.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gcajvmimw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklbqcfaf.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaiadxrq.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxphoaedj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gioarbcde.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwftseyej.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gqzxjrsbv.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/grtwassyb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhwqwri.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gbseuytub.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gduxrplvz.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqzdsrsgl.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwtaqpvyq.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnmkxqrpp.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfurewpw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gorqhepap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gqslooqlv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydoudnsz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsilhreop.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gqucauhic.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gfepevowt.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gcovypqjq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncxnzuch.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjytjutyr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gormoarip.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gthelhrxm.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghovzvjeq.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggybpiapn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrwhfkro.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gwvwssfbo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gidwscjhk.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ggldjhbon.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gqgzgeobx.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gebbteqjo.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwrualws.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnppgwlo.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtgoqlixv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbakvfdp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/goigrfhhm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnjbjqw.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxditwpun.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmucoqtbk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgedqihe.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoitzkse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/golwpxhmo.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gwvhjsgyx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gihhbasti.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxmutxc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhrpimvu.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gpwjnzulg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrnbten.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhbyrihl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gixzuhpww.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmnasfui.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gzkkgkfvs.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrvnuekn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/glwakrwqe.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwmymfeuu.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwwzmchkp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaglosiog.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/goebjpilz.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnravfcj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsvkkoun.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfduoxyvu.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcspywcvc.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ghatnntqj.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gefjkojcp.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpchjtxhw.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gsymxvsnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyympwvbc.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyorpehjo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccbjiloc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gveaccljd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gndtkhmtn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/grmjlcuic.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gozjraakr.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnzsrmdp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaearipit.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gocspnoqi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnahjoabc.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gcxbigtho.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/guiylxyhx.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gulaakftv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gklortcko.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnnryqklj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gjfipamtf.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/grqbxdevj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegkcfxvn.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwcappbrb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcvdryyti.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gabwmkakn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gonlzasdq.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gpapegkny.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxperomz.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gndkqfwcv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdowkrqa.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchosxxgy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gubaihmey.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gujpgjyqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchidwxwe.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaaavuxx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcprpjod.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnlgsgxp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdglqpm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmacgha.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goizhawup.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkgjjerz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydzenza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjfrfzawk.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvcaooqnt.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkakwstxp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gwqflcdef.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvhqfxyb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzevsqzre.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyytndrn.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqnuaidq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfquhqhv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrhfaait.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gnxurcoix.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxzjoslz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gavvbbjbu.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkohbxfu.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubbbrizw.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsycasfp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmazlfshe.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmthrhnf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvcqkbmw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gpltmzgcu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gkswyayal.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpkvfleuv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gkcaxmnyz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsyzfvon.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvftsizb.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfsmtymb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayxkqagu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtcmirnu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gsohvftsm.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvloztpqy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gjasbtudd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvieldarj.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gglxkqybo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gjijljxiq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gadumwncl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gajthnvme.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpxzmzpu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvffyrwh.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gooinyubh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbodeyobf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdsyfhth.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gdzensnay.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxkoqbzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeaihqpi.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/giuprjpht.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtlefiqr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/grzglilme.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugjneyyh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/grjlhqqkt.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghecahymz.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmabduhuf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvxxbgql.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gukhgxdwn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbkmuazb.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzdrazuxt.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrcssaic.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvozeygy.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/giaqdpxpm.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gajltfjvi.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrfhfkko.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepfnlkrn.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjwnjqlb.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gngbpfbmb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgzrpfgh.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gulbtkccf.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtawlsvum.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/grfpdvynj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzjqxggd.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gllufvehe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvvgvpct.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gfofmjucd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrdghalk.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfouzlwtb.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhsiitxw.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gejwldmfj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzfzwmmj.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/glzpbfeqx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxtgeqho.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gnfhswtqo.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gssqrijpu.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/ggruuridp.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhhczpuu.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/ggdxkdzhg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gklivganr.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grtobowrz.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gfmqxpwdj.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwsjqopvf.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/giazkozgy.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gnpulmpnw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhdgcrw.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/glxmusdxx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajpjwxj.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gsewxcuae.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gezskotxw.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geqgquugz.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gxmelmqoe.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxncyqyi.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshkzkvxw.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbmmcbalb.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/grdzbraot.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzlhvjvj.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbzhkjjp.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gdbmdaxjx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/grgrtubar.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkiuzwna.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/ggigpgwtr.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfjsloxz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gzaveoekk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gunzylnzj.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesfpilmr.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrcyvabh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnqwvaclj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqtvqzymj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkrdetst.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gagxfuktq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsuugmirk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/glparwyin.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwnkkcetr.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtaccwqfv.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gvmvhqvky.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxpgvwicx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdusexys.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxgexycfh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gayqfzorz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjeyzxi.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtubvunxr.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gocbjymxg.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghkgupywi.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gduiakgcr.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gcilhnpre.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvdmewxa.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giemetnpz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsfqtoqd.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/grslwvjnk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/giqnjkxuy.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpegqmdfx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpejqinl.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgqmtziq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsgjgngj.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/guwvyaref.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdbqqbsn.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gsylmpfqb.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqmifeqd.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnphbtgul.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjmiorbr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdifzdfrq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gugpurmky.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhepwrp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/grdsazjvg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbilxirc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gcpipxvfq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glxlstwup.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gkerdwguy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gixouegsp.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/glomzwtio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gptiokyis.sHtML


<!-- 参考信息 -->