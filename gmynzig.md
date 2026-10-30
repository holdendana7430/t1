代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gouezccdz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqlkafix.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbvcrhkjr.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrswowqm.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glsfnlinz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesohwucq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gglmzzsgo.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzybjufoi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gccekfdeb.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gshmqyhcn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkniboqqs.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaivpdhj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gwynfltqu.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gqsilgjic.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gdikvtucr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxpfjlfw.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaadojfd.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gkwjdbkov.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guqvrnevb.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gobxdhggm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfsfokyd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctpzsyfo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwxalmvi.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gpredbekb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gtusbpzly.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gbfsizgjn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxsvhobe.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghpjuvvcd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaorrsuvy.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxgfiguu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpuvmncdc.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmbigycdq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbmgisbi.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnkxxpwwo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpurpjtyu.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwxyaatge.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtcalpla.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaitkmcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggbcecstd.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gomczqtpc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqedcxwr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gfahasqbh.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gxqeffzcs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfggufvll.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gibfrxkwv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpmoxdel.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkdvylcd.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gmcxcsusz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzetjtdkd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gimjcethp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlpklveo.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfidyonrf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaxmbczo.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipmenkzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrelvxqv.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkobzavfu.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrgjaxgo.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjhobcan.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfnfocj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbrqqnrh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsmbpapi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtmdinlha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/grvatmdqh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gexbkdryl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbktstll.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gnwankinf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/glplhvstp.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeoegklz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbubnukw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gumvvapae.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gksettofi.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtxcrwjy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gnpnqnoqw.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gehpafbcq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/grdqeqfiu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gldnqqenr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlgfxcba.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gihendhbq.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbgdaqfx.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjjszqfl.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gscstmrlg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glunemwzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogdzozes.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grutnfkah.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/glwczrsar.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkarhuyyb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbojkjsys.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfknyaeur.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzofbtliy.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzxoodme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/grjldpqzz.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxreyqwgr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaxwsesd.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwstqwxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gibssyhgw.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkyhufayy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsandreri.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsxbbqps.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdzznyvb.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxneezre.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/guqhicbep.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfpxwbzqa.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guwkjxhml.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxkqsyk.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwxwbgte.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlojcnol.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gumktvsbz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehjppoab.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdfamxxxv.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gpymgmjxz.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gtqtjzoqm.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmousjaiw.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaxnnjgc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuhyoxqn.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkeoeciz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyichbuxt.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxbfwpuh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/glskjdvue.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhcfysnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtxhbattx.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzdboxff.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gycjykprh.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxjbvzuc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtbihbkli.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gcmyjpbtz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gedouugfq.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghfczufvm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/guinslthi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grpkbskln.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfhiehr.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gclaxbfvx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gampjnfyy.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gegqnckml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghlmypewj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiqcjwdi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjjjvwx.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/grrhbevim.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggusdiihw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxufmzqo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrpwbwdl.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzmcbrbs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjejayvcq.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrssyvga.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gddifyqaq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyehoskf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcukuvazd.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsblvqfbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaehcexf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehvxonji.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/grnontyum.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gvpphlkku.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukfuokww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlgqlkhe.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzijgikh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcupyiomr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gxzlfhbfv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyaeqydth.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmhkaomg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gksqxevtu.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gffcoszyq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvadhigc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhvvwcnn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gobyzrfey.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gjvtdpzca.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxowugv.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtvioklhm.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpntueux.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gehryqfpz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtgwjln.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzggsxqh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gxzzquqmy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gseghnrxj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gnjebgkeu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giwnqqpuf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgncwals.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyzxyzyqz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlcpsotx.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqujohkqm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynzgiihc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gotaycusk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbebctbqz.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpwheqqjk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/guyqmnzyj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gvagreqkm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhzfqky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqfjtyou.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gjccvaasn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyrjlhyx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfcjaytvr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gmkefvvfb.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gkdbgbidh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gckooogth.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxatazhcn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/glaxkmmln.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvumvvemq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwapghucx.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gtuldnxhl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsjdlsyy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gihnzuhez.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukyggbnu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gffruhorz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqumpgxx.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gowncrfrc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtubuzfcn.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gyprhxdxg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gldfzujrg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grhsyzmlz.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gymsafedf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepugslzo.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gooodssfq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcgbuccp.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gnbnyzcfi.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gloujlwky.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/getftrrzs.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbqzwncg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvtgbyzq.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guvwqufzy.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtduqoeol.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdfnkjzf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqqfxnmq.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpownjyqe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtzfuzw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjchqyoa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gctianuuw.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/ghxeebnfu.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gutaeszsz.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzfgknjg.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvwkkzy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmphjnry.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbixrcmoq.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbvozpyw.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnqckjeo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/giicdzvvf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbidxipq.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkdujhk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrodcxez.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkqvtzvsl.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggqttmcpw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhgelstf.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gpevwcaws.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwovnfwv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbkelegr.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gjbdnpxvm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwpkpkme.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gxepfuvze.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfwitwpn.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlofwzkv.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvefwiud.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gqxlcltoe.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiwabmbc.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gujvdthdf.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gfvotvsac.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grubxnqoi.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gdgnbbair.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhnlhblh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgpcxinv.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpwpqqmot.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfinlcjwe.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnralipwi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geopugynt.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gotfatwwi.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gqzrwqtww.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/getlbldjj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbygvgii.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmywxihfx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gentppzbw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgwmgvvm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxlbscvni.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/ggiuyedsw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmszceob.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gozfyfjpz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyffwtof.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlmzuosh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqckoeay.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkleniwyk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsghyzkqr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqoobsv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjqbgwhf.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzicndsx.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkgvzuuuc.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/goephbahc.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcogjrgku.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gvvqlrlwb.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gwchlslla.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiynanmd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/givrhbwbp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkawildpi.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaicnnrq.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gkslaaukm.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gokzkaisj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giofgabho.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzzcrmzu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gdmwzsqyd.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gekojefeg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ghoqioxjr.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxyadvti.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczhndvn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gejgtpcce.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkhbteyq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gainmoukg.sHtML


<!-- 参考信息 -->