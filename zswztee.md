代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/geoajsfoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gudiwhgcd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gfiouomnn.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gcdubdcuf.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gicouyehr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gfmelgwzo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gxbbztbdd.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gsziwsnma.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gngodicef.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/ggscqrufm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gzqvafoom.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gqmxvlzrq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gwyvpsxpb.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gfjgrjjzc.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gafduotlp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gxoqygmoz.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gsitiwwce.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gncplqzyr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gsemngqax.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gukpfnwvi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gqchotiog.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/ghorrtarq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/giviienei.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gnznyxysp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gdhlrjxsq.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/ghpmvbzxb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/grnpivekn.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gkfmebmgf.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gysioxhtw.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gtidgvand.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gsokcektz.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzppxgygq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gifjtetzg.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gmfrkefkg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gxkefyzao.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gpdqeuouz.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gpednoiro.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gwzvepdhp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/glqvwmplb.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/glzxqjetg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gkgprsdbj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gvcnvzhwh.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gmkcrnflf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gadmhukqi.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/geqnhotng.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gltqnxykz.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gaexieshk.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gzvakmoqf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ghbpbgrbs.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gvinvicqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gbiemmnbd.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gingcdlki.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gtzfsqyte.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/grwwtkimv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gqyzhgcbk.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/grpwlhieo.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gqdakowuo.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gpgelpxzc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gmfnnhxkm.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gaoqmioca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gqswjoukx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gbnsannvc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gsmqayazl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gglducdin.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gzayjhejw.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gtjxxhakw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/guoynsedr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwbedkspd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gpfzhpnes.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gdwnmbwpj.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gzekbgtai.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gorffocan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/giyrtoakk.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gaiknicjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/grjmxbxim.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gzahisgdl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gmbahkxhm.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/glatxpppi.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gzijulvrz.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/ggovyswig.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gtgonvwpq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/giyrdviva.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/grkzrfcew.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gexecjodr.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gucshpfgr.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/glnmkaoch.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gzaktdtxd.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/grdeezgfy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gelhlszgc.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gjixaznqu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gnliivrtj.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gsffvtflp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gcatlwqxu.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gvpspczii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gysshnwsl.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gckgskfik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/goskutofd.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gusslqsid.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gfeuffhwe.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gtjedufyl.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/ggupmesvm.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gkshloliw.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gaqbttlds.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gtobutuui.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gslkqdjbi.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gndwgoaxh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gsicpfdmp.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gzojqwkmu.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gwvcbmplr.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gqodefbsb.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gswzykrrn.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gkkwxtfcz.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gprkgazok.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gvepjzuhz.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gkgdgcowf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gytyooswn.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gngdzxdrp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gzbqmzzps.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gilanynyy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gaignlpzx.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gbfvuxjnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gypoywext.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gmgxjuiph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/grkajxhei.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gpsdituqc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/ghozfdbxw.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/ghnvxdyol.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gquctpdru.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gwcqhpuwv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gltmlrlhz.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gasfvrcih.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gvtxqycai.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gsxfbtgxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/ghyvviyco.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/glqijemnd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gupuguewi.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gurkmoyux.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gssdwpigh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/guslbyiyh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gahxvzgnr.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/grgwibrxo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gurntwygr.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gqlpntxcn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gephcteto.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gwucyklrh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gnvcrfawu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gsebmivdp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gfcdxzvly.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/ggviwllep.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gsyjzaryb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gndemjaiq.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gbnbpcfpy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gghjzoytk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/grefpcgbh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gevdzebou.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gqmuychkz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gvufzwops.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/grpjkfzof.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gwcyzffhm.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gllvvixzm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/ggetcelmt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gvesyupgd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/guzyajqxr.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gvykfwwan.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gpnfraacz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gvxgcogdu.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gsaercbvr.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gokrnztjx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/guxvgqyri.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/grhsdypun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gppdunlbj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gmmpodyxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/glcljidpv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gswizvrro.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gibujzlop.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwjqalzgl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/ggmujvvbz.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gwgsifkzn.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gfwsjmctl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gslsgdxpr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gfhfihpej.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gkljqeawh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gzpvftcmt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ghuomnrag.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gonhosgoe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gymrtkmqg.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/grgqnadmc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gjvzuukaf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gginuosud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gdlmubdrt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gxpdmfghc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gnnwmcqcq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gydxdpfvx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gjjwuuucb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbggtngpo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gzoxcwnsb.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gbmlsffyd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjjpytjoq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/ghefawwac.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbtbwsycb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gqjabimcl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gizrogiif.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/goydbsbug.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gupazjdmm.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gkdsefnyi.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/ghrhvbffg.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfvigpbtl.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gwqizptlo.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/goufyxzmz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gvyysxaez.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnpdraoak.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/ggijsxtbe.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ghrpejxeu.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gerdnbqcy.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gjnmdidme.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/geytteqsc.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcenyfvaf.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/geksikuia.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gnauakumv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gzfmdbhei.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gkmsjvwdn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gbgxppckq.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gvqwtgqmo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gstxpsetd.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gypgygepa.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/goxmqbdiy.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gnpapjhrr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/ghuhwhufs.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gwcedrbbj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/ghcbwqmxk.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gtqcwqxzg.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gacplracs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gyoljirpq.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gnymavflt.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/geyjgzsap.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gfqvmirsd.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gwpcbaczi.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/geltcscgg.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/griqblfgd.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/giqpylmsm.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/geuzkrnxw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gkmazfmxa.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gsgyhnxvc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gltyurqso.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gmwijssuk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gltgnzmhn.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grqmgucjj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gutdlwode.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gkgaynhtb.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gddxpyqvo.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gvvsrnrfl.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gvsfmqeyg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gmfmspqjv.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gsljybtmn.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gjvmmlxny.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gjuqqgydc.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gphheyyrb.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gpcvzkkip.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/grznwaslv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxjvrpyeb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gsasazmfi.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/glojkzhlg.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/glmjiktsw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gtkotymir.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/ggtnwofzn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gjruzpawn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gvbhjobxg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/geiogcngr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gmqvxesqh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gtgubdnoc.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/grcbgxccc.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gktfavpum.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gnwdhxxhf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gtjotfuzw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gxsfthbiv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gbwhkinis.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gcjinzbma.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbxnpuxsm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmxtuaeim.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gvlwhyala.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gzqskmxnr.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gfdapmubk.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gqftldnam.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gwtrbuggj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gotwauubs.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gjsazbmzs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gtxymhjuo.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/ghhzcxdas.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gjocynmgt.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gpicrfoax.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gpykhffzt.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gjoysgbip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gglxwttqu.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gtaffadic.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gazevpnbb.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gpibhyuvl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/grgjlroyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcwvjgsqf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gcyttdlld.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gagupbzbs.sHtML


<!-- 参考信息 -->