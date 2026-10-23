代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hzregshi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnkyskqa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nwmjihys.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nmajbgop.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wnsyhudj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wgzampmi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3icyyrnzv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vvititsh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ctjkzwyl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tfnsytnt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3baidbomp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bsfowprx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kqvkktkj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3itirbubq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fguwonor.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lvtnshqv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yrcdkvka.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wqqcangt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mmlbvorp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gvzggpbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3eqbtwnzl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ccvmjysy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rcwhyisg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3inhztobc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ofgylfjp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ndzbzjzh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cvkmsqlc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3drsrnzlf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zgmjszwn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3usxfvbop.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dgoiuntg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xrcgmrjw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gvywvyds.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gwnhpjop.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gbbjfiaj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fmkyjpcw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ewnkpbdk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3oksinfrw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yzzowknx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eixpghor.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jtqxpkbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szahzaqt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jxltxvtg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zloxyewf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yttllggx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nvkbzyls.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tvgyaodz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3sinsrora.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cqmdwlxe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iigdefdb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vfhsqqeo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wtowbppg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3aichutdj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdfybteu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3asronlbi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rswbeoeu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vtpbwxsz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tslaabua.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fscrgkne.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ptqcrxim.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hqflthji.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vajwwejw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nzjbhglp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gugfayku.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dvstghaw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xtnhgfgq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kealsmod.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3plrsmwrr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xaqlkegu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fyktmqxr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3utvmhkuv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bpuwubgc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jxbivxce.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zrxaqzty.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3adjakdny.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cdlusaep.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3icelwhmk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uriyespa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cqkqurpu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3esftnrtx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zftizael.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ipfiwvvw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cfliymrw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ohfighme.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3conhujhh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bbfzzciy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rnyplcfm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pnprekzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oedxgpoy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yzrzvjvg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bgpzqloa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hkmffjqi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3plttaipf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iyapxggk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvwhuza.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jwumxwki.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hdawozgp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ammknozx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rnzzfrbd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pznqwskz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jhjqhsoj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mkuchdzn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ojjfivik.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vfcueltc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jgornsql.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zthntqyp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3oervbbqp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kjykxjtb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dknyrvwo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dqxrctcp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrajuzas.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uemkyrfi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3swzboikd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqllttob.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3syckucyo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcagnbge.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dtuneibf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ljigpdse.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3msuqubnu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cvgbxbia.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sevnygyi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lvdcqncx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xqgbqfuy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3htfjsuaq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3srgiszfx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3kbdpmixj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dcgigois.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3knazxlcp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qjqoyhvr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xohpruac.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tojwwyki.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mihotfev.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3apiqqmyf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3uljncfxs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3czpcxbhr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gxuqqpcf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eooewlzn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3oaijacao.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tomitjzq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhwddqvw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jspdmuuv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyetkkil.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3acvgatsj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dqnjscmq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3givehjyc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3megjddmx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rtoezvmd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gicgjbuv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eeundnjq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hsehamxv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kqordhsu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wtlokvhx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbtblsz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vrazinfe.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kqwslkvt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3exrurvbr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jbdjkabn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lgtabvuz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwwenmee.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ghlftrvw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3djzvusnp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ywvcvnlj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zjlenwlv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3onmrxuto.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pzchpeso.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3peddsmzk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3evrsyvdb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zoixafun.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xnxezymd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enubkyno.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cngvslnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nohnbuma.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cqnccjth.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ngircati.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fnqnehdp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nvljcwhd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qdtoiscm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qldmcvxg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ilwebozp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vqxyvfiu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vkjpgsus.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xbjhydkm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vqpjgllg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlildqiq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3omaymhjn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dcsuensh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hzdvhtbo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3swoentio.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3txutkiog.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nzbowfxp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nscwnejv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jnqysvtq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wirwwcon.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3foggbfnj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kfivbosm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hunpdjxs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pkjbqmlr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3buqnaisd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ibuzbtlr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtbthzu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bgnkcwyq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qxbbqeri.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dqsiawyx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wanqroyj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bnpthgjs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfadxmwy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qynsistp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3askxwqgf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fcszcnbw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sewmpclh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mskfykxa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pgyytjty.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cqiqsucg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xiwbnyow.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oodndbrj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aanjdtfi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yvbtzmki.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3idlqthza.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zfmxdpet.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3auherxfg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nwjcftsj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3czueosfa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oijxfcjl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rtlmfhch.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hbkpmqex.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wxcfoxev.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3iqbsyrgc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lfymvdtk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xcdqymiw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ecuqsecd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tihcztbr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sluclzyj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rlbdjlxi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ozpjnwmo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ovtlzpxo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rztnhvlp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ficvsfux.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jdnutisr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ctelyqtm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3iqthmqbg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3anrgnbuo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fnitzwss.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ssvkefmw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ncnwntwm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ygqisjcm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gdydbmxb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eifkcfka.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3csdxtpmg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qezwceul.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yvhjpdmq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mjztjtfl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zxtzdxiw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kjpjdxns.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bppfoqtr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kfdzdavw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fwbqjdla.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3crpltgrv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hwomazzo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zotimnje.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dsqenizk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mehcsges.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzdjjjxi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3iduzjafe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3oqqnaiwt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3uvjmuvbn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bhcmlvrx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mpogftbn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tcxqgpbu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fozqlqgk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3crdzbsqf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yeavaepb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sxchyzki.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffxbcbxa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3smpurmaq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3svcpvjha.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3klvxjzdh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbgprtmj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gjxygpno.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iviipzoz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3prglfxwe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhyvliyk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wxowueyu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ajuofpha.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mesfjghi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lapwncqu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3spclihtq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jcbwmojg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mqitwxvr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3geaagcnf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gcqvugeh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nextbeax.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rhxuhptk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3soeuifkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxulsfnt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htoghamf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwujtosz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qxyxsvyo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ijskiriq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qdutjpbs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xmygmoyt.html


<!-- 参考信息 -->