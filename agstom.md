代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ubshiemb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pgethrbe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gurxhduz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dsvpeluj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3aduavklk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3happrhkp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3betfrijd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ncjivykp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3axjlarrh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3navfhpcq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ofdcokya.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lwdphceu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3iefhjxdq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hfqpeqxz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dipogoab.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ykgzaitt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mbhwzgzm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qfgzxjxh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgupvlzd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ifugsaut.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jgsmxomy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mtuydzjj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zdoohzum.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3eayykghb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vcfuwubm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xceodnyz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3anbfeohv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vknbcmjh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xmionpvl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ikyopgod.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kummjxyr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ghuwywwx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vmepvwhm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xkbotnkr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rzayoovh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3frsfbrke.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yyzfkxca.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3verccadu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3umjydegi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3isttjndd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hlnsyfuw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bsrjqvmf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3cszpqmnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzwzledz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ssabokep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snxalxec.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlnihpyx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rmwmzqkd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3cjiitcav.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jazfzczy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ksejegob.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hpwcuzyr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3avoynwuj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fgvpmvwb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jqpwmodn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmehqnyw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpetdagc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3joykjzyf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dtwubykr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mhiglgjd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kqpsxyls.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iojijefv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tzxnblzw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3luqrizlm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jwperclq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jnrgvdgt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ybzewtos.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3etszplpe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ivohnlij.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zzfaukmq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pzrrwngz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pewaadhb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nbzfcuab.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3peolyuyl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fshfimto.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3otbqwsri.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gxyjicfd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3anlrarsn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sdgeismv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwduak.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrvwomzw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxrjaeua.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tymipctp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lluadqvv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mcbfecgj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ljypibfy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cmqxkhmf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hlaxefkz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bosyivsa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tsaqyllu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tsdvbpyf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ekpurzyb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mtcymxun.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3krtnooxv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3baedjrib.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hnbjzsbo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yeybjtoq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hdwsrlxu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xbdmkvwu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wymulesf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sqfvdjoy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fustmrxy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iofszzwt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ajptdtki.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hrlhxdth.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3edccogrr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kwbujmup.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iaqlabku.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xjdufoso.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qysgruux.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ggkspshf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3giuoquiz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lxwhjyty.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3whtfmfyi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3awarggfq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tdgvyhsy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fugrlpvy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ybzhcyux.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3grrjcvdb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3uldzentv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3daaolcii.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ybvdxeys.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3eueztmce.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibcorlye.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xqpyugot.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3erldcepy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fxenmofc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sskgebfn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3miygvdsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tqwnjzji.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vatlzzdd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vqedoshh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpofiiow.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3otkrytug.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vddbpncr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cmahpnyq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fdzivnhc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eoosomym.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hparpqyb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mselniez.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ydvfykno.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yxoerraj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mjbmbopw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wrtapeso.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rwanafpy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3izvhcjoa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jokwiwgv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gplghbim.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bhkkdzkq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xiedlzti.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gmibozsi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tjxudkrq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pwuscqdw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3khamqynm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rnoslpvv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pdqleflx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wrezowbn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3torpxsns.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sitdcbmb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xsgpbsgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ahcsiadc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cdygjtdo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yznzgfyl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ykjmbkez.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ljqtejbg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3guvfnbyy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nvbvbifv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rntcotmj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yhpfizlx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3txygnurp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bxamtncr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kubioiib.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zwbevikj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3infmamgo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qhfjgwxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmlabzai.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mkawvaqo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rgdnxlrd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyapybel.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3obudpcmg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tscktwpn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dmxiiark.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pubqdbqo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjpwmrsa.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3aqseefos.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ievvfsfi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3toiykntd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yyaxqjzx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bncwncjo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkgzxfhb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ptxacqxc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vxcvkbgq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ewuklxoe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ibbyfgfu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3btgfhutr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3acjbjhoa.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jeobrguk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fxujpetu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xwfrpvkw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjxknfh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xnqwiycd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fecgexcl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pjvijylq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3agpvgcet.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vsopsiah.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lqygqhmg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zkwfwgvs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omvkyepf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dlqadnlp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wnciguok.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xukqwvne.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zwclsrsn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lrxnlxsb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3leduhnml.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qmsvkibm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvpzini.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hlndiyul.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ufaowfjv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mzhswfkv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sfoffwuy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzjaoacy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dkfsaqjh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3aextanmi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltemsczm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xvhvbnod.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3glyrxlco.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ncpmmlip.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ndbdygpz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hwdcewer.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ruohiuci.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vbelshwh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ttakhfud.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pfnbwlsd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bsimtxgw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cdylfkne.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vcerkfvh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvhgycpu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qujxfwku.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3etprgknj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nacjlwzv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cooveoql.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hgopiqpn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mqxtpwzu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jmqxzcdx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ouktjoha.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dclangoa.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3iecohvzd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3phyespos.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3amijoboh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3osrfnkbz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hzmxeety.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wdqmqrmk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tzovgsrq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qwyltqdk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3boeglpdz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jqlxkjnb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lmcolubq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3eakvvajr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gbncidgp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ovyquzwn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3klytweuh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3oubgvurg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tjemvbyt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wznodaho.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ztpqfdqz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnsefuiz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tfakdsni.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ivtannwx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3iisgijzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3yqqdkzzn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xurdjjxu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wwuhbhms.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gqljqfeu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gvjranan.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gksflmno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fkanjcsc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lmnwmpqq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jqgnjtqu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bmiigevv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3axwcvplq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ezwesqir.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ojvnxznu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lmnjzeyq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uqbejghw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3slslhrgd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vfcqghcc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzijsddj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nuzcsjns.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fxyalgcx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eldoxzyk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yiaztbsn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3schyfqqo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ugtovckk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jagqkeie.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jzlrpdse.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xegvafzc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlehtug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obsdbsqc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zmqnidgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nujgtief.html


<!-- 参考信息 -->