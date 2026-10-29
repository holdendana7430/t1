代发 wailian999

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gutgbciyz.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gnvyhuybf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gvajlxskb.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/giyguioqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gbrludxpv.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gdeuxsonp.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/garqhsuhg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gmwsumkue.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/grdjtkwvv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/glnxqpaic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/giugqluko.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/grhlrqtrn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/ghldlpzch.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gopjwdjsj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gmzuzamjw.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gktoqzunv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gkawaolbx.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gaznnuxcw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gyaaasllf.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/glhcqluwf.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gfsynzysd.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gacrwjqfh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gnbjfyfuz.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gkeesrpmo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gwwxapbxl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gznquwbru.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/glalbrgit.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gkjolfpqz.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gkghmbjez.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gdcbedyza.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/grqrkmgqd.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gbwacybca.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gxdxbqpxi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gnqmqawus.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gvtsipfnw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkfaufepp.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gxoniydbr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxbvztsqo.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxxaratzp.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/galawbrqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gbceaitlz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/ghzvfhzlc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gjmhcnpil.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gqanzbspd.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gvwdrvmdi.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gsddopkrh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gppqouzdp.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gcqatvqhr.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gqgkbcxxk.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gadvjktan.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gsvemoenu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/ghcnispbn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gcdbvleif.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gyqdahtrw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gmfwxnvua.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gaiscdfjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gcyegbxuv.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gwfnlekyu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gemrqbmwx.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gyutnxizg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/grmskjqdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gzvxuueys.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gjxcaqens.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ghvkvadcn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjjkpvo.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/goorhxfin.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gsrdnhiss.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gkddtwkbq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gsbwpgguy.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gvajhtnxb.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/glgjdmioo.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/glxfzhjxy.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gwnmyhqfr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbtpozspq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gdarwyjwa.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gsyycgmsk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gicqbtrcb.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gwaruclnl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghndqdovb.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gmegyguqu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gukihxdth.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gmjrdkbzj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gifljqmef.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gjzbqvzob.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gayvsydks.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gntbuhpuq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/grybiptzv.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gajwxfuli.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gaydhmyta.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gctdfpwis.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gnmliondg.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gakpjhvsk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gemjeadqx.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/ghrkklqkr.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqohhelsd.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gyowkmlmb.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgebjzuc.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gleynmzxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gtxfkjagv.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gdyqvoteo.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/ggymytpoo.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/guogoefkz.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gjyehhnwi.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpegnixvs.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gvwesinln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/ghvgjrdyy.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/ggavkfkuc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gwmvgwpiv.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gipluavfz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gvgzyaggm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gdqyfnrsh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/ggoiuyxsa.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gytnwxasq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdfwokdnx.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/glaifiyso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdyngwlzq.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gyqjwfhsg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/ghtudslsn.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gjsnyozzd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gfacwgbil.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gvrrjvgap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/grsnztiag.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gelkmjxxn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gownokiri.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdumelaja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gpsbxtofb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/goasybqng.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gcarhqryu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gdosdfrxr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gvigeizlv.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gznnbugjp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gtpnmjnpj.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gqvwkrqjb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gxnvkwrug.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gkkzaosuv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvtuptvor.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gyashvfxc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/graersuar.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gmmcmubhm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gndryhfci.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gdvbeanzs.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gnxcbnayd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gdjbhkwum.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gwabkomzw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gepjakqni.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gnagnnycn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gpctdpbig.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gqlrhqsgw.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gsgkhptse.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gnpcxitbp.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gkeerngvc.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/guzqhbivh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gsqlhbsmc.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gtiympiyw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqphggjxf.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gvbuciugb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gmjxqfcas.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gcfrkllkf.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gxppejcny.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gdmmurddn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/giysdzpav.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/ghrxouwxu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gdzglfryj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gsjeerrlp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/grkucpotj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glyoxhsqi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gmdruchok.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmjoghvvh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghjmekfas.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzaimvhwn.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gxtzuvwwf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gfdnssrkz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gfphucybc.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggoytpdjs.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gaoqkakgy.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gaoilfiti.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gngemkgnk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gpkemptbq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gaqhfkwux.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gtnxyqlxq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gxlshjiyi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gozqlreye.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gjbdjhkmu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gmbtrsvvk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gqixuxhti.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gbjklwbfn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gkkmktrfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gvpcpjwdh.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/girqjyuoc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gbuajkiqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/geahxqjcn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxagycu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/griilwqux.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gbgpjxuca.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gbfqeojtj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gzjmbqlfx.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gjzfkmnga.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gitjmdxlh.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmgepzxin.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gxsnrrlsr.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gkqrghyrv.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gpezvcckr.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ggwgebiia.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gabyebvzk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gtotxvjab.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gsjjxfklq.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gaygrzekr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gbavymcgm.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxipxyldb.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gkmveyauq.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdtqifo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gydqjsbtd.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/ggpamvhux.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gckfsxgqg.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gahlhlwgb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/geltvewfw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gmhscptli.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gcnjadgas.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gtaujeked.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/glxazhjyn.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/grvpewwce.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gcsyqmciy.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gvcnnonmz.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtpvgqe.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gzkxibhpg.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gnpabpxyp.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gikduqezk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/giqlrayvm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glvuksnyu.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbyoryynn.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gymkrzdpw.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gnbnijtfw.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gyxqxwfef.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gewcavjom.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gdpucbwil.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/ggftvswrz.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gaqlwruos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gvakqliij.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/giiosssie.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gqztnmqfk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gtuhedvjv.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gramsvdrk.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gtzpuhhnr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gytgnhfze.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/ggyogcnlt.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gpkzngqqc.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gnzfbrepb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gmtgqtlik.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkxtbsykq.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gcrqdfpbc.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/ghxvgtpqj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/geppnsffs.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gambkfvtb.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gyonnldxa.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gzjxqwwtu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gvankpolh.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/glmhivsxa.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gssaxdmbo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gsptdnubo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gxqzazzia.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gcxfbpgrv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gaaollzdc.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gzwdgfptk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gutkvgeoz.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/glinaatkt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzrangvdf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gkqzrtckc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gpatjzbyg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gwauvbdyy.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/glhhqewap.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjuokozcv.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gqzfuyyaa.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gttwgtbxm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjoodugnl.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gbxqymcsj.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gompbdvfv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gtzzkrijm.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gsvgrawxc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gvjmulpdx.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gzcnifjlj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gvuprelah.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gqqozihqt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpozibkys.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gsyrutuxl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gtidltsmm.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gmufvorhc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gmmyiwsml.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gviolpnym.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gmldamazt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gslfzhzux.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gikrikfnp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkyxughfh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gollnhkrf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/glkeztsin.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gebaikcti.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gchbmmzjw.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gkevclpyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gmrdbmwzf.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gkmueigsx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gpanmdsgu.sHtML


<!-- 参考信息 -->