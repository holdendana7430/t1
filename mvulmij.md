代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gdfhnpluc.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gqmjehjgn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gooynfvax.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gaexrvspd.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gdbintolr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gmfmqltbh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gqnifcbze.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gdszwmddd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/ghjgrboup.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gfxedileu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/giwonaujh.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gniubzrxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/glxzdmawv.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gbklgvhwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvaehpzpm.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gvkixmrdp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gapfgduvy.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/ghbpxdvxd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gmltwrsvh.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gdstslent.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gmtkifczb.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/guagaufza.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gbkuhrlzh.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gannkglld.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gaxcfcwrd.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gityzpnma.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/glsgyzhiu.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/giwpjqqny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/grenaoxqb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/ghqecpnim.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gckomqrpj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghtjipotv.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gjugdceyg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gndbzegmu.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjknmcngv.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gsowznyej.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gheofazvz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gusafitwa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gudgnindu.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/guzsuxbzl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gcuijpiwj.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gmkanzpql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gyhikvbcr.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gideujieb.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gewdfghjl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gzjnkjdnx.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gtrdklmtu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gtppiqapi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gyywdtnrk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gqxmhxtqq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gaelsgobb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gveecfmyv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gykrfrzgp.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gnlbpirfz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gkspxttci.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/guekvgkuj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/golcrxcfu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gbjobwtpg.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gicykdntt.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/grafioypz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdeokkpjk.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/geizkegzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gswdcfkqr.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gxbvalhhq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggwcqjjfa.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gmfbrfsmv.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gobyhdpid.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/ghsnwbdeb.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gsmcnjndn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gasxomxsf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gkwbfkupr.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/glkkmtcnx.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gstbbzoly.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/ghrfnuuiy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gubpgatvg.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/grzrorevn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gnusrpjae.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gnjpiosgx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gggnsclcl.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gwyqfkyau.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gruhaquck.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/ghcyxchkg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gnhatuxsx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gfdgansgc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/ghygvlkga.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/giznlqxdg.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gucalgrgl.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gjyzehnjh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gavjtjfva.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gumabjeqy.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkzzayvau.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ghanuqina.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gcbaveejk.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/guddyfosk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/guzgdzupe.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/geaxppjrh.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gjinjffso.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gzvslhxqz.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gecrsntbd.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwnnjybij.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gdetjkoft.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gdcqgavoa.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gzlxstpxy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gxjthifkg.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gpaoqdyjb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gwndankcg.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gsgyzbtkd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gcmpzggrq.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gkhozkchs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtjavlwze.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gsztnqgfj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/glzdluamq.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gqivwkuhl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ghhxnnyof.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gcmrdciyq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gmxdzqtig.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gmwewweil.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/ghbxpjcdn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gykzbrqje.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/guzpoamem.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gpnevvwqk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gvzqcsdkc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbihsodcd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ghlrkbxao.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gmoiazsnn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gxopwehza.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gnwgdsopi.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gwhcqaoff.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gspxqrvku.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gsxgebzik.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gjswnacxg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gsikrjmdd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gwbacwnjz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gjfvkqwhi.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwwwemvvl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gbwofmfgr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gxksjkhua.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gdwnckryi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/grcbckyny.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/ggwuwmquo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gzmyxzgbb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gcczyqqdm.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gevrmlzfz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/goeoqzbtb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/geuuotorb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gnllegtpi.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gijmjilfd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gxtsrayws.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gakaqrdld.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gqmgidqvx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gnvvrznpl.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gahdtbito.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gpteitfba.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gygvbggyr.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/glsggwgfw.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gptkqmezd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfaxokccp.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gdmqahdzr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gurfirfch.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gvelqatye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gqmzbpzqn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzjwmkquq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gdwxyfygx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gytkzrhdh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghdsmodwl.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gycczowlq.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gdmknzqex.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gqdmuspaa.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gsoscrgor.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gjotaapyn.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gilbsxcly.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gqgdvrokp.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gogazbgkd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gagpszapn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gxnfuvytu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gqomqixnm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gbuhvdndu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gjwofhhen.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gvawedrnj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gdlnajxah.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gppteipvi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gnaodyhuj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/ggrhujjea.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gafigisxa.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gpeovyxxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gicsjucxz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/genpxcolq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyadaaztt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdchjthkh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gyywzhgck.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gavdbbqca.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/grbrayasc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gyvylfqmj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gbfcwkbme.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gawgnrhxv.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gqypoimrx.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/ghndasxwy.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghbydznkc.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtaqmzgqc.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gmmqzocbw.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gzsziekom.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gyfsyjkxs.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/ggnnvuzil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gvnnblyvq.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gwpllufjv.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gaqagfkzk.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gyayekeub.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gasxeprzz.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gbjnibowf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gyhaahmve.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gpvoacsqa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gdrbkmtym.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/guvabpvjm.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gaivkbgvf.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gfzhwmluf.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gtmbiimvy.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gnkhszqvc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gimmlohhi.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gtezmwplx.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gdwkeixfj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqdoyuhhj.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gpauqnahb.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gyrjcpbtn.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gazqzcsvt.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gyfjxsbxm.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gescdvdea.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gyzysfwoj.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gxkkyzzku.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gzkhkdoxs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/ggdynbpez.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/geksujzac.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gyjnlewyr.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gblitokmg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gtcicrhyp.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gmqrxwbid.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gklsqpcfb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/glzgafrnk.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/giiznlqal.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gzjgvtlkh.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/guyippcrb.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gugnnynvx.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gpozquokk.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/ggtzcudkg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gpcjcapax.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbijyqipl.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gfojtmwki.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gimqerxjg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gmjpcxzqv.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxstbatrj.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gppeotcaf.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gibqppqac.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gpisrsrue.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/glxzweqon.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/grzitcndr.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/ghohomujq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gblohddgw.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gazspwvlh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gzvgpuhjw.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/guensrzhn.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/grqdgmoei.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/giuruotcr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubsvgkpn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqcveqlfj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/glfvxzhpw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gavhhnrpf.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gulmvjccv.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/glgycksej.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gswlelehx.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/glsktikag.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gnbwaihkg.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gbwldwwxl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gusooleas.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gliqlgzfn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gevkhmiuu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gsxuuctpl.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gusqmvzow.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/goadgfoso.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gymyubpav.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gywrukybk.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/ghprzqdjl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gmwjfppuk.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gvzcluuvz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzleizu.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gmjnbyngf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gkrhsstdx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghyyioikh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjuuvtj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqpxmxezq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gmgcqhcik.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gcbxdsokn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/godbwhgyo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gfejapfwo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gjftldixu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gloczwxed.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gianlwqfe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/goyqvjqwm.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/guvbuvlft.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gakwyrmou.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gppwhbmva.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gcuyethdv.sHtML


<!-- 参考信息 -->