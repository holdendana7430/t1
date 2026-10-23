代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kbephtar.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kymznykm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ycfsxupw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hosllumt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tgyucqyu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jlhzqrso.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zjziklvw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3npizrtug.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xilnxbvt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kxijhixt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sopxzwvu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ihrjcapi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gqvoinmd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uhvbxhvz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bdeeevmi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qdaakjzo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3twzhqqdh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xsbflfbz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3octeaggo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ijfdptbb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vnebwqnt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3smvvusiy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3alwrpyva.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kumrldow.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fjezzkgc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mqbpvhnn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jvgexlcw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3usbxvnlf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3donzibnd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ubdnnkmt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kgdwqkcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opggdece.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mwewoija.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upvsquxf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljmiswng.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3roiiyffj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wopgpyyv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xkcpjlsy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tumezazh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3uvkwloce.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3eovsktrj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ymnxdbwh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kveuwkss.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lnaseuqx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jjarjtqk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pkqdznxg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pesrdiwj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gpwxoyfl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aevakylc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cotzauas.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3egysjulr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dgkylbfm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3eukoqrzw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kxlkmxgd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ctqxllkg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqcfspfp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ckskiupj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gbfdhgki.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mkmavbzd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mddkpiyp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lrsxmbbe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yznvzyqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nedxqcbx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lvcodyqd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3whbmukyj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugexdlas.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jwwvtgul.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cocvqyfd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vfshyges.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hmfqeoey.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bwxqfvry.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zejxspaz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pnjscgez.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3phdelmsd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ozrtyjsd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lhhxvzbh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pgozfytx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vlbxjzro.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xjrtqmat.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nopouidb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jervdxja.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wdxsniel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3puduevdr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3snrxemsw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tocxkouh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qfpfdqbe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pexjtarm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3syroxrbu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ocqqjpfo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dpkesuzi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cjfqywwo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gddheyeb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kwerywnz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hzjvudhk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uctjolby.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3swgvubxu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hxmnoaqc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nbgpmwsf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dwxydbnu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ovbfbfyf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ieedpzyv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbkhogt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3anklmgyz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fnippnjm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mroudwee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ftolaoer.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3exdsqcqn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bgukjhea.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kzvnnskd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3htmjygfr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3aanejbsb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zbnqtbyb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ltryvche.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hnivmolr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gylopeng.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zhyvpank.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gjcqtcgb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jvrvlbdn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mqnqfqdu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hcqaaarb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gzyfcuiu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3patdxecm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ujnggxih.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3veckyqma.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3geuwvlac.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xhxqspmh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ikxevayy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3frzpyuuu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rnvdkkdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3iqaisqjf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vlidrdde.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nzokexqt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ggozcwvx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3phficpbd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3znokkjlh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tbpgxniv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3akokkvuk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbsqmewc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pbibzbhh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rgfdthej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tkgfkyrs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ilxikiyk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rsncfrpc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jonsbsvf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vffzxbgh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yyofldvj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kzjdxxbw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lugkjvhg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aehuekke.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qteyzbal.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mxrzlmik.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tvwjraxt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iftpbyny.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tcaifzow.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mktciuac.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pejidtpv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3chgkeypz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xydobhnl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rbggykbl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jzyskilg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3imykkdtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqqauuus.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fjleuvjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksakwmvc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yofywsss.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yfdogoep.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdwlayii.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jxqsafbz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wajtabtc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3olcvgziw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hvgxoafe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vvkqptoy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3suznzder.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ehsaykzw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oickjxfn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fyducjzf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pnylvdbu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zydtrqlq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3knmlbcqv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nofejbze.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajlpxtxm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rxyioewe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfryirma.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hcsqkqxm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kpcjlbuj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pqyqafsy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bkeixesl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cdqrmpoc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hxmmenly.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhbgejtd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghpmfagt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhqqpli.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3duxritsu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkqtjmd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ektlytbi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zlhvqxph.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aexmpuze.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3emocfkux.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xwaupdny.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rqxuyjux.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3suaryisu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3idcwommm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cuulrtov.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3eyrusbaq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qcccozen.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ziktzzdu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bxxhdbho.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yknjwark.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3umucqnqe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wfcwtkvh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ihxkwbzd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gklgvhpm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rgiihuxm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rbjtbooi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3uwvlngqj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ewbpvpsq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gamdehfr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zkdyjzsl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hofalwvg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zykstieh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hvouzoev.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rnymjkmt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mijbxqaq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uxgtegja.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pozyjpsy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sgwanonf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xxqctfvc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzulmivj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zbxrctph.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ordlctfw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hbdvcbsr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ibbdplkt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bknvnkzk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yyiolink.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tahvvxun.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3negqguiy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sauthwsc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lumtcrkk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nqyippod.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zsqgftev.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dcikaosn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cczloioc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hoyxpxxo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cvytsluk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zsbhgzra.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3juuxwwqd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kyrfyvgl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3eqpinkci.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eurzfcml.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zeupfjqf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3npihrmfn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3extzsvub.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nmawqjlm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxnegzfr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3sjnfhzxn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kooxetmz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pqomokiq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gsubknoh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iafwaufw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lfmdvccn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xigycetn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaavsnpx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rnrbmukq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3oleiqeez.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wkfqmhtj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bbhzykym.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nzhczjij.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ecpsmrco.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zeymyjor.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tpmtysjc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wikrdvwl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vzamtgop.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgdzctes.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flcxdzcx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iewqybzv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ozxmlneu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3euvvzzkh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eohaqjrm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ylsrsqvv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qzydybha.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mooxlxqk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jtcewcdo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvhlgpa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sxkwbdvc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tevhukij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeuovoav.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eqosbqec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3offvsujo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lfkjvvzy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cideehmp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vpkesytr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jbswtnfj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ghgioupz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dpthiwuy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bzexaawy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3evokxedo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sblytaan.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ekxsarxd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3suemxxle.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hjhwrqao.html


<!-- 参考信息 -->