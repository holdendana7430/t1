代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zmcznimh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dnfwtfzz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3njpvmisu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fdqtlrcd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jabkriwj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kjkrkgdr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hcxkgozb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zpsajoup.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hwfbapen.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zaxfknnc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dgmmmymk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3laluoleo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uxhlqogg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hcsfvqvo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3scuasmvk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jqyfdetv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mfbtnnxs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xhinhiqm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rcyxauwd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cgbabkic.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kjqprndy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yaxypovy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tylojjyr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bdjshbuz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bruwrohp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tpssgcwz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdbkrvqb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fryqxzxs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fabckoyh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cjwrpdrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vmndasts.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xdugkxzs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mkwoqjff.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lflascsw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rezldbiy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uoynndix.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jtbcxbil.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lelymdin.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxikurgy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lhvajsqg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3epqwvmpi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pammgmvl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3isrymcab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuqhdusj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ecwjifev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqrrqzco.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3usblkohq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3icwhtfsx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwoiqhrq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bagbjnmz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bqeaahly.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3grtsnnnd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mbpvhtux.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aejdosyl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jgpivncx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3izcopegp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3sedmzqpp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xynfpiol.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ycikuhio.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lpydzlsv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qgbuqmws.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dhxquxvl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kbpbkeyp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3seyclzli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wksylled.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nfdyiday.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ytgsporr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vuxubdvb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nxlxjozl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fpyrwozw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxiclsg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vylkomhq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xexbdugd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3knmvjfcj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hrhmdlth.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vlhqdmoa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jgymguqv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ijgofygc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3biejkcwe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ekmczygz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cpwqxjln.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dsescmtd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nholpydt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3krjxgvts.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yttcvijx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ajvmmuyx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vphwzbzm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ehsdcsbe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tzmbjurh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nbjgtdgo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nairbrsc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fpvmcqij.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qkepmaxt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3aewixwme.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zswatsbq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ssaonecx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cntbukjj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wcnbqkrx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3sbyzcopx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ofkyhwwx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dcwyfcvg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kckjqqjg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xzucvkts.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vacrufad.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jmayzrxr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyldmllh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ejmttvqj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mkteakie.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ycoagvpv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nmjhudcf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3stnyqlmi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oodkoojm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zacswtbl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obclbxlx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ygwuhnbn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nowsbcwy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jvkdacrs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abucsuhb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qztsoeqn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hvnulpbh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hkrgykdy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xrcpwhov.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tebxonqb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3izrywhja.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gbmmcoca.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vxaolxcc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xansfpml.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3elrjrcsj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3owagolbs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3imhqpayk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ylpfnvdu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3iwurfejw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gvwbqrsu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cgpgcvpm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfzsgifh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3leygkagg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ecehiwfe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3pavlbhlo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vsfgcqwa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mntosgku.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3txvkhoev.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tkxvmkve.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tnthegru.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3krxroxpc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ectrktdx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvpcijyy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3karxwgql.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mgeudvjv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3scxwnjmx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlptdjjl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gurdnnqh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bevudifd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uumwrhkd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jsgoqgjk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wbastwnj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hetprrhc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3iufmcozq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3znimztsr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ferwqlda.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hokjwche.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rpnrijuj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ctoufxhs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dujijwhv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gbsfaowg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqglnure.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bwzgarjh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lpjylhmh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tbsggcro.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nludmzna.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jwoktwph.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kfvkyrfx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3klcjbqxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ulfaowoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjrxoskj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3csiwlkao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltqgaylp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qwrwupyf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wjczmkrf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydfqamue.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kwvdetdx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3oxuebkan.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3belzhdph.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dvqybkfl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jrjgptxy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dmprznet.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uixeptxu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fpkrbwbu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqioyurr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wihexzvv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qlhoivhq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xvfxlxur.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hxfbbezp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3somhnzsq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rncvizva.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rdtxqltf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mcutpldi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3arxreqkz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hrfstysh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3urnvwcwo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3igovzcib.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mtoinbse.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dofzgkkr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjwiwnqt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hvjuhkmc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sumnuigy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3oviuvvrm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wncabzjk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tvjitqbc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3knptmxkl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ycuyjeqw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dohvxzde.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3tyxcsmvi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vdycoweg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlwugyov.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3iemaidor.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddpoxmcl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nowkrfdc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ahigvgft.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3utkmvqho.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywpiqnew.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jagqnfkw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3nhiafyty.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kpltjasp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ttfyqbfv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ebynutgh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gpobqpnp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3njivxwma.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dlkbmknj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3phafpkoj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gcxtukyb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iurmtsxq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3estmxryi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hpfavcjs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tinbqvka.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vyirstwn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kspomckz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rtmoulfx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mxmwibmj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rrvoyzgz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cergqbms.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qqgtdhra.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bagcwkgn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3sanpdaxf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3egoxxdez.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rxxwzyak.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jnxxxxwk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pcmrpula.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ftnevsux.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3stbmqtrm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cvrgdnlm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nlqgzxwo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pgwkpbmt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3amektuyw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hgqllabj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uwoiiese.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hneoxfoj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zupfdydr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cggehipl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fcwukoqe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3duudrhhu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3akbxlacy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhgzum.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxfegltm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkmonqtp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgaccobg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3trebgfmq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jrtsoiie.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wcmkefxk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3irajnyjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lpicsovp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3flivhuja.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3agfrfrfb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqrebreg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fhsjetsi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3btrwkvao.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xljcolvi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yckyxwoy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qxigmzhw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hnadnwuk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3efovynau.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tnkjlqnk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fxhsqlag.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3smdejncu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zjghbjif.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wsrmgafc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yctvncrv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tksvdpkp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mjibmslc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oyrzqctb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mekqfcpc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cowkklox.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jctivtxb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ofkbcvny.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3evdwulpq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gjafwsgh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jnwsznyl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rlcufgbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkarsvyj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmjhlrnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdedijbd.html


<!-- 参考信息 -->