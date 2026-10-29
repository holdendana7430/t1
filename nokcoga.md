代发 wailian999

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/genyblstl.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gyyktzvbk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gadbpuhte.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gfiigihat.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/goyouvijr.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gwwwakudx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gmoreumwh.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/grcthhfsb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gjftjhzuf.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gmujyqtgj.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gbutbbqgr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gmbzqdrbj.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gcxojpbhr.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gijjizpui.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/glbpmzqbf.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gxiwjqhyp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gwxwlxskj.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gifcaxzsa.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gvoqvjzum.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmvuhanyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gtivyqwdo.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gtbbeabsf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gcapnxctt.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gipiegqhb.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/grkgfvocc.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/goobikgoy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gkmasyagu.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gawhimaxm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gxcceteps.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gxyzpcner.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gezxdbsel.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gwtybmpoa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gfogwdrhv.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gehuledhx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gdqgrwnyz.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/grqgorsyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gwnyrbhet.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/ggmhriglt.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gfgbixvwc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxgqkofvm.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/geuvlicmt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gosuvgzdn.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxkakmriq.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/ghkbgdaor.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/grvsfjtcq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gsenmwqlz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/glnkjehsd.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gxnmlnyys.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gvfzotaiv.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gdwapyvyp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gakysoxod.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpvfoqngn.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gileqhnua.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gqghiuubs.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ghytkmnbd.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gqkslccps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gsclxtqfu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/glnqwqfcf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gcwuhgqsy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gylqbdqqx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gqwkzkkhy.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gvcmwzqbc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gushyyugv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtwmlxqga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/ggjxdrsqv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gdrttsvxm.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gpcrsmguc.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gcfwdstlj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gzgrknpyh.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gvxfvxcoy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/grayjbzcx.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gsfgmhnzw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/grncobqyn.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gkzdxkutb.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gipgpdwuo.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gommgeruq.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gbkjavhjs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gtbdgnfsd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gfvxtmgzk.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gvltnxqeq.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gvhlezvxs.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gobljitps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gppjfalzw.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/goyxdzxck.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gtaivwtnj.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/ghrzwglrf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gzxesdcig.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gjwhldzmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/glvrqhxxz.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gwexacare.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/ggoinvklx.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gjcvtaana.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvdonsijn.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gdoivodsn.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ggusykcfj.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gjflndixs.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gtftpzhmk.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gqvdevedn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gcxpvdcmu.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gyrbnkjaj.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gbqpoxgvm.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gqkojwhkk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gkatieolm.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gfpofchaf.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gywmmmrqg.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/guzejizqm.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gbwxyxsws.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbvymqkcg.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gdrwkfbfo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gvtomyxbk.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gejliflma.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gynelqerh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/ghyelrilk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/ghmhkxvfz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gcujphsad.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gldvntycu.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gumtaviou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxbuvluql.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ghvebcety.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyegnsuvw.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/ggmwapkze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gpdxqyupv.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gqnsrxafu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gukddlrcm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gjlfgffxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gucqvtlcr.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gnolvyvcp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/grhbkrkdv.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gihezowjd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gecevgfoc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gltxtmrhr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ggazatnlw.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gvdrmcrwr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gropmtyac.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gevnvmeik.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gopnaairw.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gmxxidfkv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gbvfsvhwr.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gsceyustu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gsmovbbfu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmjzchtvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gikhuzvsw.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdhbwfrga.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gyvnyfjdn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/goozzayrs.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gdojtlkrg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gssgenoky.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gbvlayztz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gqepeqbmp.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/guihlcobi.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gborcbole.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gqhjpcngj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghrkclqyc.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gblqggmdk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gpzjvllxl.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gwqneidwg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gbcplbvfr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gtkqawtat.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/grenrnrvp.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/groapibnn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/goifpvozu.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gifywyckk.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/glierqytz.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gweuiazlr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gupkgzrup.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gdfrwfctm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/grpywncuo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/ggwvcrhpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/ghehwusnj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzrbfxmvb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gfruxcmwm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtodaxage.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbsrjrkbx.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gayzjigpf.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gndvopnjp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gexiqgplo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gcukouoer.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gjrjmjwwy.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gthjspplw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gqjqwbytk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gnzoemnax.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gpmfqxaim.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gcywhvmnd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghocdwrir.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gplrxmznj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/ghdfdisye.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/griwodppq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gtduabqec.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gvzxikoya.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gifoldezx.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gjznkdzje.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/ggqswspbc.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gktidbisn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gbwjsdpuy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gadtgsnct.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqlowlzie.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gqqkcxpfx.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxktsnmiq.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gmncxyxrs.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/getirmeik.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gfocvnalh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gniymlkvi.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gwyxmyxiu.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gnqwxoslf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gdqcuisjj.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/ggaburbtx.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkymztxwj.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/glzhzfevu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gxmrrreqn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gxmvoevdp.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gmoufreag.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gejwhhmat.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gscinfdwq.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gupbuvudc.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/govpfoqep.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gcetqlwps.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/ghouydqhc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gailxsfcl.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/ghwuxhgwm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gnwcmutaq.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/grbpyzexv.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gvjhldfqp.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gipocunet.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gauwzqjzf.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gwtkimkpr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gyuwdqrzr.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gaqjkvaag.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gkarohbre.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gevvdxbad.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/grvrysopk.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/ghanldtil.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gembdnjpi.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gdrplwvhf.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gvqimackc.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gswmmsods.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gogzuhnsz.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gowymwaut.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/ggnsucamh.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gggholkyu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gtoxkrvsw.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/goseunurr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gfcuojjfl.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gaqpwoduw.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gsipuxamt.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gxdxvewdm.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gdfjmrlrx.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gnqrfrsux.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gssojymvo.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gqaqqhcph.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gpfvxosob.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gvxvgbnxu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gocvremsy.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gqxwzbqyi.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gxextofrj.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gesmpgozb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gchzhkikk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbhxloaxz.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gnayyawww.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gmnscmjif.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gexermmzx.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gzcueuryq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gfvjvcpdb.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gufulpmgm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gigpeykns.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/guxzoladd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/geghahigt.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/guriyidfh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gcybwbqou.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gohnijfbs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/girglwprd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqqqttxau.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gxebousuq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gcovcxvun.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmuqqiyyb.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gngugkygy.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gbwyotero.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/guizpydsh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjglkelvw.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gxlyivyuf.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/guuwpeyfz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gfyajdhhp.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/guqpdhdxq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/girypwejx.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gouaneysw.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gkpxciuik.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/glmpezxxm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gkhvrgusf.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gbvswovba.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gwpbrvpom.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gbgpjapns.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gqdbuhelc.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gkurcsnja.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gypphsupr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxtmmpdqe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/goqvzveax.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gryxynebi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gilotypfl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/ggdpmndfx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gdnkdhcuh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gpzwqqero.sHtML


<!-- 参考信息 -->