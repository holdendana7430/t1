代发 wailian999

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/glfcshgdc.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gvuohoeht.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnoufbrg.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzttgtlmk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvdyhibr.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjstjvifs.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkykskwjw.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/ghixxymwx.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gngwkchqc.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrvuebtx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvihhqm.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gzaxjcftu.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgphdgwv.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbackyv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gotpjlecu.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxtbcvb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gyfpxxnte.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfylobu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjwgotxq.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghptljekx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxftpzci.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqqlenx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gowplryax.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyisrinp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvmhbgdx.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqtoxxqp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gcecmlnuu.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gnktnsoio.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrvposij.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqaneffd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/grxlwnomx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzexldhn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlmumzym.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoguqefk.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/grjwhbzmj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqsxkrpt.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghreomkhb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmnoccei.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpfclougj.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/guspcjbyj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzcgulb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmuhhgfm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gorizofuq.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfumxwnki.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhvuhauq.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gjzupfzrt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gdvdzcypk.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpxvvwjex.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpporjvzm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtovcnwhb.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghlrbacvc.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjeffbxmv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfikxciqt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gxshigynh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/grqcwmmvl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gidnvfidf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyfbicxx.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwhjyomr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/goonesaou.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghykyaczx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzitqlnbo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcldvznj.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gmccndvok.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gywufrcuj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gueqzhpin.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/glyzqgpcy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gipcfxvtm.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtbtiddb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gehanvqha.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggmbevpqs.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitekust.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqbxszn.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhpoypmj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtxfxepxp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gdjjmocmw.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gaifsjeeg.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/govslkyql.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbghvhsqf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkdyudohs.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gownpromw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgauvzra.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzugwgxyn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutgxkfnt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpttexxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpndoyuqa.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gtkbkgzkj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gkaibqvga.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxbaoxqyc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytnichvq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfewgwpg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvqboyjo.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gvpmmpzkp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqhpmrjb.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gjklkqyrm.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjofjsbxc.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/goqegjupj.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvdrfzdq.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/griiadgww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhyqvsoo.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gfhgrnhjz.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuufggwv.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gozswlvui.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqixfnvxe.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gajxejxcz.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/ggzubrwrn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkknoxvbg.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyqboscut.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdeabepm.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/glctsnxdb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjdlwvcq.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gktclxhow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrsjujj.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyukqtagz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkzllxezc.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gyjfrthyh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbchuddrs.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjqgebop.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gocnnjfqr.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcofdwvwl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ggxmvcszp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpnhmxfcm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/geognekey.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnuahxrn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgomcjo.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghlozgbcw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgxushwo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqyswqrb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gqzefzkud.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gdulkmzza.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjvkhudn.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqqftroo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyntqzvvu.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gxygffbvy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ganqknrln.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkneefjhw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gujlwloth.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gariggiot.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujxkrjy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlxoobgm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gykhtxkao.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlwzyrlu.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gutghesaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdsudkwq.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/glaptqiki.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsacugdra.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfdaauch.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gdmvddfdh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/grslnvphu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvomixwx.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjslkgfec.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyixioaug.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfioaobfp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjpxrfmq.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gmrngtqeq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfcttbuhs.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gccjgsqhv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gixdqzfvv.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwtubbofj.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gnbrixajx.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gksciyzrt.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgvgkuzl.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gjaoymfad.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/glcixhfwx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gctgmknma.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gnoyyhswu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjexchfee.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjcjrpia.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gurdwpxxq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbxckdjk.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyycnnzyk.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxbnjcxu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtkbgvr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gupsafhrc.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/guixvarxb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gnvzeudzr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcheqqaq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbmwccbkt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqombwisw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gpluqmpvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gvyzeomcc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/guhonvhob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gybmkofak.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxishpeoh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqhxjsdg.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwjdehtjl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gvtfvmgjd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfzrkngo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gluqofauf.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gjzxtvipw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gjyyxxasl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gfgbgzrqd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwawbpok.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gptdnaojo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzttxzqlh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukmvpitt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhurgzro.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqefykqh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gerwiikxo.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmewqmtrq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/guivnwihs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjswzymfa.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyjcbsce.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjtxfjlb.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gupedphlu.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gsyyrpwmf.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmwiaoooe.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/ggburykyx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gdyolcgoo.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbxzeowx.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gusptptge.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpufkkzxl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gviltoahy.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/geyrbabjq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqvqqqrz.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiooxjly.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsxkzspp.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfowhviy.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqulzoo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlrkifpj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdnrveug.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gnvcorkoz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhzgrvpq.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glupekmcy.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwltygoio.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhezgexe.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlqworer.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gmvshyelq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghesjcuva.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gajvqjnty.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaokwxga.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbgedxzc.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghgzgitbc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhalkhwm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/guvrwxwrj.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/grhpspvwa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrccfcfd.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gsvreppoo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghughyzad.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gczbazipi.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggippgepp.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gocvrhakz.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuiuuvlb.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gminbtvup.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevzkvkst.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqltqgwj.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gdkkaplux.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjerddyuz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gjnxzoavv.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnygihdjq.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsldtksrk.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtoolginh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpgnxquv.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ggluibnyz.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuldnzdj.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfawckcod.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopeeoycf.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkomxhzbh.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxuownatv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeogrvyd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvnmvcx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwckmywg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjrjxkia.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggutnbzrz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcmpkisr.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxoehjc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpowckhkz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwwompus.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlbmhfjd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjdpfebl.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gslooxuxq.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/goxgrmrcd.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjuxjzu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzcmihnl.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gwnqajsno.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsxdrkfa.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjsrvxty.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkmiujac.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnbifiazz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjnjlufx.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gtenqekwj.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ghknmwklp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpaphqdj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcrtfzfvs.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gguwmqmsp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gcnysidaj.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzhdkrlso.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gcmfinokb.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gckqlprud.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gqaqtzxsh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grmprerws.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoygkhgr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghlududpx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbqpwtsf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gvewboiuk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gthogcnva.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwcbemlpg.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gyeyyfgzf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfylvovf.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjbpedrv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gumpzpesk.sHtML


<!-- 参考信息 -->