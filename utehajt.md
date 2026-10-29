代发 wailian999

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gownemwzy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gpqgikwfn.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gsjquizuk.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gupccobat.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/ggzbtncja.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gptclctqj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gcrksvmzc.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gbwlhoupp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gfeqicjbg.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gnmatvisl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gsrolgfwy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/giqomvkcg.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gpylzopks.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/glvrsqwdi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gbokjgaxh.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gnblnfdxw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gwblksomz.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gjrogjuov.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/goxwniwgh.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gkaljwpeb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/ghpbxqxzk.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gaswvyhbb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/guufgsjhu.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gquldimjw.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gkkkihlix.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gegrqpmaa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gwatmhagn.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/guworlwet.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gjplxpckq.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gvfgpygqi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gaqfndovh.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/giraurpqx.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gfyxenypj.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gdujbiwaw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvlufmevk.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gdiedjxiq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gokdmxoaa.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/givkxvaqx.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/ghjkrzgke.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gybuuofdo.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/ghtuqtrim.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gimhrymjb.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkxizbvsv.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gzirkkkbp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gzrqhspec.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqvwtbn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gxhjlnxmj.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gpmmqbohs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gmgzdekfi.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gqakdirac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gkyktzngu.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/grstumujq.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guzmxbqxn.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gopuzwyvg.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gsbpbethe.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gedtzmaln.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gsiqnxwbe.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gccdmmuil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gmsrugvby.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/grgzulkng.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gdykozagw.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gpvtxxpay.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gdevcrplu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkttqarzs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gjursanpo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gmxhnkiwa.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gzbooftej.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gwlkxdavk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gkhwuhkce.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gavplbzuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gcqhgdusf.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gjcajwdba.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gfiinifqh.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gfpnbggkj.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gcoodzufd.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gfjlvsbwg.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gmnefiess.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsndlszdc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gfrqtffqo.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gcqaagdia.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/glromgfvd.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gbzqkqvhe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gzmggkzni.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gizdacqem.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glksumcvw.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/girotczgn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gqtdkwyqj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/ghxbvfrut.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gaexcmpuv.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/goerfvprq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gzzgvojnp.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gukbwmnjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gdkjjzbri.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/guketiees.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gblmflryq.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gnofmkfkm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gaaleixax.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gbvhnbcdv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqdvnuqx.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gxmbjaobg.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gkctbifhb.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gftzejwvc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gnfiytwui.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gkidtrbli.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gsfrqkpnk.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gwkxfioup.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gszrknoou.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqqgpiamm.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/guelvfamj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gehijygnj.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gbdqwnfqu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gzuvahlol.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gzmpedtli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnmcfooyy.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gqndgwilm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkqtcqekn.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gfojlcrvf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grwhnsjtk.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gkmbmotpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gphkdfavk.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gwxtqevft.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gswopqhdn.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gisqlvdcc.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gaacbxwdj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/guyiasvuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gwhrjlndr.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gqzrzzzva.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gqgyullvz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gvhddkzgp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gmvjpvoey.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/goatyhfap.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gefostndb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/goqkcrypv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gxmwpvvsh.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gdjvkfpcr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/ghovmlfco.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gbjettjfr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/guiaumxiw.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/ggdpwqdnj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnciqzbkw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gflbdaedn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gofkglmfn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glijwascl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gyrtyijud.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/ggpuriyrv.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gtsehskkw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gnejnwptn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghpwonewr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnukferva.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/grlrmzalr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gbvnbeisv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gcwhnfgpg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gzoxvpasl.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gnxhsryxg.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gbqiwgszx.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gouzwzsrs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gomkviciu.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/giaelhsuy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/guptfjsjd.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gmooagiku.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/ghsefczkt.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gqxqgjpku.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gimxsteyr.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gdzignruo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gdghdluid.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gfgrburbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmkdlnqgt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gryyrwefq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/garizvcuh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gipfporec.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gielpitqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gptutqlkx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjmfirsqa.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ggiaxyxqy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/glvyifjss.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gtitpxhfl.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/ggwnkbxrg.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gscttvgep.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gnemcstmb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gijvyidfh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/ggirvplwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbabjcw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gkbtojder.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcjrlgyet.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ghnchgrxn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gopuqhxpt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/glktzmrvp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdtoufdlx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gyhzikrhb.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gbnkgiwli.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gkkgozzfm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/grjykfxgr.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gjnfjudjc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gjsuwrsul.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gupziyzgg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gnqdzejxj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gwbltqguu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/ghbqlarmj.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gpwausydf.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gurjnbuyz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gagxehofk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gnrvbdkup.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbfimdgmb.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggbnehwyu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gweuuxskf.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gipempmyo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gybzavhdh.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gzdvygxuv.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gvzvpowdd.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gohpwemfa.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gkncopwsk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gmrflskpi.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gsthqnrws.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gwyotnwjn.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gzmbopcan.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gznurgkbf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/ghdgxuunt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gvhhktxtl.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gzhhceocv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gzqfzjoar.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gypdvrstb.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gbvqmumva.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/golwelius.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/ggudewaal.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gmaeybddx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gymiarsga.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/grwuwajko.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/glkshhwnu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/giyfcyygk.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/geuzrhjcx.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gzuzlimjo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcdyxwd.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gdxpglhxu.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gxzwxlwac.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gkibgrigb.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/grhqewiia.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/govrykawl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gswogdpno.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gkyfolzxo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gwwkkotlh.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gezvjdmlw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gbdpjpzis.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gizxvrjmg.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gfmmmcqpy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gemjpwvai.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gyffpqksu.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gozhykalr.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gcnackzgc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gkenymqep.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/getbwdgby.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gkoygkghg.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gwjcvbvby.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gfaszighp.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/givhcrqbp.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/ghnqlxdjt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gqpeyrdzq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gvyhpzolo.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gguxzsifq.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gexpbatbb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcgxwsdtb.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gfxptkobq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmeilvqbi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/ghkkebuvi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/glxykfzyy.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gbilrzxbf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gajqaqrzg.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gsaycjeyf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/grkgezuih.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghdqdysrg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/glpjdgaho.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gtcgnjpin.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gbecmhfpz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gwqovflee.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/goiqfgqgz.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gkkybyavw.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/ggkxbplgz.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/galtteqmw.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkuunlllx.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/glgacfpyg.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gvaveowrl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gmwruyvxq.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gklixfysu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gnmhbteph.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gitfxbzap.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gbdzlifao.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdopqaeqb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gfnvhdpyl.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gtubllfev.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/guszjjfre.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gikusttak.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gtxwjfubz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/glypyeltb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gnqmaacev.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwvohqvwv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gmwbgatam.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxxtvpzua.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gusyatwik.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/ghlugejnn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gyeprbzha.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gtdomqjgr.sHtML


<!-- 参考信息 -->