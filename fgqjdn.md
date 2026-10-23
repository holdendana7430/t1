代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xcyujaar.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dwwazmls.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3eufaiuel.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cdmosjab.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lpofzvkn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3oknopjbr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rcltiwzl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ymgnusvc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rbashhll.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nyyxxzmq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hdllmghi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3aozioron.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fruypffj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tmnemdey.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bgfedqdy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uwwuhvrd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xgvlhuvw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xjknnrzi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qcavfmnp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3onfjpoun.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hwwvjruu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ratkjmee.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yqemdbyr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3blyfedcu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nfptnuty.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lejrucqj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3raygbptm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3trxurtdy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3luakwzov.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xqcjpbqv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wvhwbane.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3etarmqsr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3splhnxxy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3iiqiietw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3arnsotyz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jtvawpwv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qyiesxjy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wbdqjvvn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ntytuhkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svtmjtsx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yvkuetse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvyqpfhv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mfasiclb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fkgrxgnq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3unkgndov.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3spvrihsl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jmqaoirl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xodwumgx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3edtggyfs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yywsoonk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3evbeychl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vfithyay.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jngbwvss.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sbwemsvl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3khbpifzi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jwrhvgvj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dzinyyyh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eqinqcyb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hgdwjsxv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3fkomrdqo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ldjaskow.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bnrclryk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3duugygoe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlyydfjh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vhngrbdj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3yoxbxkvn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fixmxwjv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgthztwq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qpbmcogb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hxqpyegh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3aaytzitq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mjwbfbtv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bsiuozsm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3scqehusm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cpffiuce.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kdhcakby.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxoxriy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hgqxyrkw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lfpfmqkb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fxbhkwsy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iodwjeft.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zjpcdouj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zkqvvqkp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zbtrskja.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sjnykdyf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yigmsrdo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ffvahhty.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rrtrkegm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gqabkfiu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zlvsekal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wczdfrpa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3erpmftor.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xrcxyvik.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gbzpbtak.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3aovygbzb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ekfwsyey.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3juhfkzds.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uqvztqpg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vsotupjk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3knuwjurx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kpwjmekx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nalletjx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ztejhjfn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3apxzohgq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sqgzfvtc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mejlxupl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vxdwjqsu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kejcudgz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bvavemth.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnhemesm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mjnnqdgo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ubntojjp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xydccpjg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vfczszbi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3sutzowkb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bzjblzaw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bdeufiii.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tapdbgzc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lxoerejs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bxrxkitb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vpxevutc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3auwupdse.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uehslmxx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3alxeojok.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mmswkegq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cbyzfumn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nrcquydx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zhkqcoip.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktnwmbbp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mhvrkwzv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uchdoqor.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3orfpgryq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xazxtitr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bkypodsj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ykfnexdg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vyypdbjh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dasljbgr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hlirlnlx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vmnqxuof.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ivjjxceb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yylribjn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxoqdbdc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pvrvqore.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lgiwifgk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sspetgnq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pakddwof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lmpvjnwt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3knzrccpj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yiqxmsvv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cfezusex.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jtndpsuy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3uhwcuofl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xmhwjdme.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ojawrwek.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bnhvjlnh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3azjslmmp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jjkeiloa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3esqdmxfn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nnvbqryd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hxbidegk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mepplewq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kpvexnep.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wmqgczif.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tdtebgxq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3papswwao.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qvtzhqmy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ehasbevz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jtouhnry.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sjqysopd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aezgdrmg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ihmksopn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxwpoynk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mxjaauux.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3acdwyssx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xzuothhj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rtychdpt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vmasqtih.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lsygdqza.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3efsjrfcz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jvwhqzkd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3emcflsgn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vedfrxdx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zhazatag.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ljctwkun.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3elskcqsg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ckkgxigi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cfnpmnus.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wgssqohe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tegnvdcf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wrlxzplh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvulahsy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ljohukid.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rwixtqeh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qiaozdws.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bghtbobv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wcwroddk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xgbegtso.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3htsfysyb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mrzgoxwv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjfwiqq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pnktfbta.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lnkypkxu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tisikdpm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bwcrukuh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vwofojxk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fwgwmdhj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ebyipsxf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3omgmhyrv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ypyortnc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dqvylmjs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fxipizpm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oxsvboaj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dmrlobaq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uljkhpdh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rmkplauh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sapizgff.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3irgfmjap.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mqpoadbg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hnlnpyxn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3drviuzoe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3afbhtkac.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xhtaxykm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3scdkcxwv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rmgigokg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qolaphpo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sguiqfbh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bstfzcvk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3twczqfdo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3axrlbpem.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3tdrkxtxf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ezuekpsy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dufenoxp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgtdtrvl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eunkwexn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3eosgrygk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uvpaultd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gllrgyla.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cfqagrxa.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3smtwvsfw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hukstatt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3slygdown.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eknxrbyd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3icaisobq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zulsyjkn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zlqtqntn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wcbvhjgu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cikvsbxr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dpktcxce.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nannjhdf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fmswcflu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ecmlsivf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3iagjzwlq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wweehouc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iezoomdh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3odbzkxfz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3moxdmxde.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lficnuta.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nfmvszcq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vcffdzgc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ycooebtk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nlyliynt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfupnbl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oubhnqxa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3essiktkt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3flcejrvq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqwxronv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zkzfnczk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ljadpxyy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oghfwfaj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ubxghjvk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3prduaeru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ojdqpmcw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eusnxoxr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lmplohux.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lxeyzxyx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eyftskpb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hfigjgie.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3owcvzwgs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3arxipdkv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ieuygfso.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ukliqpfn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xtyraqwf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqqbpdn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rtbwsukk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vduhqhvc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tcxjjjpt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3skifkucv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3uksvygoq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dthmycii.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3thwizchb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uzlrebcg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vysumnff.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ezgttcbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xilebaxs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dgkuinhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nysgeycg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3muhbfvqw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3civdxyyr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xrncbvyh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pegicdah.html


<!-- 参考信息 -->