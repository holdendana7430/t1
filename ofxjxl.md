代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gjboiyvl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3isvpgnkj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zkszewhb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gqausyfv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vvwosgnq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kahdmbam.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wxavawrp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dgaasivy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3iycwxtkt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zlqjpbwh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jjkbrsuz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rxdxsfak.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zowcktdg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xiyrbtjz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3beadwvjz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3sorffiey.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qindsplk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mlmdfmze.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xuyikkiq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ymhftlgx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uoetocwc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nkicbgxm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tvpnegge.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hnfpzmko.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pdtshhga.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vxdezbpp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wkpxnvbr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3afvrirxg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3aoshlsiv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lfklbvrv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uwoldxiv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3slpkaitv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ovqffcyu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3sbxtabuf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3emgxrpfl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gtekoiic.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfpxwkyt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qvqqxrgr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ftxcnirt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udtzqqnt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3emfnbzyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvppcroc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmxlxnrj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iwyresfx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3slqfqima.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uiikxdlx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yetzrzpd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ohppntwv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3buawxvbh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fhdhxiod.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kzlamosg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fztlvmuv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwpjbkcf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3biqsnzfj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lgraqewa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zzpsrlwz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vuwndqpb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bhxvsvyz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ujvjtlhs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3abjxjltm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3skayisfz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lfjwszoo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zvefqptp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfkzwidb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ozvuaovf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kvgdxtvk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aslhbutr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qrgjqflq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3typbyhvx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qtymgyfq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ifmkocuj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nksbfwtk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ppuelljv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fuveogbz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zseopowt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mgueolte.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mctwybyw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdsmctmy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hbiwirek.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ljowzltq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vlkntyxv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3grojikoq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fgzorwhh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3apxvbakc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3svoszkml.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mqedxmzg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dekrwide.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ewjmlboe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ouazygyx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qefeznyj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3assfuofq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pzxxconz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jkoprwzg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tdtydgzm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rgfofqrn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mxxoprxu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3eakutela.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ygdmtqhe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3agzngisy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mhshnzkw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dvpiasto.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xbbmxvwe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ittmrjag.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jeyfeuth.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vrmzzrjg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3spzaqcug.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qzpdjisv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fdqznwiq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wxbpubss.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owjevrel.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3psuhphgm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hwbwcruy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ezxxokma.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttsqpynt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3adltrifq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3uxqwerwg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dqftlrrg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mgjfoudb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bptmqoww.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jwzpinsr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rrwdtuma.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lwnzrhiy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ytfpltef.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nexesnxl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uskiecvw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tqtlonpz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gaqxjkvf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yjordcom.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3irffsfcz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tifuxsop.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hskubtdn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3inogdqxk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qkwkkxlg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vyaivyyg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ylkzacxl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmexdmsp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dwwnehfz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ntrdwajs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nlxbdoxb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrnkuujv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jowmyxcr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gzxbpjot.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ayxaljkk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cruqvair.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3glaecgeq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xuauwjvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gsdsxxtl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3diafpwzy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jqltzhsz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cddkqpic.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vcjiuhwp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yvgkbifl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mcyowkzd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cswhuoxc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3klryqhmp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nbzzjvts.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3yestpbxs.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wtgalufc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wokpqtfs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cqmlfolk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3imrzuvgi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mewfopnp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fcbkyifd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jwbmmwmn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jliyrcef.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3efarpmfa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tbzyvluh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3owzzjfnr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3huxbhzhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3treqwfko.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oqzxnywj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnynrhhq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3okoxjnrn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jdkksmhr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fwtcfbnm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bkqxojqz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ovzxympu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fcubrjlr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pmudjmyx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lbqhltig.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hzhptlse.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3esbsbspe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jxdxxlbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vzvqriqm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cvawqgnq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vqrucrae.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3epylsgwi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vxgmgmba.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3noulgsoj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wldyyyar.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkstpuzl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3skjxhmcl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wcbfmqik.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mwoaulpl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pmryqjtb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3numjurul.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wmxgmolh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vpdykcew.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3egpqohqm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kwdabwop.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zjeaygtr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wvopdfuf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nkapqsub.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fwteuaxp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ykiuiles.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3huqakuci.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iagjhzvs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ugtvdato.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3tkgrqril.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhqrssty.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3knzgtkxy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrdthsk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dvkgicyn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvbhasgr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3awygscgb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wnsxathd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3oftiutss.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zekwbsnr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tipnwiun.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uptgytta.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vctmcczy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ozzzrlvl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ghovhowo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ryhvkhoc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zfplnldt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fkivvovq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pmdvxbsy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ujlftres.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3syqwyeus.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ahxfwacc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cmtlehtf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dmzgjtso.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3khcejupx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cpikjrow.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vyhboqdy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3eyvpnfbt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3funknbhe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3opsivzwt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3inmrkesb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vqkivkch.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wjqwlalm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3afapimdl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3turdkrdn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jmmtyijq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bbvmmvzm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qawimwny.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3awnizfbg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kkloreqt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vheqysie.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tjvvejje.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wuvnpxzj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3enmzmqao.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3crelhdvi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3izkbmmbd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yztijdoq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlqtkqjl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yehdqstn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3uazsvuin.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bmksguqa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kbafrbeh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amrimsrz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkmkscxk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vvryesur.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3onaoaeos.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qcsdavgv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbqjfzkc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ccwszhoh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3smbrretx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtkzwkat.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxvrtenc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uemsykyd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3uovwarlz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxdcbbyc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fzhutiqx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cdnyhnfa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gatrdojh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wksxmdvt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ycypsznz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vfvvafoq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mpsdpexz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vafjhvhh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ulzvexxx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3roejjolx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wqokrqwu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iocjdbcl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xkzaieyi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hblnzucu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ccbcjfch.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3exbkoguv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nrzbvtul.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3isqxnxnp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rqccfqut.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3oitzaxqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uupodqyi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tqjfucdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkvbluyr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yhuafvll.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3agzmnqiz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hgskldmv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zzkxladg.html


<!-- 参考信息 -->