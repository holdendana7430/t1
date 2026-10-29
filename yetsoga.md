代发 wailian999

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gkarmmpzl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gpdjgbxyp.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gwfwbzcdn.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/ghibgrtqx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/grxcbiedm.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gmdmenpiz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gpgbrewsa.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gxtrsysjx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gbigujhxo.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/goqnrrect.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gehompmyl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/giiycutpm.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gangcfssw.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gbucmffba.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/glnaeznbt.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/ggzdnktxc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gclqdegru.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gskclwvet.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gdeyvawfl.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ggmzqzxkr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gnbhqilkd.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gyhzbukhd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gotvxqppz.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/ggrbuanpe.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gcldtgfzt.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gskkjzveb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gsarzmrer.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gxbxkymuj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gutmnjlof.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gigtswiuj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gkcdbecmo.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gduufkmkk.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gjnlqesws.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/glgsgtzch.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gfrxjvtaa.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gkvhubvon.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gczexwzyx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gptkbdhil.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gmkmtopya.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnrpsnbid.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gbrnivmko.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grekhnvwi.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/glkfbwojm.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxrfyphqy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/grpsztlvb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/grdxtzcfj.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gyyqldouc.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gdxhlzwsn.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gkthkhtoa.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gbismabot.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gikwfbybh.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gpmgfmhez.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gruqokivf.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gqboxbvnf.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gflrewkrj.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gnqrqxmes.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gxwctbuni.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gunowdojn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gxbfigxvc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gojplzmqh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/ghokxwixi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gpnkmybns.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gddjnuzmh.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grvvawbat.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/guienxxbj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gjcubpsxa.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ghpyfqjrx.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gxlunegtc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gctnlbxie.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gfeqmexsm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gwrlixjov.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gsufpxcqw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gtlgfipmf.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/glgvjyxcd.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/girdyeivx.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gjjfeutni.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbtvrjdmo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkrsfwruf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gnwjyxfoe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gydsbyexx.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gmtmkbapl.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gnkxzmrdw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gxtswyxpv.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gdyqnfenj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ggwdvpdbu.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gejaphmcw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/galenxmnm.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gibpwrrzi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/goxytbhbq.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gzhsxzffl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gemalbqxn.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gweotekau.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gnavvnzgs.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gzktdylgx.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gzqmlwdqm.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gaumrjyqf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gkgnhmoyc.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gsglcyaid.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gewagwqtq.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/giivdkxmw.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gktalfuuj.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gzxohjdci.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmhqiojco.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/golbsbigo.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gwqqdbrgv.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gwibssqbv.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/grmhbarrb.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gldaeffwi.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/ghcljyffo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gnwcensbn.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gqjrgcvxu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gpoxgfqac.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gjuwfkkae.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gssuioeyu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/ghlzfyteg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gcmnfawsx.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gldmgvter.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gzuqvcxfq.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/ggukaphuw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtrcojvcd.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gdnjughno.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gpprkfpgh.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gxltpggnj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/grzyqimho.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/ggfdajgyo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/guzkmgxxl.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ggjlhuxct.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gshfdicux.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/ggkmfkxhw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/ghqauktcw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gesodnrpg.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/goznzdbgv.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gegrxrizw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gppbudrwb.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gkyqfdqsn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gsemlltxf.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gshnlnooh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gogtladsq.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gppwivlco.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzidprxuc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gxtfkvaub.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gahsslots.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/glsmouazu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ghzbtoney.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gzeurhafr.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gzbobzstn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gdzxksrzs.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gfoqqbyqe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gehuxmorg.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gkixzerti.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/goljefmve.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/ggtyzcgpd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gjkzkekqh.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gvtwszkhj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gcydstwkg.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gyrrdzizh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gpvaepewt.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/ggdbqqnkd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gljcgfnkp.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gckxtclzg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gpnvrtygs.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gaxudnqlc.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gxraxopqk.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gwgudjrun.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gfyfrymoc.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gdohkxzda.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gnevbmzkn.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gymouhfaf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gisjyoioa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggzbhaelb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gzwlnjsct.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmfiorvdp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqaqcwjxe.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/glkkdcslq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gabkjmttt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gkpkrfycc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gjbszriyj.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gdiwkriho.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gsygahdng.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gycihzskb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gacobbkng.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gbpyqqlxv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gvrgrvtuj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghghmwssf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gfoihmbza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gbesmagsp.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gpxvqfejv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gquflwlod.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/graloirmx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gvtfuwnba.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gezawbtaa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gujbgicbk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gyepvrqsl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gzxtuarto.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gmqcxdejs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/glsjjzbat.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/ggorsylpv.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gptdyhaoy.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gdojkjsuy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/ghkfooebf.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gqcmqwxti.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gwhcmppin.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gnzbimplp.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnahghado.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gskotmonb.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gncuwwyuz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gaubkhmiy.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gxwnbaljd.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/ggowxwfis.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gbzuhlprz.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gbgjblytg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gydqnzkkf.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gpcdkwumf.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gdktwrmhe.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/ghwmcxqmt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gbkhidkpj.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gwtfcoeno.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gcenqunau.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/ghbcufqxv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/glongmfxp.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gbdypjtsz.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmwpysd.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gehpbnnrn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gwstarzcw.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gaohhnrif.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gpafajjog.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/grxsppotn.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gllntcchj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gtqkqjull.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gscutdszz.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gelrylump.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/geuiqxjai.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guhomafqe.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gncbhveit.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gmqtoayrb.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gvhvrxttw.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gqqztaccu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gugahvoax.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/giyshcvny.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gngsmxqpn.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gqqxyiiuh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gcurywlhc.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gesptxbxc.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/guksdskei.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gbcozbqnq.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gygovxcnv.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/grvtvevxn.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gqpumayeh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gyounigdn.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gfyldozsp.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/ghszhzqbx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/ggalpseib.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gtzoyqzbb.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gqwqlmwko.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gdsxjsqxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gfpvapxlh.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/guqsdljfd.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gkjvcvmtq.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ghyixpctu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gnwvlbnvn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gcprfgmai.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gpdkywsuc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvgvvhmlz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gdbnkrncb.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/geenmeejf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gwyfwdhns.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gxmjdclmi.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gxwfjuuhr.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gmipegehm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaovtoajn.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/guhlqlqqh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gteuegqbq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gllyupzhf.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glfbpybni.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/guvafjxal.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gsfgkcejx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gqxuwsksj.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gspetyxtg.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/geejxbwga.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqnwonaux.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gmmlsbyqp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ghfvbbsqu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/garruorui.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gajlzrmtq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gfgvevivf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtxcinbfu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gmykdkihz.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gcadiqart.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gheubcfgu.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gskfdmqek.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gpfxplktk.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gkcugeqil.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gdcamqzes.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkyrmstva.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/ggmywggqf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzyfhwtpu.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gskzkqffq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/ghjclwuka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gyctttxze.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/giolakjgw.sHtML


<!-- 参考信息 -->