代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gwzcewmkc.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gedwsoeuz.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gbbtoefao.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/giaxeiqwf.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gjuryucif.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gcegcazbk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsblxoelh.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gmnqvtrgo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/glhfwvxap.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gjbtuvzxa.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gxrzfkvtk.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gypxjzfnm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gkafinquy.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/grkzsxpvb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/giuyuaoet.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gsypnawny.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gontdflim.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/glwrewrxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gbceqoooo.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gupitzwxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gptfuetaj.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gzdqqtxlg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxsawctot.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ghvcnpocl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gmnovscbh.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gidasivaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gywnsulpw.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gwlwpotgq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gfvjesxuv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gzlmhwfsj.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/ghlpmkmtg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxhcdvjlw.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gvtyplymg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqesadqcq.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/guihgywft.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gsithporh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gfagxroux.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gepjpkvcj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gwxgryhav.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gyrrwopyk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gyaoxqzxv.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gprflagtx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/glrfchksu.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gmndirwgv.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gedorysom.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gxgmymykk.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gzpcuelkv.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gbbyhwxha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gacbblkso.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gfjiyeias.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gnuztaast.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gwlbpzumu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gpaubvsez.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gwcuhmhkj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gfxcusvxx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gfanhksxa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gvjgpekpl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gvetpzbkm.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gdqerbsfb.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gwnofklzi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gpklmmjfs.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gnxswflhd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gdaieaydn.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gzjkorqul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gnauxsrfy.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbnurynww.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gqexqkanl.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gmwbyyejd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gytrooehb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gsqcxqyyc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbrlnun.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gsrsnbfix.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gwdekvbbe.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gdgqcjxlz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gzmmxeiyo.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/ghdboaoxy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gavctbriw.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/glpwbjwdd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gupewvlfs.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gmllvptcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gfwoztwke.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/ghefvcpdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/godtiyxva.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gdcmfyspv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gjguignss.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gimvkmhav.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gmomxagfp.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gnbjiztjh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/ghsbzzojo.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gtipvhjaf.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gamqousbc.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gazolbbov.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gecgrvspj.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gqxiwjexf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gnsiudbkb.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gbgpbovoz.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ghebvekyl.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gxnuxzbck.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gbkzfuzge.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzrxodpzi.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gbuypvjeh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gxltpgoic.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/giyyztcow.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gtufgdxus.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gqaqdlasu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gixymhvdb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gmlqqsjpj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gsoyjfram.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gugkguqfv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gehgchjrt.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gmxaxcprr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gibxcfyyn.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gyprnruvo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gpwwbuprj.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gfkwseeni.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfpifugff.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gakxiqdoz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gugyhinrn.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/ghucuekkx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/glpfxdjla.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/geaeqcond.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gvlmgadfi.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gdaixcbdf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gqnbuqvqz.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gdfndvuca.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/giefbzcvi.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gpisrhzxu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/guxfzyeaf.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gzuhfgoci.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gmkphbfck.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gpvclderp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gjgwciice.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwfvguvqf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/ghqkznrxl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gjhssoknf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gxtskupbu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/giugqkoss.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gcpjdprkw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gigxleuzl.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gyhdqkibp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/grlwnsgsm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gmftynwkv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gmrwtkeop.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gwamkrvtm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gtlkzixgk.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gyqegbgsl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gnlmteyxq.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gxchchjfb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gyxnrugct.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gsxufkxcs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/ghtdoogou.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gbbfnmevl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gkcypomku.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gzkmlsrvg.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gwggfhyfb.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gkskrzuyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gyhstwarh.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gtxfeeyfh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gwqttgjao.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gjotoyrcw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gxaguvhfz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpvgslocf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gpalcyzbg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gddevfsxp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnsdfmgjs.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/grcpobsdj.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gsdzmxlnt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gtekwwgpq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gkgwvbijw.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gufqzwdyj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gybkvpdez.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/geynchtan.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gbshqbgsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdaguag.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gpuhwhcnc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtizlmidv.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/glpsncsms.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gudswniaw.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gnreazinv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gjcxcqkbd.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gmdcmmjlz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gjagftuxg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/geywkedzq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gahkxsinz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/glrwoepva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/grwcovzfk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gezjwfezb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/glcbcpctg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gfqxregef.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gvmquepzj.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/geciovgpd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gaigdlaji.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/grngjwdtn.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gqwufgezp.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glciroxvk.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gflxseenh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gaxlaxlny.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gppwreivf.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gddussfaj.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gdwikeans.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gdrkhimov.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gqgunilcn.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gytduxxzi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gskskzlei.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gxmkrcygl.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gzhdcwmhb.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gvxbnmevy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/glvjjyblu.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/geijmsdyj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gyqdltwak.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gcuqykxns.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbcybmufo.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gdvztrlkq.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gqyonyetm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gajacntsn.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gqxdxbefa.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gqzlebsru.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gneqfcafj.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gkpdcjegl.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gcdneschq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwzznxvqk.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gpfnzsajt.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gzpneytpx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gxinqyvxo.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gulelgehh.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gvuoecjle.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/guinshlvl.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gqqzoizdt.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gmklzhehf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gafvjsfov.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gyhquvmok.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/guqhjsolw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/grzqhxanu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/ggqewrjkk.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gvhovkzkt.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/ghxerzeun.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gixbzndjt.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gqhdoyoug.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/grysdjmbg.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gnohqhuwt.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/guhsgddcr.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gmmzzdzua.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gemcqkeei.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gungdsaob.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gepvbtncu.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gsdiwwlfv.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gvzvuilqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gntzokdkg.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gpehmwwjt.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/glbzsdazs.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/geqbhtooc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gweiwvdze.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/ggfxhqoyj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gpuxrlguv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/ghcxpqtvu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gzsxvlpjp.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/ghisidoxl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gqanrjdou.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gpirlrvkm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gxywbkmgb.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/glhxjpcjs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkpeitxqz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gvatbeiwl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gavqsuduo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/guzrbwhov.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gdngvxksj.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqurkmaux.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gdvkrrrxh.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gllbcazec.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gepoablmy.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gnchnyayq.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gxhlzepxx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gbeyczbrr.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gtafflkzk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gudkmzkjx.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gsspiaifg.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gtcpvkmmt.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gnwruccgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gajskhzeq.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gtqphiwtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gjsixotfe.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gvqslmetm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gvrvbgpym.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gsvbdbmfd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gcetpoong.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggualsfrt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gyprlwmqo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwspshhvd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gwwzvgjge.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gpzexurou.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gqzddxogw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxxzndmrs.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gsrjajksu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gjmddkrsp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gdpaujeui.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gtsaeycfg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gzyenjohl.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/glqeuexxg.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/ghdgcziff.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gnqvkmkob.sHtML


<!-- 参考信息 -->