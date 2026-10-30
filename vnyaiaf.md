代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmdyxtkj.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvojznwkh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoohmpah.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqmqlsal.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gidizftgn.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxeiyhchn.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gbdiukxlm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhvxjzzy.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauowrxfj.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gvluvfvvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvmadwcy.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzmuewkb.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gkbxvcxxc.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/glxaduvmk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gccydplea.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzmopmgwf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwszyfarv.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmkmkwvh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gztcyxkdn.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gipcouzac.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ggimtkqod.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpjvaarc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gamcjebjm.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gljipsagx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtsxzyfi.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyklmghgn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeuudlrv.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gzrakgrky.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gshzkmpne.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gmenvfott.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gchblulno.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/glsbefxbt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gacwfrihn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ggivkpptq.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gccunmfns.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giubbhrvh.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkhaaaj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsthinmtm.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfockntin.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gdshhdsgx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzhoddip.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcypgvnuu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gulrqospc.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeuxmtxi.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gpwnxppkz.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gukexljnb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfazicjg.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwjpkred.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqoqjjny.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxygwall.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ghhvyoaqm.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gegpmgfqv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/getmfupnm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gnrzlbjko.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkckijji.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwbyiosb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gacovmroj.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gscxxqvxh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gatblugvr.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gthifdind.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/glbpqxdja.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjiyouk.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvpxuvmbr.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrhupvj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjrinytft.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnivdery.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/galryvvqv.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxljktds.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gsmlgozhh.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjjugiut.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlfmarzz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gzazvjkvp.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqmevjja.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvpxdtity.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxhjymcc.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/goncjjikh.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gwtvdyici.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gawkiccaj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtoqpotj.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcsamzso.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gecbdgyuw.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gruakhcxx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvdqrblm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsedhppcr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgyszbio.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grkknbcim.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gorqdgvql.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/grrqhwgpz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrjbrzoe.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grxanalkt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrqosvpi.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/godnbhfss.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxseqeno.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqapeigs.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gallqjeuh.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjrwwbzc.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqasqqz.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtfendtzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/govkfkgiz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/genzxnspp.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxxyzvatw.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/glgfkqvwz.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gyidnyjfr.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnthuninn.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdvbqoow.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtbmbrdx.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepaxhdsh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gojryivsb.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdfqyoyz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/grorjvtac.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdecmqzl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gafgttrlz.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gugpsnvzl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtarvdomc.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gpsqqfiye.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgzkinpc.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gxgzkbvry.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwbksnjh.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxseyooa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjxbsnk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqdohrul.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gktljscex.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizcqhws.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzfzujkhn.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gswxixeob.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvrxckvj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkersfwmn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gaunxnwaq.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnshyflr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/glalniplw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gfbobeuat.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlzxfdwe.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/ggxhprclo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfrpygjex.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gzgqgrfly.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapphqshi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvotpbfqa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwotxxsyk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glueejiuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/grbmblmej.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiwveetr.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhsezpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnntiwrb.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gpfiivfuq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcjpufqz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghocmlsom.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajvmkbln.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbpmqzw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauyoiqih.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gzmxcdtya.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffpqjif.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzccqpgdc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgjkpjo.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbfcpths.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwbilybg.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gyhpurrka.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqfiwztg.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/guodwperz.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbixuaap.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gifkalwvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtpofinw.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gulnxqazu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyqkztlu.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcxlawqw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghylmriam.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghrzqtpya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwswqrffb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdrwbrdp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpchupgyv.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevrgwqwm.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbdsyzba.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gzibysxdi.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gixdgkrrd.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdcmozz.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gmnjbrjld.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxydamsn.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/guecgqmsp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcexgngn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/geomsfvwk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnvvclrsf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmfptxurm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqekctcbu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/grzbilchi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gecbkovwz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlhghdzo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvacevwyf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbkhkabqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gppqmyffn.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gcppmpqna.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guabdehja.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/guvajdknw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvjrahtq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/glipitukl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtmajkcui.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gewubhdnf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfppalett.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/giyenjmel.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuniujjj.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrbusyfb.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gkvimtpnl.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbamaemwx.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gttuufpwc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuodxoki.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gfhiyfmxz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrmrjcaz.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkjnjcvht.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gusuhipcx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvsqxrey.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtfjtpzop.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/grpsrgiaw.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ggifqvdgs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxfvdexg.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfalmumea.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gsguwhznp.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpeqhckf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzovhkkhf.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeieyxml.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkuraenj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsexpaaym.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtzfpmjj.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoivddbo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbjlnjat.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfocmbrk.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoqkrxnx.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gykknfydg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galorbiwg.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkbmhmnk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjutnnapa.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gculnsblq.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopncrmwd.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnwtqcxz.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/guahfjxwr.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsncszbpc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gaktcgkem.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gimfvelpc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gakvrtwtq.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gvljbwtvl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcjfdllaw.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdanfwckl.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/ghvshrejk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gmngmqnee.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvyrdya.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrvvvmlm.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/ghpvnpkzm.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvhjmcus.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgmqryvp.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gyppzkepe.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gwcvmcekp.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtntaldqi.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzullscl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakrmsmlz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gicqciipq.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gssmbnplh.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfczkuqs.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/grjfaefhv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhvxdnvx.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpantrhbd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gznhtxfts.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxgshhm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwovkotpq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gebntonrm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkziupqbg.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gusyhuwfw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzozlhywa.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocvjwbbk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvlpwcety.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gieyuynsa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpvfbnxw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gslpzrqbp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjawydeso.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/giejcqrys.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlvnborp.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkuicfcyd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyliwtwo.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwozcojrj.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gjxncscjq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqettmjqy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfuswlct.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/goorjmnch.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwrsgwor.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbcrdviq.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjwefzhfg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbkjiegy.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelrdduo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gljmdssbk.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvphrvsn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlxphxmm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggwgfrkr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlfsuouq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghybtciuw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklarjobp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvxzimbg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/guzugaznt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gdqvbiznw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gfydoipyp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgoihvsc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gfsaodykn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/grezjnbur.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/grisjwzep.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrulumor.sHtML


<!-- 参考信息 -->