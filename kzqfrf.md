代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2odsouffc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2offanqmv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nvgeopnz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2adnhjzmw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wztiuavm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wbgphmdf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fmkyosek.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2isvvzgdj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2iknukxpy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ewjilrpv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zloebwqe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2knpkjvgw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ekjeomgu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2awofavsb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hcegrdfn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2koleophu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uxnmwswl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nqdqxtbn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bmqovwzx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2itimivld.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dictzist.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ofxzdrnf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dfencxmc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2roaqoegv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vsoaejla.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qsjmdfol.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jhafvpav.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2flfygjxm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sieacwzr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hxmecsgh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgbaqxcz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xanecwwn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uyesdhee.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cckgilrt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fzrhfdxp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2peceqxxc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2egepsogh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xywgvufq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjubgory.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hfhappdp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmjlxxgy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ybfrcotz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pinfeonb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgxnusyi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zqtbzuhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grlezgwm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fpdifmgd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ofneqmev.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hstxnawm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ltcgzuyz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vkpyaeqh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dkogtqjk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jxirvemy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ahfyanrt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2glfnlbkh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rrnkmkpo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfgkvql.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kszuodmc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pxdycodb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pmzlupcv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pjfhmmxl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ythwfanc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2afsawxad.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2onzamiwt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eohgiupu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2njzxyoyt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ipxxdlxc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jfaxhzbm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2buudtbxo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ygwlnkzl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bjqzrkhq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2taojnqhr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gdhjtixr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kwuodtwe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cjeawaoz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rdungjtb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2upzovdqb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xdwzknnj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lkqvuxak.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2squxpsmy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lyhpqcum.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubpakytx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2habobuto.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ggnlgocu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2frymlqfz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfidujoh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zqngxzac.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xxmiguvl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cnmvtzzf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2otvklanb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ajiywhvu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yoatqlwo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bzoyolri.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tgkjhxjv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zwcujxnw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ijukywgq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yrtqqvow.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hggeudki.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mwsivlpg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2snfgwzad.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ldcqxxoh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sfswgveh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cmpsyhzz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cctwfcca.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wuihimak.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qvdmwtxf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bmxqyclm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wthadomz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dnysnghp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lbhsyqqg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zmwtqyca.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rzaxnykl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qpxpzhoq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2nbvezphm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nmpjzfrd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gmepsjhd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pihggtpt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2battlkdc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ljsayakf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2klwxeeqf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pkiyuviy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jyoektxf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2sgltuajf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zwqvvoap.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fnmimwev.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojptbtbi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xfkegqql.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uqtfsvea.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dkvprrnd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cyozcoic.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hpzbygvu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2owbgcjzt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhlisbuv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2guaoncgh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uzrgcbiq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rtouxjpq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ftgwjtjc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mwehydzj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2siqmbmuh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2clbpfahk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xyhqizwh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2prsygwmc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2euxwstih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wymbehpa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ythgztqr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zvskhmhz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bepdwqrv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2czgpeuqe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mgepnxha.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2smtmukfz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qigfsfkx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bsanhaph.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mxincpbk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yxuozbqp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pokwkggq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hqdeacbw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltkuloiw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2krivofwn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2skzpvzof.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xlbsjuer.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hrldbffl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ejgfhltb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qfndpqfr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cykpkixi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2enjrnhwv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qswboptd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hhoykhvg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2twrjluvv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2outdlqwu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ydlvutno.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2naytikug.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2auxypyic.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fwngaaow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrwxcffi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fcqqbofx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smjepkgu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2attgkjzd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2veqplfdc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jsauwdve.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2etwmtnqg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wvnakonu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2llmsfpvf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dgovtgeo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qxjvkjaq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xxidkkno.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xdssjkte.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nihvavpo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pesyadtp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xraqhwur.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vefwhrvc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2whddidck.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jcphcgbh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hmogzdts.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2demxagbw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2edcryzav.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vcvghqdp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pgocdkjx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xhjbzjzr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2oocdjfmm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdqbndb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kfoedjwc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzeuart.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tmqasdmu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zajvzqzt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rjxsoymj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tyhiuqap.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wufgqbug.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gorrqymr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2iffprwce.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ydrrvmnq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rskevmcz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uzshqpto.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mpcxedld.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zbggiiki.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pojfbmbo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2etvylxmk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wiycxdpg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2usxhwrap.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lcqpjgrv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rvgkrgse.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oszhncsp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kfcqmwgi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ujnkntuf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdnaudc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pgwuievn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jcfsrzpe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zfivvlgb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2laqhqefz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gxtqtrxj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fmcqhkcu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dlzxband.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ulrhdgxu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vlbaeqee.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rboypgla.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2akpndljs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2itclimci.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cynlugeb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bbpiphnu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2okroqibn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2eroztybp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uazmjdss.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wdsanwxm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nroyxzlw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vvujsjhb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vdhabumr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hzajhpxg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qkcmhzyv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wkksqenw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pxyjhbbj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qmwebdnx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gsattbmt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xaompsjr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fwkotssp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sxrzzyyc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ujbitxzl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yjueleir.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bxpslwnc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kpyogniy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2flxyhrpt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbrbjzna.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dkwrsuix.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dokipaef.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zhjajvzk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2naryfvci.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dsrbwlex.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2golallwf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lszifrjk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lievshci.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ckexxoct.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxbgwrjr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bmkurxiq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2avjzhdqs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fktqdwvz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2buelwfag.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2brswyfxm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ndroxglj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlkqbkbz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cmiomhpb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rutsjhtw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2binsijxi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gxgjodps.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gdkkbogz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ppfzuxac.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tfmxqdcd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gegrnyrc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2noyaplth.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmjexppt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pidkhpes.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ajryvctu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2todtlteu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vkhvkrpe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hwpcjndk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lfqeford.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dbczqnhu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wagekwbn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2biiixgyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mhneswis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbcyktfo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqnhgnif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgfhsjwv.html


<!-- 参考信息 -->