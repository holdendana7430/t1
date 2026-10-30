代发 wailian999

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkydwghy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbrrzynq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnunoptfi.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyrovsmm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgbjizqu.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqmzoqbtn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrmhokkj.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgzomxtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidimylik.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrkaydys.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ghhxxzlbe.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gntzghsgm.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gxetaoler.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqfypwev.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxssyjwal.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwrksstx.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gkouhsitq.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggzjdlyna.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gulixzbhh.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnsczaugw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/glcpvqfra.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/goweckhfg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyshekgj.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatsvxeun.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gphlgkmqh.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gshmykczt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnjfrthw.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gogvkybvw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnmecuyn.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvdhdqwb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrobqmeb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvxuipgj.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ghtsfthsu.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/grvrecyvn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckdxdeeh.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gfwsobuia.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyodiwtar.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaxbfnnp.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gugjqitpi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdcqohvp.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlnhibbp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grohyynig.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwrjfpoc.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gmkxqmebj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxloadyq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiobsivr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcqruyhdr.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkseobedu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gufpshnqg.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gcadrzsoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjscrovc.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmdzfms.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaqmptvn.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gncicnsap.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmxqthnv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlssytwn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gekmcgnms.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gadhloskg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyhjarta.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gjefexkpi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gnsbswgje.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gorvlpvxa.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvgjrvwj.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnlqkeeur.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gdbtyfzpv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbbxuake.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glskfzfsm.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmeaxkoq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gultxjdmp.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmkfrzifl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkimfinei.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstjyybcp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzhthder.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gttbsvmmz.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gluruspvd.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gsglhdepb.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gajsxegqb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzopmwpf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqpkiruh.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvusucclk.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gocjwpwha.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnysglprp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvthvbvj.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxtuidp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwfvdrud.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gahptncec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gulxrrobc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogssiben.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqmjklbj.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gdvxrhaht.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmtfxbhk.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghiqkdxea.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnihedvp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtsnssnjs.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gakckjkib.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlbginqi.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gacopwmlp.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gduivtrux.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkrxsqar.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdqqhylwm.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvggxosrk.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gemxyfpjm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldavcwa.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbdcthuds.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gentmbltp.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrbwwfb.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gyolikixt.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtnxizsul.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqvylamd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvvtxduy.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxijrhsqz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksqavjuh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgwmqqjm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgewjpnq.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gxjsvsnsd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatshqzyn.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiglxsum.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gcaycwbej.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/goayocnls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdogojcrt.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkqoaeas.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzetxspmj.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeedbwfc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnmywtpc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpxapinv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhnferqw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/giauzrzkh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtktcyjbz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/golweemif.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpezjsbq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gziilpfuu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjifglhi.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gujazrmrl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gmjpkhbdw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkobdcsa.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmcbaxhv.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ggjjmrtob.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrlismsr.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfpdcsip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqnrhdgq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmxnkdyn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzctreijg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gplobotox.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gtcoohvqy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtclbzmvn.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grxkzmmpd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gpxrkmwqi.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gupnwarwz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwbpkuhx.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzapxvhol.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzerubpoh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gehqlzeqa.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxjdiuoe.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/guvmdulqa.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkscdtjbk.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gltnfxcds.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gapqxppbu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxximmex.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gdoqqwhli.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gnnhilptw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlgjdzvr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxulegklp.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhxmtkaw.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/guboyppnc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlopheoj.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gntglenab.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gwjnuprsv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsdgodtr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/grmwfaazr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxgmgxwhd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtncmnmn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gswlgqbrs.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqruydqvt.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giukumchh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggupoelfg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gtevtmqzb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/giulkatfr.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwromgui.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gwjhztykw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpxqmcmx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhufnole.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfoboxdt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gzkzndryb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ghwkdtzmd.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gjfseeeqm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gokriconn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwqsawfb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gggvxrxds.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/geflaoijm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gqtvfknkp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiedgcoi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gritucdvr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gyocyqmtx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gokmzsysv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gtpimcecv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfebqlmcj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gxdkcrdmz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkotpstmd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlakhlgb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkfgytpe.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsprztzq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gvngzpjhg.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmsocsw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gynlcbnaj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqxrcojx.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glyqwkpyr.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkcbzomj.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gudtembui.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/grawsinut.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqrcfwxs.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypjaqzz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gjnrpnxqq.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgrgbmld.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapeeibsl.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjyotxkln.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjadxaknn.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giephgsov.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbcmkeoul.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gvkckjuzy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcqeulhh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvodjjqh.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gibayijzf.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gymxmilgp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbahlmgv.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycpisugl.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gydmjaxbh.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gixyhgxuf.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gdflelvhg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gucdxnxrc.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gmbstzuda.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgyymmpe.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmmntkkmx.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/guchczwba.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljfaaguo.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gthakjroi.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grczgxpzw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpflmfmgw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthemepjk.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gqgaftrbj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gibnybyqc.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggivdeuiy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdevktow.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaodhgktl.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdwpgbw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gxywtvulu.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghacgsbps.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxsckccr.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gflhxbjpz.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/geynldvjq.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gaqgzfrxd.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gjlvmbqsl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gugqqcgbv.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoqnqatu.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoocfxco.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyolxuvx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gyhozpgfm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/glodzfkkh.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gocqzmejh.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/goprttmxn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gglyczyue.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhukukg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooomyncz.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbwgyhook.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqmofjqqr.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gvalbslsr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/guunybgoc.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkxdnnf.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gxsugvvxe.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsggnemlz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gydhevctf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjjbwprn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/guhjcfhou.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gellqfnfn.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grxbxvjsb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkuaonet.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goxspfdvu.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gynaaeddu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtydzbnpk.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqavzwj.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/geogxzdpl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqihafiqv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtdkyccz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnwcmcpy.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpwivvnx.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjnedufx.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gtrafvtbx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzosqsae.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbvlketa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlprggwv.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkkiuowjy.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gteurhfhe.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnyirheu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiazumvl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfcdebqm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxbphecm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfijjlxao.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gohcbquma.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gonklsypl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gltugxfyf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqrauyip.sHtML


<!-- 参考信息 -->