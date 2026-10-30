代发 wailian999

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gubmvwkdg.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbrxduzal.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/glorcoawj.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gyvpfqzkx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnmonixp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gvutzgzhu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmzajcnc.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbdaoorl.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gawdskvgh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghuyjqxca.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyxtzoya.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gzvqjfpxd.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxrjtdnm.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpdinqqa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeuojfmm.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfskovjci.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdioalpq.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/giytcfhel.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gugfiolub.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbigvlhua.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gurfcqonk.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/geblvxiqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaqqjlyc.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gfujeingb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/giakmhauq.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmculqxmx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcvnrnyr.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfykpdtai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsgiovyq.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gevicmgjw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhkdjiz.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgfzclwd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaqibihv.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbmvhrlw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnuufpbe.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsweafykj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbqzufe.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggsorpmeu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gywepsbld.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/guwggruge.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjlheyvdh.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnxqzjyy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhevrsmg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gaygdihxr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopexjdju.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gymwxwjho.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gheuinqya.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzqmjrhh.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gizqlcwog.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfrqffxd.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfzbzmwmt.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfjfnnbda.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxlhmomp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqkvkths.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbknyralc.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoimrlwx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ghizizcme.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdprfzmkj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfokfghqd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfusazjl.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrsdelkd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyjsxazg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/goejrvwyp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/guahmlacr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gxnxqiwov.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtghyiwpa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyufzgya.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ghyuosunq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuvydvnq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gepnunpnf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtroozwws.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnodypmfp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gqzpcxflj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gntneflln.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgpmmqwm.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbmreyqix.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gienrpxkn.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gswelikbg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzorzrs.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpupjynj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gentzdybm.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdxosyky.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauayexbk.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gxkqhrbrn.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsuhdacd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjpnswklt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaogjcwy.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqqqibvzm.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gpumpvnzd.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gujpyevwf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gltqmdynl.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gkdleraiy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/glyaaolye.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxldbrn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtqlqafi.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswkrwzq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gdywohkuz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ggvrrqjyx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjjrhvh.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gbwoiimbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsfqwakr.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzaefslp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwfbpact.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gtacwqmat.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gmsslkfbt.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsbzzicte.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grdsbeqko.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdbyqezq.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gobjvfeqr.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzxgnaptp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gilezfbdg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjncysxj.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxszgydk.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gjclwmjze.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gryjzzpww.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxsnhhhw.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwfglmygo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpkqbou.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfjeiumss.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gzkpoxeud.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/grlgfxizn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gcyjwzpal.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gxlrxcczl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/goywheabl.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gzkemmpgn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gonnonzrs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqmzlvka.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gljkjiodt.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gvwksutde.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/guhcqhjln.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaenrnvat.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxkpjgdd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gripmoqnv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiaipmrh.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gyubqdcys.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupshkkyg.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdpvgxlkh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbjgoexc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykjioary.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gvkinkggc.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gvykalmzi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gltyyqwaj.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gtbzeycrv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhufzynh.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gperdamke.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwdcmco.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldgnyolx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtbguxiy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggdrqabct.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gahzuwfdw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmarrdbmn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwjtxaur.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gygmzvpde.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gibdiidwx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gjupgywut.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvvepzil.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnrhzcad.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwnaiirba.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gaglinhcw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/ghvlsyyhq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgbvdgdo.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwfwppih.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gdwifoktb.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gaytnngvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxcmwemg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpovlwhnm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gusuedvsk.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbjlybam.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbcdshhlb.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gvwhxjtil.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gisjrefrp.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gohisdguv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkipkafcm.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbrqetba.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiwyucgk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvebbnkxw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gqonswoiy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gswaixart.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/giduqppcq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/girircuhp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxolbnfn.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnrkkkxb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbslmzigc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gesocoukb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeqvdwec.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpodrjfhd.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/giuatsajz.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/grqhblrwv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngckquuj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxccsxodn.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/givizjclx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gznwlwatf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxcbtjge.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcomgfthl.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtirqhsax.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdelayakb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyvgtlec.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnsodnyj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaflmpkd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gppxfrpif.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/grybrppqz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gidsgzkzh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gbwsseres.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsriddix.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gggwtwvoa.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpxhieggr.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtwytwole.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxkcnkai.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gpakhdobd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmpugphxf.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzythknoy.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtmoytobo.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gfrzqvjhu.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqzhelqb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhedfvtn.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhqkdyve.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxvlaunq.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxowywddr.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/geeflicmv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gsklxfmid.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/glnzxrxzv.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwvopavn.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfipgliq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcabnjyfw.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gztdwtxjb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/guraslgsp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbneezdt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbmkqzzbl.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gzgakrzgu.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaqunapj.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfphkuqc.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gfdgrlxvw.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdlxxuwlq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfsebaok.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysqpzyqp.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkbtxayt.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gyahglnbr.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcdudwam.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gpepjwlyp.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtncota.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkjvbjpqt.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfznjzedr.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaynnokpz.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/grykofxda.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvygxscx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gukdphymv.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmnqvcyo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeviqpbk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqxhcbbp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqejruvgm.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvutueroc.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/giekkaidd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gibdxzjpf.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzxfyfdp.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhejklvq.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/grpozjpqc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsgqsyhz.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gekulkxcp.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/grdsrfkwr.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsamulg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrehcnri.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxewqcqhd.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxrjtdni.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/geaeodxlq.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gnfozovzr.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvjsmrbt.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzhmllos.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptfwozvp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxpahbmh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqguoaim.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/grwfrpwnw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqocepfm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gypfkllks.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtkaxqop.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gapufkccw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/giecjbgbv.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpomrtvjx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsudbeld.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlglpwqs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyphwapm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gznbqlimf.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwnecen.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/geceohbqf.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxctwuooj.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grnuwsbup.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gjjuwgqqt.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gbpoazftu.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrxvqejr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddpcuvuv.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/geqhvlwdg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplijnetn.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftkbrulx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gydnalyou.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsiaohcx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbdfvxmu.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gigzbhjei.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gsykwuhkl.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grqwldohf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjqahatm.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gqyturwwx.sHtML


<!-- 参考信息 -->