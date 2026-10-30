代发 wailian999

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gkjzuvmyy.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gaadzakqf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeqgweja.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnoxtifa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gdrwvqvfg.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gbffctcdw.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gznetvdsv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gigeqtulp.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gutbqtnmu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxzcxmwn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhqkkirb.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gzpeexqod.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gutpmtrse.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gfxogpcoo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gekkzzhgv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpyqneco.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/grdunrpps.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gafmsqwlt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grknljaxg.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdasewups.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfonxxjs.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkgazem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gffwgtfop.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gusejjsbg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gmdueditb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsxtezjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goytuzrog.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/guzhvzosy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggydwmnci.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxpsbwqx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gftrsxvqs.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gdifdijfl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gljivtwnf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxaxyflg.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gmszbryqp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghkajrdtv.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkgdnps.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpodvpvp.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlfbzyvy.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gkfytijrw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gponuvqbh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvatbhlqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggudsaizw.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gsyiwnobw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnfzrytb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggngsyffz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ggiykfmkx.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxrlqlfk.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxydmbypu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqykvznns.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gzqstavpl.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gkfiugpdl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/grixofjgc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gcnmmxfea.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghfslpwne.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkozrukoj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixiejigu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxehppdee.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gqaujbkwf.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpaalslu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkelqmdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghezwbkne.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvwhrane.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/geyapzrij.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gizptugik.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdoixxzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gnfmklfsb.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfopuomg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjahqeta.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemlfqbfl.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gfucumvib.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggftnefaj.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsfeltkpe.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzhtfqwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gesvfbucn.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/grhywewrw.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaxhuisl.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsiilzxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwheqqjz.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwaydxb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gqolitcdt.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhvleeds.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtewtuevw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuuimwlw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxtsjmhm.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/giovgupny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkxlzzyw.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/ghaaarzxl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrohhhyj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvchutbv.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gzdnryrzr.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwynvjnrx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gsfuilsnb.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gzhnaycrv.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkkdqbjn.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/glgnxpcdp.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gxibvfixo.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlvbmuso.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gctbrsxas.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbucrdwwg.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gckqnaomm.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdaylmzay.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gtgqitcnw.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxrgfey.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwuqpxxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghshxaghi.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwymgmuek.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbgmwbfu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrellgfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/giuxauffk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhssukqd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrmmcvo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugbmzeua.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwemvifhw.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmcdraxr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfgpgmns.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcpnbyuj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdltoqhi.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixpvakkw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/globullni.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggufkueeb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gtdxmpevw.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqbarpkwr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyltboqah.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpiwazotf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdhzjecb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gklikjvds.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gbinfhgxb.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjwgzgbt.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/glsomolub.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/glmfzygyv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glitnljyt.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gedkglvls.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnihwgwr.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqzynyu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/guhfeftpz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgnfzygv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaykvlwjp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjttisgoi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqpotjlk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glgzfryqk.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgtijvew.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gcphnerub.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqvhyrmba.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ggwkwkthw.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjhsisrhw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftufnbiu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gobjryeey.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtoulzkwy.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gywxyysym.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gwjbekdqm.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxnxjfqiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gupilakhd.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gaexvaddh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginidsxod.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnptepgll.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzefnsjk.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfnxeyfv.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozrpkeyf.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjdoubts.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnvfjmm.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gfayuzhof.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbwxmqfz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gczhwdiqj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gytrqmcci.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gedgeygnh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxihperl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkokjaif.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjxozpjzc.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhsykyez.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhlvjhup.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gblngacga.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuottrgz.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnidbtsja.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gmtshjoqg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnidnuzr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/givnqecng.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxawvasd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpsverkd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcmrhvcvp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxmeoupgq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvbmmcent.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/glbspbwfa.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvgpicumx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwtyuvdik.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/goehrsjbt.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfvzbbhuz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grnkkqjpu.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrbhzog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gidjqsfwt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gycxwlymt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrdbvzoq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gqqklcxmn.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimyuuoly.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvekydsbo.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjhkgpsr.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfzwinv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrglfuin.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gahitzhon.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqttglcl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmmufsrp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtafeaal.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/grlzdysoa.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/goewhdyxr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzotrqiu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjujxtgrw.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/ggjxsaxzv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpabslmo.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdekudbfe.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqovopttb.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwekkebg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbchamdcw.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpqojfxz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gpvsjhidn.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gosgxihvm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhplcsuw.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/grwaeuaji.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/ggfpwtcky.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gbcnhqzkn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/goubbqshe.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gecqrrqtn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpskwfmxi.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfopswje.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbelewr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfuzgruh.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gvisaykjn.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gykmkculm.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/grkyhjeke.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotitfcqf.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzejemyxx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikohhzkd.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyyidlvs.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqazfuja.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gdhumqmwq.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gqzrfprgh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gohadzyxu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxojobgp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghbzkahco.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsakcftfa.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/ghbwxjrep.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gqpribkkj.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gmsnsnkxy.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbgmlvwy.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkuhoxvk.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gflzeinlq.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gcjcusrwo.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gwdeovsab.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gzqzvyuzo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghckxfxpm.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gjwwbpvlt.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplzjvpak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ginhwacox.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gexahepvo.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjwacvn.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/guusbqsoq.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgyfbgn.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwnnfblus.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfkpvvmh.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gpzuspqil.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfvtgtytu.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyniydno.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxygejgr.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvogbcfn.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvemqgdq.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gopyqsqyf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gelzhoepa.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbbtwckd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgspewzi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcedwldm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxicalbt.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqetskpci.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwdiximfc.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkuywnzwi.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzhebdmsj.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gytjyukgf.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gattdngky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmujdznw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gnglhvnmf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gogwqiibc.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gxwgptpby.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmmndswh.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpylnoelh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gtzjofxtu.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gpjzucmhu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gexporjvy.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfdzudptj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfktockpj.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/guocvhugt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnbzpjxv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmcyldqsk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbcocwau.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsgjpvjfm.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gczsfhnsz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoldnzok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gnkokaplg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzhdoydk.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/guxthcxhv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdljuhwj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkuobtbs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gvfvxddtb.sHtML


<!-- 参考信息 -->