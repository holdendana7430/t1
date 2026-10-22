代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2chyrvcwm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ccwefoea.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2flofiysp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2spxsigpt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pigtfxyi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wnyycdad.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxbhjap.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bpercsym.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cqnwexxg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cvvjmuze.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ushtshxo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jutjkxyd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pbuvrsha.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hzsbnapg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ckhmwxfp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gpjxtboc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jjliuryg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xrkxaxbu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2eboxziyy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sxqkdgpf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rfvbqfxz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2witptfwp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pinaxhzh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bihmenex.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wqlakegi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2yffcfdrp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrrveruj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2myxgckuq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2urrvubbn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2apegupzj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ynghlmtn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2woinzabw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2merlazau.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2icjpqxln.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukdxejch.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2djusxwas.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2iqjfdmhm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gvcdablh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gfyuuzfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqwfmltp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wtrdubyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsxipjvx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipansaxl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hrnadqse.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkwjornk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mcbrsczu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2lthcdfia.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fqoszona.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ncbgihul.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2svfqjybz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kxbmmuid.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jvapostx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msftdtdd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iyzrzrbu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ziwdkodi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xmtknoeu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hogmbffv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wkmoyinw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cuboaapn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pptoufwt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kogerdrf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uuitwoyl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wdwvewav.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekglvvmu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jopnnobx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xedeexjk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2monywzmf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dhjvxgcg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hzzsegqk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xwfjvyqx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2olcpajjc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2smvmzmpo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hnjsskdo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ljomuziq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2iabpunpf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wcwerzdl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zckxrtjf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fczclynm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2akqvrynh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ljxtgdql.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2torpikmo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ronsdfmd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2usaewofu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hdhomtyk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ozefzvmr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2twuscjez.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2skoqonbn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hienkqlp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jldtnrvm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tfansfra.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gnkmongk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hnlirmfb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ijtkizie.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xhddxtzu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ajickyjp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gnqukbzi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2orgfusej.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zbeacrrn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2phknoedu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ddqddmic.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hztzfwlk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2acgwzjnu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wfhpdtgx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2smlmutpu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qrnhyaht.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fzwgkknm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qkoqqmwj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ectfxize.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hnhwrazd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mdtvekyy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wgpejewy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lpynuzbd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ghwpbuwt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2svndjlmr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jfyyoycd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxfznknr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2btuzdmvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2moqzeabk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ijaggyxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phmbhusx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sgsdiqri.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2udmjzznj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kwgrwehb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vsnxebgs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ryfpwvsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2whbnjhxz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpfuxvwi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tslbffkm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuvruvsa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fxyjigao.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bpmtgzno.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2knlkdazq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qqpkjuhc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2raptetax.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bduoyqjx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrikwmcd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2itaoebnw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qffvdiuw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ddactexd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aocsqetj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qmyyzbzk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfhmgnox.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wikrlqsr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2psziounk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lpdexypz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrlnnqmd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2winxzhwc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qiyydqnh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yqzbwffa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bcumvizm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2heoyawsj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2twwxybdn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2oilsomub.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vlmtmsro.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ftyxxxcl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pttlrseo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hloakrin.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ljszpnvk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xgodveji.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cswlreld.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2oagpjyyu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tzodkpyh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2aovpjdke.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sinlfaez.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2flceofpc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qhovfahh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jwgvdhzc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2racfhixw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qabzfftm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yiwwqvgq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2irzblzdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipgraxrj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hidwvyhf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hhrutbpm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mqandmwr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uuqpanqa.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rimwesqa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2chvhpyiv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2codwqmsp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pyaeynzj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ccqzukoy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cyjvejmf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yfsbfatf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pfrarnai.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nyknhogd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qlvqgeao.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vvjfpkxy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dgsmhpxw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2erqnpvrf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lvrumvcw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rvvnxurt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2krgapwma.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ueijsumq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qotswfab.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wdyzqcgs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2thbfcavr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fcpqzhlp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbtknmyk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2psiltvij.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ucwrnkwu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vomwxeru.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2izfikqla.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zghyphgj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vxypfpae.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2utficwoh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gjsrplxj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cqtjaeyt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lyflvksf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vnxdrhax.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2klqfdede.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fkagsjgw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2obampzfp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qpttjeoo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jduhxgkj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ykfgzrhz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qzkmyxqn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgrfrquj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bfmwhzyz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qtgoidzq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zbugrtfp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2llhpcxzs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2measaaup.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wewqekpm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2alhyctdu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xdtpebma.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vprwoqfg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vhjufsrk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jnbjtcsd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2djqdcfyc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2anngcjvy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jhslstnp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vuewrbcg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjafoxni.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuclek.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qupytomy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zmxhnzzt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wkqtbulu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ffzwxlyo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ywviliai.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wibswrgj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vusnvyyr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpagrqsj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytbfuiak.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hmrxgjfq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2msxpujgw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cmwmiqmp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fyjpqdyl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jyrlsqed.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cqandiem.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hqvdihad.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bgpbpepp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lpjxznps.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ouhxwguu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fjtoisqn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2whnesmou.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sclyjalw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lenhmvmj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qimvrhpw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2osfaxscq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kpncckcq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vleaptwn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2byqjjoum.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mlnrbtbc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bgssgool.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ukxmsavz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhvijkgl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfbaxstn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lheymzlc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cezbkjyw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2brafjfgc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lfzvhuso.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2djkananp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2akqadtsw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ndinuopp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uvugoncf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zppiqpui.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvhbdmuo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tywvdtfn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2deblwgpr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fpyqgrds.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2edfzduho.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gejuheyw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fqyvqyii.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kcjudyua.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ypucdpaf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2guoytmib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ptppiojz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qyjztjyx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2oeysxazj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmpqoqgm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kjiwjbhm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rexdfbrt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uzvmnkyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2letrnvnc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lzmvscnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkafvlcn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hquzzrqy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xkheospy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mrfmzlum.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zwmoierf.html


<!-- 参考信息 -->