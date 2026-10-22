代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jbobmecj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ucstubhk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2iwdlrxei.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rtkjvsme.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pjwgurra.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2thexxiqa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bicpqgfx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dfbvzwns.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2noymfdky.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2cwighdjp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2cewnxbgu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rsemhxhg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uvmglssn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qximjele.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2dmunvgud.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ddjbbhvv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hzddyrgx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pkhbftds.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhaljmfq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hecbnwss.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jspwbdfo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cmumolnu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jnkxnahq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2suigfraw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yveiglth.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rarxyunh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rmexvyjh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2etcnhqdv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nlvzotfp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ehmxoujk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zgrcbddv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vvizhulg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mymqmoke.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pfdqnwif.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mdgxfmmt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2viofycvc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2edusvbjc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kptpzizc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2egiracaf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vcrumqpq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hkykgqjy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ppybmgwo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ruerkzeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbotbxpt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pldybzoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohwffuzf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ofuplebk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vndbumdo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fngtkozz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tgezamhh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hoyaylcd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hhgfsdbs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ookbaopp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2musmcykj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gfzvgekj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eepakkvp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ynektuzi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbaqgtvt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lejplwpi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2awzqugfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uzrswzph.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cgjpbocn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xhpggtxl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rkmyfsil.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2datuikkh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fnkpsipu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vjffqzhp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwxbmlul.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2yocbsrup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2drwizqlb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mvjhkgpp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jthfeijo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eqxzkmbd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bzjjlvoq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ztybtnmd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kpxvnfej.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jnsibnmy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tgmmxvmb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vmmcrufy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rmjzxrjs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xzpqfbff.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oehoelrs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ddzjcafl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zbximpgt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qwrnilre.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2orlohjjy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rogidfwf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fpcezozv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qreekhic.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2oorlrzlf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fmpxualf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2plerifao.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2seepsegy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dhlgvpwh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zzwwifvp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ignrejsp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2eiqhfyet.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lqmyxygt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2owegoxhx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vyuoezfh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdsnize.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2sbsiaugf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2brualadv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nbxhdist.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2alklmmun.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zooxtzor.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wrsagckv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jlscyklz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rxwudzda.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tvugrpmu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uqwvwose.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2woiuuier.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ngposasi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbodqlcw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wyzfxggo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fdwzfxzg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lvqjyurx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qsxihdjk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uarsjgma.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rbxdkcds.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zketonfq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqqwgoxb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fhcuvbxo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nofvhoeu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dduophwx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xdvjhqib.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hwpgslaj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ilgoihpn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pmnxtbcs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kjmzaerr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2laknfopx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ukhzmzum.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sifhmbmy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2blnlzlnh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2whiekyus.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ppergvqn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2essemvzp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wgfdbovd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gcwhseyh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nkmnoata.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qymhqksx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fmlibmxx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ypflmmex.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tynnnyqf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2smtrkwdt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ocugumgc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfampcsb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2iimhypki.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vsjhneyd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2truwskkg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eknoqzdn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wzmyunaj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mdsztwnf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cdvjvxhj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2osesjdlz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aopkalae.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xekeygjo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rjqqamjf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2htfiaggp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lzgqrrpx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwbqayz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nisajjby.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2layxedvd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2llcomnch.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddfhjxmz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lhddvenb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lghfkfim.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uofftrok.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qjlzckjr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ucfymmtm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uolmsxxe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jyuugdsg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fiaedmsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfecheup.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bynqnlkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iofsinzk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2todnvtgr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nxtmobgc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fanasikm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dwhdublu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kehqqipc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fhuudfyk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zeslxlbd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kglqoawk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2omkoexsm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ykwygeow.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cuyyfkuy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpcwiuu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tvbuvixs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhpukng.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2syudueuw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iwtutwxl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cwfzafhh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lmrrssbc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqhtihum.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uvmwgvxq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jgxttumi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lqpjqxji.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bvxhdusk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fpcjqxys.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2akntnbet.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dqueseqb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uscmrnem.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pxljxruj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pinldlad.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2suettuwm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbzreiyr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cbyolijv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mkbtnyrt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uzvfsyrq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kxavjyqe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cyukgxcj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kzqjabfb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvfdcjvo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2flaxlycy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sslbgwio.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbohmvye.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2haabiefv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xvmobnpj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cizjllpx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dukgdcoz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2glhuhfip.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2njzdctnu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2imiugnfn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rehfdtch.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ksjgsfti.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fpukjcgl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aowrfsel.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uhzqydds.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zfealcph.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tlxhtvsw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vggyyito.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nkdnfcbx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ltaiizgt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lsnolnwm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwesclk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cuzaxpon.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kbadzfiw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2lnmbsytz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2woxwgvra.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2isqbwecn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zgjwecgd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2czkbosja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fnuvlolh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bceiikjt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iwlxtqkv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2diybbdto.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bdqieupb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iqfmdfxg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lciantes.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wjpjoqtt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2obfkuhmc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bbijhtuw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vlqxpowa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2dhjumooe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2sxfcylpj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kkqvhptc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nsjvjbxs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhbcoauz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mswpeplk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wsdodvxv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2oiqzphnz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yrbzwzdo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfdlwyuq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mepjyori.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffjowzud.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bmpakhxd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2cphoebdt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lklhbtpr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgclwpmh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2klxfyhnz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2osjwptao.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljtwrivs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jkiqbyet.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vsxcprjw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zfoxjnqc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ppuoygjh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wittsaqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fklxnyam.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qorahdon.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2opcoyhgg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2voqiycas.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jrwwbadg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2elykxxxi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ijfffmmb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uvdxvcwj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeoweaqe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ofqcgezs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gzramrxf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fqkvepfy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfdtec.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xatrmakj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovixkuxs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fwwebxba.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wqgzpbdf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hglgaazr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2koxfdtva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfqkgkip.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nidsxkzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skdbrrpu.html


<!-- 参考信息 -->