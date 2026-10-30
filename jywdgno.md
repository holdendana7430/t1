代发 wailian999

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtgocwcr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjigizt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeydpzrp.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdkrzncmy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gngyhvkse.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbdfptxy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/grraqilvv.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gupvirpam.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmrbkvlv.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdfymjfuz.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gzuvltrvm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gghzhkguv.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gitqmzzyk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecqrdjnz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfnjftsjb.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdcygjdc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/ghvmsiayw.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywljtra.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkjxqynh.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmanvdyjk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gvapbhaot.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/ghsktsoae.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxisejhk.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmoyfvpf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlkvhkfk.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdtrnyzi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmlsponug.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqwcrbngz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzcsmgnx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwonjoyeb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gnossdayn.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gfrplhtic.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gzktpgmne.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gsdfigjsq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjrudua.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokijqfd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvwwfxpu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/glzcdqrqm.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gncxxamom.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbndxadsa.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gccxiituv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/givcjhajo.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gauytgkgi.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gftybkvdg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjflrdguo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjkefbxp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjqhvutr.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gylzuszgb.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/givekseyz.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gotclwrgd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdudeggvy.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gngkroqcy.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvghqck.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtevuiubr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkgbtfly.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gixscpyjj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gaxmjcasn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gmittizwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvtxydod.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioanfyyb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gbetjglfg.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gijymgome.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvxccpua.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpkbhfurs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gbmnxsdth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfwhrxrg.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/goudxyfbn.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/getfsqwrs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbtxmcsa.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gvtwvwefl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gvswfezkl.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuhhqgwq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gfqyxugtw.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkrohgmrv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glezrgnul.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/glyzaqted.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkslujapy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfsdjotgu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/grcqfafjj.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggwufujft.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevbpvsag.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghdpqvolk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gzdygldnv.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnedfjksv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwepykco.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoyyrbkc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtszsmuqo.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/givborvrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmobefwcg.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gmqblwmtu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/galibxdod.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtesphtu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gppjsxoee.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvtbxaeh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzphvihn.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiueqhkj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghabdstaw.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/giqxqsyso.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gowokbkas.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyzvmymm.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuxzptbw.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvngjnrih.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/grctrrdeq.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gbnigfmns.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxjikfuam.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gibxnoxxd.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gfbptxinp.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gddplqwth.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gjulgwcld.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxchumu.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtqapwmyy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjprinc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gggcvejwm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsdlbpamx.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/glnpdgsoe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfccywulu.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gizueiign.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqcwtptp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgiixqvy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthjkujsj.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gynbatvgi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvzcmfds.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthzourik.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glmfawylm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkecvvbzg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdutwoayu.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhouked.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/glmttltdx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glyrndqac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxhrsfg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gimndjljg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/geunxjget.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgdalbuh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gvknapqix.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyapixfw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcbtuqau.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gllfzfudc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gphtgzrpn.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gpadxngbr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/geqaevqtx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxoiemji.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gstlkculs.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grenruavv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/grfmbnuhp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/geedkxsow.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpjhauiok.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyovyrbik.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/ghvsptbce.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccydxhi.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ginyxxneu.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjhaumlj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrknyuds.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggritlagx.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gronpzaaf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuxutgdy.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/ggbodrlzw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpbvaubhh.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpmkfld.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gvcolpjfh.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpomhzkj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyygrqbqk.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqhbqkes.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnqvanrt.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdwzjdnac.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbabdcaz.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxykrxoz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcdjyrji.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gvmetaxyr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucihgxpd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghqwbxado.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gmcyufuxm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzsyoonv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkjmaucwi.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuaqwmue.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gadqlwyht.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuthysdw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvwabtkw.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrpykzwy.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ghlhayxsk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqarwoyu.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbdqrisl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmffsbpfe.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gqrsdwuxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgyungje.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gohpcyzrn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqcznxkz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gburbzdow.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwwpclgb.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwylmtqxu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdublcmb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbciqbsg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhkbxdks.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtspmvbb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnjdazii.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdullcci.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuxncbgx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuizvsov.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gghtenabe.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmlsbkkho.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtznpikjv.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkmavsgr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gqcdapllj.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmmcxogf.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhadpjrt.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdknkeipj.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grbletenv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gaexrvouf.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gxuxcbbog.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/grtmokjyc.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/giunbfycw.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynelzdk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/ghzrahfqx.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gausrgopl.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjjmrvp.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzafljqma.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmsypjtgc.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwwsznkjb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/grenoioek.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gozshsjpm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gejtitkcp.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gmujuveae.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsvxgxgf.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuwrzbqr.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gxeeplzhy.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbnhakyr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/giyqsnkcw.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhfztvsv.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqnjrsam.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/glsxyhcqa.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gucfvhwjm.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/ggjoyxasb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gauzfxmls.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtstzllyp.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggcplmlsd.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzcfolsot.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsrspths.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ggnteeciv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gvwszuzkd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjpyksur.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqnpupy.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkbbhzya.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gucxhpygh.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gutmendmt.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxsjksq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhkukfyy.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gycnqermv.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdxzzabij.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gqkzwhanp.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gathbysbm.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gnuazlapb.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/glutneawb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gdfygkkrr.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gajclcbvc.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/geklbnflu.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnlcikzrk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqskgtqwk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/glhqksnmh.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnorfitjw.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghthzxczm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnjwjygs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gaidfzoyn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmprxxht.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gddekhicr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcrlckiq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/goltvzsal.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/guzvwkxvb.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpikdoh.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/glotpnugr.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gegqaitav.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegnoxusj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guotpzcyp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/glgddbwem.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggpbdtdcq.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaytematg.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goizkrxas.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvfqqdsph.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeedlten.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/glnflchuv.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gngsifbes.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxanphca.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwukrulw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomvkzrjf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gofnarvcs.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzwywuid.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/glzbidxbf.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grloirqbf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuyhfebz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcogdbyp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gujvsyahq.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpknybtdx.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ginqazvit.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfledxu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfwrbst.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlhlsugb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnzjsaequ.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiyewhhk.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gbofufbgs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiekdtpm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfjqnym.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gihbonlry.sHtML


<!-- 参考信息 -->