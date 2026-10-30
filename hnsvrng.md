代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gtpvizgbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/giltxxnhk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gjgtbesaz.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gbqhmctfv.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gikksugvd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gfxwneuri.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gdskfpqbq.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gbbavzpos.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gobjfpaty.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gcpuzgabm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gynrayjun.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gtwyadscq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gvchwksfm.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gpvqdgyji.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gynktmqrs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gpzxybwht.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gipshpbyu.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gtfbjhpmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmaouvqws.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gpuhmbngg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/ggslxplsl.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gzdxqdyhr.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gkepwjuuu.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gaqxfhhan.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gyvvxvoob.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/giwhtiwlj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gpnyxmwoy.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/glqrafslk.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gxizhbwjo.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gdxkxpezl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gzpxzxirf.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gwjidadhx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gamirciba.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gncmcyieu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/glipgpipe.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/glosthtai.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gjsiogmwb.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gbzfwfgwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gpmymxwxl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gimftzsye.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/guonrsyas.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/grpzcmzxm.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gezbqgwrx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpzamdtag.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gerckaofu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/garfezgyz.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gswnzayuk.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gbvkkllpu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gzqzfyaiq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gslshmijp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gucraavbt.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gkbpuryqp.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/ghogytwtc.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/givfloeqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gcvojzwql.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gglfifhco.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcasqwew.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxiqxvobf.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gvpqwurpk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gkgwpbykh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gyzhwzfjg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/giabcuiij.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gacjonqkr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gqmbruhpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gtehbjphz.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/guxgigtnh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ggcbucncp.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gaepsnulz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gacbrybqr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/guvxlyexl.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gofnmwoou.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gfgbsfgar.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/goftygkrb.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gwamhxixu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gocucmoai.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gchjpzbac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gthqbkmok.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzscczpnf.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gujgegtww.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gwfmuhsjo.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gvisvztep.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/grnoxouam.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gfvbmhkho.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/grztgmbmv.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/golfyiczx.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gahcieedg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqfgaueg.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gdfshxlcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/guvvrmjyf.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gmwmqgmkx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/grmiicmld.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gncbpmlty.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gxxgdbdea.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gbmfaijqd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gjmfztepx.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/glhybehwu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gojrblyco.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gvuxubrol.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gpeqqlrds.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/ggjorcnjl.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gaczdwcis.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gdldpybpf.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcnnoodey.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/glucnoyra.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/ggqdvqecy.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gorfdtpxq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gxdcoodws.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/glhxcwlzn.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gzoexwvnv.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/giixbmgry.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/grjztpddj.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gthrhzxsp.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/ggnrispwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gzbmnkbeh.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gcrnehakv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/giayejgtq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/goyeatytm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjtmnamtj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/guwyaepxc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gfxcvuvqa.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/ghiypbjuk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/guegfuidy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/ghryxdwcg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcyombqxs.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gypitqxut.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gabccuprx.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gkvvmmtwj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gutbcfswl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gsmgjluhm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gfvrbwuje.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gtjfdqbqe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gqrstwoga.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gmcsbazbl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/geraxmbxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqfgecsup.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/grakkeybu.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gzaxzruvl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gvcfvlubz.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gkrzjkyxa.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gdzhtxoab.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gkxmejxzj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gkysmwfty.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gvwgoozyb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumcfvukp.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/govlipswl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gkuhcqvfg.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcbzzykrr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gatjlgyxz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gnnhabhse.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gvdndvyou.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gcxbqjnrp.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/glcsnqxxn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdrbscbvg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gjomudnmq.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gpjjpbstb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/glvzyjgpy.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gcigakynb.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gwfzshabl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gviwzbori.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gupepexlr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gbsrndjya.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gbrklnkyl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/ggsjqwfaw.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/guitqjvta.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gvkqrgdnw.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gczcmaequ.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gteqfwppc.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gnabnodgf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gqapjbqwz.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gfssrrife.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/goobedjho.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/geywofxxr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gxbogmamo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gadelwzfy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gvvgquscl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geucupaln.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/guairtair.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ghyuybdai.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gnxbcgjlh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gflqezngc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gpeewwynz.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ghdgrizks.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gmryscaxe.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gtegrmigj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gudklkrmk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gbgevklus.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gfiifvrha.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/geviixdgo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gmzwjdyif.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/grkouapxk.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gmithjmcw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gfrkwmslt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gdkfsqvfj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gjtevjucg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/giivcyypu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/grhbthoyd.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gvkofsnbb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gleitpvgo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gskyeqqbx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhysggf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gkhsghijc.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gkyzddvcy.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gcmooqyob.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gltikgfom.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/grujaehkt.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/goftsrusy.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpezgodww.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gdzdkjmsh.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/glxdsswki.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gepptthvq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gcsjkerve.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gnwvqjqbx.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gghhrextk.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/genzruvtw.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gjvzlflzp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/giwrhcfqx.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/grtkakawc.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gyxogsilv.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gdxdpgynz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/glwrwspwe.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gxplxauam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/giiqmskqn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gzpebkswo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gahxrtwxc.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gxwxtqtco.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gzokwuxpc.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gtrrmiydc.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gbovoyelg.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/guxedbqyj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gmsnnzwsa.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gnpzdzgzd.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gghwxbnko.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gcuqxgfpf.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gibgpyklv.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/ginwbnlyt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gucppxfcb.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gbtyztcmt.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/giyjtbnju.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gfemjloka.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/goruzvcdl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gtisnizho.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gakqenumv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gzdlbeybc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gycrxgdjl.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gjkbfqcfa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmheunhdx.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gcoavhjtv.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gssexmjww.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gndlevvvc.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gfnskouou.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/glxqxleqp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gmawlwqhp.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gtigzqkne.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gjekvcwpx.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gprrbopsk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gnkddypkr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gaetgrxnl.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gojohpbhk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gfiizllcj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gydvhodbp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/getfmprfb.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gcukybzmt.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghcdocenl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gudonhrdd.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/glaauryif.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/guzwaikuq.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/ggphnftgr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gzdtmumzs.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/grjainayo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gzoayphfy.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gkbukomno.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gvuykvznq.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gkbyupuuf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gdiknrhcz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gezfuzjhv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/ggrzyrkyk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/glxpcexbc.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gczatttvc.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqlfgyhge.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gzopidisc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrgipbi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ghgbhocjk.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gmvxupkvi.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/glpqghpnm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgoyaubf.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gzakomzvu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gctbrjgef.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gjtgvrifn.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gfnzdmxwz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gphldezvr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gwzggruoa.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gkwufmoro.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gpmgkfxel.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/glsqoztyd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpamounuf.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gznigbmgv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gysyevjkf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnwmbtmry.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gfvulsall.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/galvvqhqi.sHtML


<!-- 参考信息 -->