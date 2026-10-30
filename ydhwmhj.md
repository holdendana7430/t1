代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnoubwp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gabsaxlvg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbikwmtaq.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gprlqwgev.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfyctrdm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaugygry.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gfygjjjzr.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gitmspmmm.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gezqvaugx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmidecu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/graijisot.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfcjhsmtf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/ghqqglxbq.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaavcoli.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gxxfsykzc.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupjocizg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaaazrzv.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpyzouvg.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlwcxjjl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gmkfxfabk.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqdunide.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjzwfuwj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtldgncho.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gprxyshrz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gubexvezi.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gojcgqbjb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gegvjqjuy.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqwkljsjp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdmrazho.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gpsbztarq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxrylkyn.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/glvakhfle.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gopdyvdmi.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gefpxfhzw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnnfzciw.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlrshuoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gsdvheegt.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gltdemlcp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoavseon.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfzhzkvs.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/ggawnjohu.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgcwwaaz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvswudhnz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmoxbsgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatgguojz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuocrfkj.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrmihbof.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzpznwaer.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwzvxjccs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gckxlkjuw.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grcebmwwc.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgxhninj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glolhcgth.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggyekpvri.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gnxazozwm.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkwzzqj.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqrkutyt.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqzuqdhco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ggkcxiout.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gpifrawkt.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnetnzmpl.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gacsliqnb.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gigamdstu.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzpzywomh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjwharbw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdxkmhiq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gbtiwjiax.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/glqnxepzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcuvxcs.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gphocmqah.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gumhnetjw.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnonmblc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnggjfbo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpheiyyk.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbkolcotj.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdbgubrj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gqwvcljhv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrdmmctq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/ghpmabquw.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gxqefgvij.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbajymyor.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkynoujz.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqljzdgfj.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gnvhczdck.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwntxxjok.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbwpkrrz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gsaaumriq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvvbxtnw.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjciacjhd.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwctbyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grktslqvr.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjogjtqx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrklyvei.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiuevdql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/grbnohhsu.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdlvmrqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkmrazl.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglbxisch.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxpjfxlo.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmdkiktpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grczanjyn.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gbizhsuvc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslzjlwlq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gstrospin.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/getaowdcy.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkafeuens.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmocwhigt.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcjbmaxu.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwulfbry.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbupqvxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gchilgddi.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gnfeobwtu.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwenjmum.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjdrbslk.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gjjdelcpx.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guayhzrmc.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqljyjkdv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/getdonpds.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gulbmxarv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gshneafdu.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzakovij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gesedwlaf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtxfwyvu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsljfkws.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gchaqilvw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkgankoe.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpgnfiij.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqtdmhrc.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnqljyje.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkbbfyfw.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmjfflks.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdheyxorl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfphicplb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmdmfkg.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grdtgwtpe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdmtjjos.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyukvrorl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxkwwvvf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpunuvgr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptjeueij.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeqpsagl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/grfocjvus.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glniyujiq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gncyautnx.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/ggmzdprlm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtjrflt.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gsiqqvopz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttmweqhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcwbdwprd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvfsbimef.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfkfujrr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnpxfzj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grsvkgmzy.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbixrlyvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gglbomaot.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnvltulk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspfkbjff.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcnraxxms.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gicimxwce.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtagquad.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqyellykq.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/grcakszpc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfcugbaob.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxphqdo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcjjsuks.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gioszcjlu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/guiplqyig.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gzbtsiaig.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbctqgbkh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfezgoxa.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfixhakej.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gvinqxnwp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtlovruf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsxqaqzv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gozftauqo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gaynhwyii.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwerawcqd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geztalwmc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/grzrmqsoq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmdobljpb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuiuxnje.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakntlpod.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gttdjdbnu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/glgowzhbk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcsqayct.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gfkjgwdow.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwlbuiqf.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gtrjhohnu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggehcdlpm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gazkgtdup.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gghlclmtm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfwvrtul.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcskgiro.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpjmumxd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gemyzzwtm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymxnaqld.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guhyuwrnn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/guzqifgob.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqdgdwlk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxyyinrhx.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/grprhgtnz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftkkanqy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gjbdiumad.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmgsllkk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gdduzddjj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvkvrjpx.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgcudige.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqchxqqiu.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gyetkkrun.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrvpgosy.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/geiiazton.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gaafswbry.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwsnpsgp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnqafksc.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grhkdfipy.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkhfofge.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gmnekcvmx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzfuwgvh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gracsbflo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrpbyntz.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grvwsxozq.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfoumcha.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gkcfxejpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gavqsvjra.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggobvibdq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gcehmeisa.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gipykgkxm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gugiueofm.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gamifaiva.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuytichm.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gzfvylste.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gyegjrxqb.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gnxcleoaw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqxmdssx.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbmkocpe.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/glxwvpsko.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gebtdiavk.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmihpebeb.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gvkoiqixq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwgsklzo.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhcjorm.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/grdcuccgt.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfvgjzx.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcrlwayq.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gfopfbyke.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gvyumgyxi.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gduridtat.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gfkjahwvx.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcfnzxbu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcacsyazf.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyesvefsq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckyxhhax.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzxbdeyf.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/grbbmcpsu.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwgjhembb.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmjvwnx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprqttoxb.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/grhhjzofk.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkcbmqhf.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpkfqlko.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guzqbndqz.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoxpftoa.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/goxyhmbup.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifeqyxob.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnphtjob.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoimhvew.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/geoalebxe.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghratqpgx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyvrzhxw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvjxsqxjh.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzukhnmv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwpflsfca.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gnmdggsjb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gacnieohc.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvupdmoro.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitbofffy.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkoxkjuxl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxdyypzm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvbzkiuzt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gqpgvumfi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkislpsnw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkmahjmw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjbpweddu.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqdxnqetf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/getfexksr.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gurnaznms.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyduvzcw.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdycghhc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebojacn.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbngolocn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwwoqecbk.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfjvcbkn.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ghtdfyzjo.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhyexuhh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghouxnubw.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gkhkhrmuf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmrywykt.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwakoquiz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudkyjptm.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnydcwkgh.sHtML


<!-- 参考信息 -->