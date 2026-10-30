代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gtdpccoka.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/grcibtqla.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/ggwqumqop.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gacutmuoa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gazoqsxkj.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gsxdorbrm.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gqocqmkfr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gkwhjnsxn.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gxentbztb.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gntjsiybk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gclhdzveg.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gerqoxobk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gsnkigohf.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gsrkljdph.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gloqwymwd.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gvoqeyhud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gnjubzqzx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gncvweioj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gdxldpmyh.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gdmqmobui.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/glojzgzmp.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gmyqdlqlo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gesunifkn.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gplcxqrpx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gnkogtcva.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gutddqxjy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gajlpgahx.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/giasglxap.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gbgkersna.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gqxnqtpcx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/glztogcmi.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gjaqtijxg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gmsidqyyx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gwgiryezs.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gbrphdfvm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmrphywqq.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gcufksskm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcfcpudms.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/glvbilvzb.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gbeuwznwc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gtpitcfic.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gojqujpwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gqqfsmfes.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gshbppzsm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/geqdrsist.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/ghcevdzdl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/ggcxhmrui.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gejoakthn.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gemuijcsy.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvirwckpc.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gsbjvagig.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gbosxjssg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gtnposkaj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/ghmgzbwqx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gohxgkzea.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gkmidscux.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gifapvvgd.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gcmihacai.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gepipzqex.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gahclikfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gtlzjwjmu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gqgfjmyvo.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gkdfuubmc.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gtyhqkins.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gesfxrhou.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/glnnsiypg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gacbneuoe.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/guseiyoxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gbtniinmi.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gpqmjmwjx.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gkwnzlzau.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gzleyijxn.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gkbflagnm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gbulwlfsr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gdbkymqqn.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gxplvhopj.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gwwdpbbic.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gkdnvexxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqkabsdcw.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/grpmrwvsl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gioxtaubn.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gqskpaqbb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/guojccopb.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/grdyijaqy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gyfcjusyy.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gzumggiyt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/grwteqryx.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gzljyqqwc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gkboxxuwv.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gielhwdxp.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/glgqkcqjk.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ginimliwi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gsrrlhdin.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gktvfbidg.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggwshlywp.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gxvipduwz.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gbayexzeg.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gtuahsxin.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gaoxxjkgn.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/guqdgauwf.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gbiemwoli.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gqgkokvwz.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gbwksvxmi.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gshpzvjlb.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gfsyxcywn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ginrikpwi.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gxexqrscb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gdemkpucw.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gwnkgyomn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gmipwgkck.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gzyxeeupp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gwyubwjmx.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/ghlzlrusg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnevwbnst.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gqnjnazta.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcprbplab.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gavhjlyom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gfmroxtzm.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gkmrkzxda.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gwseuruhm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/grsoajtmc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gkmtagsqa.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gmdioncdp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gtwgjfput.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gcjshfssr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/ggxocrjox.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gcnmoqqgl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gwjmpamnx.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gdufkqaio.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gwbtaszrv.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gbsmnainf.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gelojjgkl.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gjgxroqzi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gjgkaltbh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gmfxlnvmu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ghxbrnadh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/glcezgawb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gvxylfntg.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gtphyphmr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gpfvaysco.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/glajgqkre.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gejvaxtob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gsynylqwu.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gmibiuyxp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmosevkvo.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ginktpbav.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gjzqvdnnn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gcjufabvv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gbblncmaq.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gnjhzibjd.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gkluqzzcb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gosvdlakr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gsdmypplk.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gajqlygtj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gqfxtlspj.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/glspfosup.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gdmaipgxw.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gcdmhwbec.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gplzpiegm.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gepywhpjt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gvwmzmyev.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/grwnkgtlj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/geklxbkla.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gbslzsflb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gaztofrrt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzuerjzqf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gomettusv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gssvjqvtk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gzhqpempg.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpxtllcsk.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gsqowyhaf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gvrlyfpbu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gdzcypdye.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gutptkmdl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gnkqnptqi.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gxwrjdcid.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gualwgjbm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gfczuvtoc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/goofdlhjn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/govhpulrb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gstdhbcye.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gtoonfdky.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gmjxfxbtw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/ghwnacizo.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gcnalglti.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gdjhdnvmt.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gzumsjkjp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gmwprjbrf.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/ggsmuptno.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gqiefvvgw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gorfrwfwp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtczmedqd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gqtncsfcp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gigsomdjg.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gtbnanwds.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gptnwvjbu.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gnewsxfoa.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gitnlqryn.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gfmpigygk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gkisjzezi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gohodycfu.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/ghexazvzt.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gceovrcds.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/glhpmanbn.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gpgogqubv.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gftdfgova.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gurpgeigq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gxbyvesdk.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/ghvyhefqk.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gilibqyhb.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gwbypxgpc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/ghuswnqmv.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gcglvmlqm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gdwaonkdp.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gkkmhpvex.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/grnxlgkrc.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gnkpzrepd.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gzixbqaem.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gwbihycdw.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gmqnunyzr.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gjjviivut.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gwkzcikoy.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gastahjfu.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/grgxnvypj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gwdjtzrze.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gkcdxxmah.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gdilzewlp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gqodcvclr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gypimyawa.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gbjoheoox.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gzsvcfvfy.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/ggtrjrijk.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gsezyhwrt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gzryvdljp.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gvjoifepk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gewpisjeu.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gzqgofbht.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gyerltbcu.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gprmxejny.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gkkdueewt.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/goritolkn.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gkssgytci.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/giratfdtw.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gevhzdncd.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gaysdlivm.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gicjklukr.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/ghfnnzeml.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gffzcoawh.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/girfcyfdq.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gptvouwaz.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gaetdsydw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/grftljmnx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gbypbbwrh.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/geltziaji.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gygkoaipn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gmlfusecp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/ggwofhjgc.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gomkrcgqg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gzcohpusa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gzkyxuqxx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gkmlevbiz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gdeteeksc.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gvtrdbppw.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gasoaqeki.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gdsppyypd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gnsjbvdeu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdycctert.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gsewourhl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/ggmmnokah.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gasepigqm.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghrqficru.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gldwckuhh.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gvzrllyqx.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gyxuqepcz.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/grbhlpzcs.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gdrvxynqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gyxbgrwot.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gnzaehvio.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/glmblqkoi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gwfkvvpzl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gahrzcfxw.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gycinkmwc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/ggggexivq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/garksvurh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gsanmfvvc.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gcgtcsuqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ghrfrybdq.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gefubuywz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/galtnstwh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gskvpjsyw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gyzpfkhcm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpibuvccg.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/grhvvkgts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gnzqsxpuz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/guvntwyqm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gqvkawacl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gtamxshqo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gxirlrgoh.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gokeihzac.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gzhtpmivm.sHtML


<!-- 参考信息 -->