代发 wailian999

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/guonbolei.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grrgetowm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/geivhgaak.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjjmsgzva.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyqmahot.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjykoanhq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gssuutvph.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadiekjdw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gduutabzu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcynazitb.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/ghgssvjzk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjisovou.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrixmpq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddkjxkb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoxcnous.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gxrkymmri.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwuhbrkvx.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gyrhtpqcj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvxziumon.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnvkzqywv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzptgnsf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnyudoix.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwbhdgzi.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnxyrauyw.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gzibxceue.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjzbptxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblqjayhw.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxljvwoud.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gnlmbjotc.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/guxddlgcj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gknuhfqqf.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdheypblg.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/glfcuxllu.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnjlfhzk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfoqzcj.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gbkvbmlsf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmekltlwj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gkycfkjrj.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgoulqul.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvqekrh.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/giylyujoc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfjhelhk.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfpdorfrl.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gwycwgdui.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvlihlxvy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrutqzgj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcajaugdj.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gajillpnw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazjnylum.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwpzqudt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywhsnpr.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvqoeiwuc.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdhjdnhc.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/geohixyjp.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gdqblphxq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncckzxzn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/grxbtcwvb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyltjspq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkoiczpu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdpgfkjv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlaiwfdm.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gbnhdbnzm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/grrazfwgc.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwjuolfqq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gwmoggpmw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gegvgszru.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehjsunxf.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvjiexc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gntckwdgy.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwijebvpa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphpnvgqf.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gujgpzpgw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpdzmigy.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gejxkfcje.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmkxpcs.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gfuwetmls.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/giigyurgc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxhyqtykk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gyyfbakkr.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/giarhqnuz.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/grcvyaeyd.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gawshvnxo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvzyfoy.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwinwaruz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gmbpgujfd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefhqavsx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpdxvtta.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gvddfqszo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxxwkyzc.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/glcpgbaiz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvfhtccu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gmugkbaji.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gysyeyxhc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykochfyk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpinyrrmu.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gaixzyvgi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhzmnjcj.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghxicuuds.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyfebjf.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfuqkqpq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunqgrlrn.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzdrbjvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmvfbste.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gpcxxutqx.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giifuhbdx.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gyagckjou.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudjzpyyx.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glxyaicsn.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnjljffh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grtxsxwyc.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxodeyckk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjttnpdrh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gokoyhurq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnttjnmoa.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gzoebjcwk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grvuczckm.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gozzaaktv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gecqblgiz.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvawtjzpd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/giovjaqlh.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/genbovahs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gemqeduaf.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspkdfyhw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gleiscfwv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzepavjyi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gfnnkspvx.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggrhaubos.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsflaucjw.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvkwmogbb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gibqnzlcm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiclaxwl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gjbyqseld.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtooxlkad.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gbbbfcomb.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gfpmkrbrw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrpsjlic.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gockwcoon.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqafzjlt.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gwadkjxqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkxiscjf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbaejbll.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gghxwnfpn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gabbffzvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxluneke.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthmvznlc.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtnzwcbtj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gedhzxbje.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrssnnov.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuyxcpev.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyzekmvwt.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkzziaga.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlxkrnev.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gluookhro.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gwooxedcn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/geqrlwoky.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gyuhqfuts.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpqodiit.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gsytuqjcc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggutcvwik.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmebaeypc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gplhmkwrs.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqyzcpw.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnpdpnkm.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gkwpmjxqt.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/golghdhcv.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gushdsecg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkajuwnwk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsezxrxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatonmbsj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrhgzlcj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gazvxqksy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvydozaj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcnmlomv.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkwspamw.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmxyjnznq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ggiuomoxp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/ghdvgrulx.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjfelmth.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/grlqorcus.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gwwampftf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grteuqbkc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gugietdty.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gvflqrxuw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqyrvgpu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqsysubm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbdjeytre.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gctjrsbig.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gksmnzeif.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrgdsavl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gosvhvxoh.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/goaddghfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/geqkcbbfg.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/ghhmwnpbr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebvjooj.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/ghfzioipl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsvgvvym.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymiewdjb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfklhlxvw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gszyeauko.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmrgohlv.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gyshdmwrj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grifgrjqf.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvnhdio.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gnhqvalgm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyucmvlan.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqalvzovn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfomkvlr.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gvlsbbkbm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/glapjcoid.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzawuxba.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/grpsvndyp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/ginnjsnlp.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/glqiqmrwf.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gurzolbmw.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcohnzee.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmkcxkis.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbmrmfkwx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gbgsndibl.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gocnphbwr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldibbyqg.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/ggmsamgai.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthhzeeey.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gfunrdrts.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxpeklcf.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmnzjpbe.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwveuyvra.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgaxpvku.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/guzhpcnth.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/guwsyovdg.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgmlxgfw.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gcasulzxu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxscjqtke.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcbzfxtnb.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlhbpueu.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzjyuseoy.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/grnxvqfbv.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gtixdjcdh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbyvpdki.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/glyntfyav.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkrxflct.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/glgcjpjoc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/goqrepimz.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnhcjzhy.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjrrekon.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/geykgyanm.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gcgssofxu.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlbghkyi.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gybcwagds.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gobpsqkep.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/glswoksmy.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gnqxhmybj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gamnfnvnc.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gllmqbtvv.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwibgsezq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyanbvyp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gbvxbrjxl.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsexeppso.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqldbydm.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gghptgbbq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwrqrtwvl.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtarmtqr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giojaibpi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glvpigntm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gopdvvoru.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gninzhqxf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjhdraih.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gucaxykfh.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjeayggl.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkwzkvbcj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzrfpnofc.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golddlonw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxouwmnd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzzwzgyon.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfbafmwq.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeyqktjb.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcpgxwyis.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grwnyvigy.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/geibgwlfe.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gawdcopbx.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/goqusytog.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbndfbow.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtjnkvjjd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjioeeavc.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/grwmbgsao.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gmnvoalxu.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gywbzppfc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiolsblj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnoqmnmv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsjubayh.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxqnwssz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbtwjullh.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gcjjfsozh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzwboorw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnkskoahj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggwcjbowq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghtcuioxy.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtgmtvlo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gijfyujxp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxecfpuc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyoigdcm.sHtML


<!-- 参考信息 -->