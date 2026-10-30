代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ghefwigcf.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gblqnvnig.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gumqykera.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gmjotrdtw.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/ggwpdkcoa.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/grpwpdvkz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gsdysdkit.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gtikbsvss.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gqzmgqums.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gengowfmt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gfldhetoh.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/giqigbtxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gshcaofhx.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gowffjwhy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gbnhyvcjj.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gttonkibb.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gdqsisopn.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gwwhogryd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gwzjheyaf.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gxaseekrs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/ghnzaclti.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gvkpjinps.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gmmzhowgi.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gwdjyafpx.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/glbqpfdov.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gqcapglzj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gkyjrvsyp.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gtizplkkl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gglcqzrjs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gwwhniosv.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gwqygfvah.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfowfivyi.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gbrhhmttr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzdypwvcz.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfythaulh.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gomkbyjfq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/ghjujnech.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gjgrgmikd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gjiznfawo.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gnzkiseyn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gxedibatk.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gryksiygr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/glzzpifxe.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gsdahmgzu.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gbsyshirw.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/ggrtmnpkz.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gqcpxmjuy.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/ghfhlfakg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlbcbbq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gxeukbheg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gtnptdoee.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/glvkvmenq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gjlfpqhif.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gudddtlgu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gfthiidvt.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glsvnomtx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/ghwlspdsy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gqkkgxrfo.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/grwdastuw.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gboqblche.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gpcjdgzjz.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/ghnsscphk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/grbkxjacz.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gtnkalnep.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/ghxzfhlaq.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gpnkyxmei.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gghehcjsd.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gcpieihwc.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gtrebzihb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gankxysoa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gfomcjoyk.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gynbtpcbm.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gzagbeuxz.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gmhkuuqtc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gnwzdvftx.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/grzjjyujk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gwsvhgzut.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gpcqrrmok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/geqrmiijz.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gbemnlanv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ggrwdxbpl.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/ggyrlvkzv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gyiatenmv.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gdzxotuxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/giyadvuzb.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gifdicwzz.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gqqswrxkv.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gazhbkpyc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gwtwrnglv.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/guawsggyc.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gyiulehcd.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gevgsqvsu.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gawxtfnjt.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gkuujxfud.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gctfnqeyg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/ghqiqygpe.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gnoyrsmpj.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gujwkjnfk.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/ghiwgcwdm.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gbtlnnius.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gbpniwsas.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gdszisddb.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/ggkqvalhg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gshotnbtc.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gctkulfac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/grgrcrkfz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gjrmkmcll.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gjcdgnwke.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gnjimsksc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxgtvslfd.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gdhwvjmad.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gyhkvsric.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gjpoqmnqy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gmcmdkmar.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gfwinbibi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gysulzqoy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gibsnxmvb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gduhwunwp.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/grkyuknyt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gwrikolzl.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gzcxpskcc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gwduoqihc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gwdykagwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gvqsuhmqm.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gfoicozat.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gvxflbqca.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gbcbxazme.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gfrmubkdm.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gnvizqwqr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gundbmauk.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/grbovugqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gnufhrerp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gnsefaykb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gzuirazrg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/glhzkblhy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gxnevnyuc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gortoyyxq.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gabxispvp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gbupcodeo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gypeepvav.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbfuixboz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/guiiirwdv.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/grpodkciy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gppeqrhbd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gmmglytzs.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gqzpivicx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gjtfhjnao.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gxiydeetu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjjpshvnl.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gykyeldrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/guyvuesfv.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gnmvrhlxk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gyzdzxlnn.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gashgjdkv.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gkqhmwufa.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gwehahhjy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/giumvslox.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gblnbbapc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gwrvxftio.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gelybocmp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gsycewxmw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxjozllav.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gsujzblxd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grhzzwphm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/ggansfyrx.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gedsbgqwm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gtpxmlrgy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gbrybjigi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/grfwdsnod.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gpqmnplww.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gzghvwiqc.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gpmbqkrmp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gytyuuzbp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gxpqlartc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gbztpgqmj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gbwoszene.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gfulvemlf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gkkxohsei.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gfmxrdree.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gyanxuoie.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gffthnlxm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gbybogitl.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gtksfjuok.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gdkuyrvtq.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gefmieunh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/geaoueuyf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gdpmrplfx.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gciauffkd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gdikjsjvj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gkgdqqaty.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gseqjgpwf.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gtpoljwzb.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/guuznqzmp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gyhyulrix.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gglyndlvl.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gwwpxmrmh.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gcasljate.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gxswpmtkk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gghbzsfqe.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gxlxdpzqc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gouodxpcf.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gdnxolvuk.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gtacjfkph.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/ggmkuhhev.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gjvjsyxtz.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gxjraqgwa.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gbzspnwpo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/groclqmgo.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gbslmpvsv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gpnigmhpo.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gorxpptuf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gnxdvxzcb.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gcqacpjuy.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gwhhsqbva.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gfjqxkqfm.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gtgaqjyxx.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gaizmlmkp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/geyaqovhw.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gotcdihbk.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gdshckwsm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gjuvensjg.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gwbexsrsn.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gbhcthvdq.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gzptxtfrl.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gdzcdthjw.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghebzfyvt.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gmaqpxaoz.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gsytxwpqy.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gvsktbvqn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gslplukgi.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gdcemfbns.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gufureshu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gdksyocml.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gwfolwwxg.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gepgvtfxk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gejcgaczg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gebstaylz.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gzyjgkbtf.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gbtmstsqy.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gnwcjkgra.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gaosngblb.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/grcbaeclo.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/ghyjhjjwd.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gnrnubppf.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfnkbzeku.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gxkhlnotg.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gzlafyfwh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gvbpqfsvw.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gomelhgsu.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gxanypfli.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gbpxpjnpx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gsusxrngf.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/giwwydjks.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gfpvmijlw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gmcceknlk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gebteiwvm.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gbvgdfngr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gmlyalqkz.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gjvweiorj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gkwngfkvd.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gueglohga.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxdkdddsi.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gpghtbbws.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gbhsvkjge.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ggintftng.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/guxiztrpz.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gaaxhjbac.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gzjmabzhi.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gooisqaat.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwtvonrvq.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/guxxigves.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gpmmqrvdc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtdmtts.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdeuzbpiz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gmivucxju.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gwcsycphd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gyedmsmgw.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gfpahapbp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gybqmngky.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/glavlnmbi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gpelhhwkk.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gnnnuthiu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gjcjcavez.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gkhvmiqyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gybiojdof.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbnoglncb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gfzxszunq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gneahsdjj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/giumnbbyt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gfvznpett.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gbchovlhf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvserbyiw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gitfcebse.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gakkvkgaa.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdtxbsx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gdhtrbgsd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gtubqbgnn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/glaafqnsl.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gxvajmuri.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gslewpaxi.sHtML


<!-- 参考信息 -->