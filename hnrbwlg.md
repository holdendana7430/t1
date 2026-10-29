代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gkjulqvzb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdkvxqgkg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gyjjzbsrk.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gkbrenikc.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gqheojluj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gbxvghorv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gfmggseru.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gwarjcgym.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/ghnyxpoyg.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/geujnepuz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gxxxymdsu.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gmxieshwd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gxmchbtfh.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gvmhtapfs.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gcxsrmegg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/giltqhwzw.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/grfbxfjhy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gnjnxzpsb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gyktaaruf.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gyrgcvvpb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gwfibmzym.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gzpzsgrkp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gfqaqklcz.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gprwitakw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/ggpiuetwg.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gjvbngrra.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gftnueuva.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gkxnezexi.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gwsltwnjn.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/guhlyvomj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gfwrpulti.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gguhiipht.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gncoezpar.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gaoimdkdv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gxfrrojac.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gqmfxgbxm.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gxipmqrnb.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gnnylrkww.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gqrhgihzr.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gakqcmpfl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gxbflpakn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gqemtbguh.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gmbkvvphd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtchikuky.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/grwwylcpd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqvgqnjzt.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/guensnnxd.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gjdymtzgg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/grugfwtgk.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gkavjuejw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gdbtsdvca.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gpowtbpmf.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gflafpcgj.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gopswqjmp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gjlygxfsu.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gcjwsgggb.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/givtdrqda.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gcjdhxfak.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gdzffvgxm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gmzkmxqek.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/goxhuipud.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/ghoqukkte.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/grrkzzmnv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gcwonzzdl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gpppuccrj.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/guuvyniip.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/ghpjaekxh.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gekckwowy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/grolrscio.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/ggoddhxey.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gadbzzwel.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gjsctfyil.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gubpzihjb.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gfelxylma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gozmqksmk.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gcmcyeqfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/goxbebjtf.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/grdwbmqwq.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gzxulikxo.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gxcnsyxyn.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/goikhwnno.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gycblmnhx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gfcpvjczd.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/grnzpgmgo.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gqpdykvnh.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gkkfdvomz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gedfdlamd.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gwypnwihw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggaxqkukx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/glawbmtmi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/grgpkhtrg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/ggaurxctp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gbbydtspi.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grrjxbrly.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/glzohwusc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gyznhjyhp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gmsnfjtkm.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gsrlilugc.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gpwrsxsjc.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/grezrhqrh.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gdlkdqgof.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gflgxfbig.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gyssmhvvq.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gprsypoxc.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gdkcirevt.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gzunbchig.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gyuzxuiam.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/grzvhmzza.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gzdyawcfs.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gjcwdvjvn.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gxlcihexl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfwsbvxwp.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gxtkxrmvj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gjvrwvjwo.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gghqajvbp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gjjeyqezh.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gavhcaeyc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/ghnhgtujc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gufgkcuyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gttcykqmi.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gnzslnqca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gpbksmnbp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gwfsfmbcq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxyfxkugo.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gacvvomsc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gznvvwbew.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gqhekvdpt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/griyfaqyx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gwjguehpq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gfuuadqwy.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gavswlcew.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/ggsfoejlm.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gqwzomllt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gbvtjmpfb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gdnigislb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gmnblwijp.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gaxdzzmwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ginbubgxh.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/ggfridccy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gvdmmyvxc.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gaeppdaiv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gdsdmglvt.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gndevfjwx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gdpseginb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gruaoznud.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gqqfzobnw.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtzwzlnjq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gktwiauni.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gkxeffiof.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gqnpxlrud.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/glkdddqrm.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gjietpfnp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggslfavxg.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/grzubmaqu.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gbtklofan.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gfjwsakze.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/grsyhdfeq.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gywagciad.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/ggpdjaosq.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/geqqkpuvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gyhnoswqx.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gzzbenzef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/geuqkvvga.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gwervfwcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gsijzrtop.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gagnegojk.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/grtthdahx.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gpkfctpqr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gniucfosh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/guauwnhaw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gsmftywft.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/glwnpexyt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gsxnhggvu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grmkynqnm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gaywjuons.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljhvwqwd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfnnvgxju.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gkliorhlp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gldjresag.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/ghtaqnwkr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gmflhufmh.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gxwabhyxk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gxwclilrd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gnmaxhjlr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gzfjhniec.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gjxhcfdeg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gxahypedk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gvxnndhbh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gsiwyzqei.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gkiprzujh.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gzzrscved.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gxesgqspv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gyqdksjwj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gjewcjxfk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gjfoqfsbp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gmlzxdkfy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gcazvxznp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gozbxcins.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/glmiubjml.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfcwykzvl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gdrtozmpk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/ghcdhgxfw.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gnosdezcw.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdsvxutcs.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gplwiunsx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkpzmnmf.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzivckcor.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gvmoxggaw.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gtcaxdduc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gbevljdsv.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gloaaoopv.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gyyhdceul.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwtnjptax.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ggjdnsftj.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/ghhgjbntj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gswfphkex.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gkcojnjmw.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gfdvcxazy.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/guhsmddyw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gcgmmbjry.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gpkwkgcyf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqqvwkuii.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gyniloneo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gzoiwhmmk.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gqwfdtvpo.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gqgudwhjo.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gnnlmyjku.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gugjwdddn.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gjnxydvjw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gymarzdwf.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gvyqwmrby.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gfmoljtew.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gerqlyyjk.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gfpytuicc.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/ghqtdqxmy.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gocrfhvkr.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gpzmzxbju.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gjgibwbiv.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gisldembf.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gvfeimhbh.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gqdjsdapv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gqykcxtur.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/grpnyxpzw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gqoqttidu.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gmktbebnr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/ghotwdraj.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gfxecorxw.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gkypjdtbe.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gocdchpph.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gkbuguvrl.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/ghpozpkgr.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/grqufihyd.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gfrpgjdnk.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/grvgotsvt.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gglstzapo.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gxwgohwad.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/glmdfzrdy.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gjapciluz.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gnswruqkk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/golelsdgx.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gleafmxgo.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gcjiuxprz.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gjyztpeay.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/geaiellzd.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gkuclqtse.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gludkbwvy.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gmllemuoh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gyjuughle.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gcfbbnymh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gwzqpzdtm.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gfvtkssis.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gxdjmwzks.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcosfcdmy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gmgsvbuvo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glwzfhymu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/guaghohgg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gconbtvkw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtxnsvpdb.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtmcapexo.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gcyefuwhc.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/ggrviqqeh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gubsixhir.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ganrjbeiw.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gwqxirodn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gsuhaswoo.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gckpicrwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gxikxmqvk.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gabrceqff.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gmmaygxqd.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gjxdoxbfa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gzreevfmf.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gaehmvnfl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gdhsvdoux.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gbfwjuypp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gvsictbhh.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gnwvemfft.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gxweenkij.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwosvubes.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gonerbfez.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkznrwmao.sHtML


<!-- 参考信息 -->