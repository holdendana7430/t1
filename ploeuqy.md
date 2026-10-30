代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdpzqdv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/griueznos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzjzmnri.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfyyfdqm.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gfabtfucf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gftvhupef.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvycsfkpg.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeciaizc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgiaahw.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gsoynfezr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gicemlujh.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdwwwcxt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjdueazk.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjteoewzp.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/guqyxcufj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnibjzmon.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnouqtcmn.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gvndhuvfm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdcxngvq.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/grykusrbg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcstqlwne.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gefowrrho.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gnwrosawf.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gliuszdwr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzhhismk.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gghaitksd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnmheapng.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkxolujn.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmiwiyov.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gjmngkkpw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gegiwgnfm.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxpcfzgwz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gvhiybhpg.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjcukmi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/goaygbhii.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrcvskne.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnfrinmr.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/ganttymkq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/geeatxpdn.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/ghgcampzj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsjfxpoq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gsguzstnr.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/groyyhziw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjlvxqxt.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/giwmpabqb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glrsmivty.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlsnjjul.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyhvzanj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/grdqfmaji.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhyswnrj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaursyofu.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gfrwohrpx.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gwyeetpor.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrdgeurr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gynqdzpmn.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/guyhpvbuk.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfmdiwhk.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxgfwhzl.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gtmsdovpn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzubemnf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwlpoyxr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsrpmicr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqbhkwwq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeudpqgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjqrijds.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqpveeae.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopmfphas.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gukqosbmn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvokurcl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdqfamve.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfvrllop.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoqsncbf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchysoqh.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gpcewhdzg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gclitgxgg.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gictjfscm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gytnrhqxd.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghqupoouv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghktdkeiu.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gkeswwerw.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gshoezqqp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gurxlogur.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gztabciuj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlgdrvv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyflndlaz.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmcqpusgm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gviuztnuj.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gycffcjlx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/guiwvlrwz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdjyasfs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqkzaldt.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gaasjjgml.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsxhpifu.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gakdlyuwo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gsrokvtuj.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gjdeiqqmy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gekiyuwll.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplohxcyu.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwfoebdd.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gacrvtdzg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gvhmhlgky.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilwlojue.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpepjpqf.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpphoykkp.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gymsnisty.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpttpwsyt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcvendkl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gyihtoqiy.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwmxmiog.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gloslyzds.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzyulyfm.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbftkboar.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjgfiysz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gssxddcsl.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqravlvdo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grtkmxwxy.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gzomjsbuz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gviquniyz.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/ghkrqstcf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpsexyrgq.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/ggyckyenm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glezzajiu.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdapnbbyq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grgcbafby.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gbrfnurqs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsydihfso.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gupdkgltm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gppnsdxqh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhwfdrcu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/ghszaqlhx.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmlxktpha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gihnnnjxb.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/goplolipw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbmrnfyw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghokmsmoe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegausyal.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gzydikuon.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gbazkorsy.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gaixnsqxt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/glygbgwbo.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcepouks.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxijkkwqq.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gwleslqsi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpfpzwma.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqpbvltn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojypqapp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkjsrmlx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavkzqcms.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtpzpfyg.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gujexkvqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/glhrpjuco.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeteufwm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gnmftprbl.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqzbftris.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gloouoklu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmavpopit.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkqkydxn.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gguqnndmv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gmltmndgq.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gogireqnl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtrlgtkzs.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbuttehd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gkcjmnfel.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwhwkdsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxfptewwl.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwalupen.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfhuegja.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gexplaeat.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmuotlkx.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ghglllidd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gtesivhcj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gonlehsdp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhvacbav.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkcuqcfms.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gprxmzkmc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggarxeapm.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewzwjedw.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gjseyjhru.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpggktnl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkoxkzhp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/grkvzuewj.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gqfpbyuey.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gdyknhvav.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrywmfsd.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/geaphgnip.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfxtypg.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gbjktpdwz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ggukdmxab.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkrinlkyh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmiuthk.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghjzfhbhy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guenzuwuw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqmdoyfq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwlewoov.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggdvwuct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grjwytdvs.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmcopii.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnlvbgyk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/grrgcfgvv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/goibvtjhx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwwkuvae.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gznucutqy.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gofsmyidm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gltauikww.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ggcgldjgp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmoobisky.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwvhkdsn.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gprxfqboq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjnmdsvzh.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gutvrrvyq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpxkugh.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffgajoyh.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gzijlqvvg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvaqfljx.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gebzajaum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvximsmam.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gryzucqad.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gogdcoyqg.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlbntazg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxdtriyu.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/godvolrni.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxokhpwz.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gztpygzfc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gksjjwaqf.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gxcvbrbtv.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/ggoagwmyc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwneomqvu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeasmqpm.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gmukyuuju.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvcvhqjt.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghivfizqg.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/geyabqfod.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gofiagqmu.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/grelkddnf.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gywfaobiq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhvlkldd.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyxwrkxx.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcdhaqnyp.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqtvsvjqq.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdixydtrl.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtqlpljv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gccjisxyg.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/glszpmmge.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsevrnmb.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gujswkswi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gducfyuec.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giqlkypqs.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzzjxkw.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gopqjlgco.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlkvqlv.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdslylsu.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gsevcwcgi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoilcyte.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrdkdbtq.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gzvkdcwvc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gonmlxbwp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmsutlay.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbxlhnnq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabrbbfiy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylvlyrda.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwkhtezqe.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrhnyxn.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghahqjpmq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbikcjiey.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnztrywa.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxgwtjuq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/goxmbnncm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjujcbu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzvayqb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxcomwyq.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjhhztspl.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdedbyjrq.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzkzozju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwydifpns.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvwurkvl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/ghgdblrmt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqmpvsmfg.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gftojnivp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtdvehod.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnsnnfsz.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwgktngp.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/grqjeeymr.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyxwzxix.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwigilds.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzxlowce.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddnurslh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbrgnxopi.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqvoewhm.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gyzrbnusv.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwymmoaed.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbzpqeno.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gmryenqvz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/grbshsirv.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gwptwnqaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeihrqws.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqghmaiw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijbbexxp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpaiuviyw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoyfjelb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmuzzekta.sHtML


<!-- 参考信息 -->