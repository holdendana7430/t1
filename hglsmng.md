代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/guzndeurk.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gmulvpyuz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gsqjlycrs.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gqrxzksxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gvckyotgt.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gmftjohuj.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gkvynjlgb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gkvubfens.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gzrljrtjr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gwyzxrqjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpehshyih.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gewsukgzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gkgeurfws.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gmeuhtzqk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gpkuvexbn.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/grjclvfdg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gffivtkru.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gtgqdcomz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gftruhlss.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gldmofihw.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gmpjvhnqv.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gtmjvswyw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmydywkuk.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvzehwqtt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gylcuxprk.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/ghbvgrvtx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gkofldybw.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gafzahnde.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gnahriazh.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gffzjfggq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gypjdpsld.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gqopccgzx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gwtaxpbzi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gjiapqfwe.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ganaghjff.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gufgjtmao.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gwdaicqzz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grsmhtmoy.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gidzrjavy.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gzzsuruky.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gujiwfqdb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gkisozuqt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/geiidcaog.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gbalyphgo.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/ghruogotf.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gsjpmyaxs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gwrrvykqw.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gjoyldhlo.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gguojjafx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gcncyozbc.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gfdoicykg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gdupzyndx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/glbnvyyqe.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gbngbiyaq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/glqbuxdlr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpbagyfyb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gpfcieanb.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gnxbaeian.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gegzagerx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsbmdipco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gixubwklr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/grwawwats.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gszhtspyn.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gfrvzwxfn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gljilgvdg.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gvsiwlhxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gjgttwlmg.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gndauhkvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gxepujzup.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gdnyjvghk.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gloyreovz.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/ghoiecxwh.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/ghexnuhxn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/glioguzue.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gwneaygaa.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gygwaaabp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gtyvqwhsg.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gadflrhnn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gttyhbtiy.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gvodbzrmr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gjpoxkvit.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gyloumpmt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gtkqgvcdy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gmpanjumi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gvawzdukf.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gplqqzswz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gifeypphp.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gxzbloprr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gthysdigk.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gzmatdumo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gxxlfongz.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gxcrtevyb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/ghpkluodh.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gmjogzfaq.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/grfkpgjsh.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gwzcfzdpj.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gaffzptqo.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gvfpsyhab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gnmgxiyef.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gkavyrwcp.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gqrxlltec.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gccknvvab.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/guxhdjwrh.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfkqjpvvf.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gwbtjhkrq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gaxesxbhg.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/ghynlomyy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gamtedcij.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gyemtmwol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gihcekztu.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/ggiowavba.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gvaheqcqf.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gxhcugzol.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gpwfcncqf.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gjalffimn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glpsucpgy.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gupyvpfvo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gtsrwndab.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gktsyabfq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ghreujzep.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gzcgmdeoh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gcrsderpt.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gwlhdttpf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gzjwllicl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gfgfoygrf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gylapbark.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gudtkghnm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gwgyrwpvx.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gmhystqhi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gmlcdvodr.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/ghmxzihnk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gmywzmsyk.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gjpkjfvxa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gztphgkum.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gxuxrtmta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gestsnchw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gayjlafvc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gylnysjzx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gplfyhnlg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gjppzijlq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gtmpxucer.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gehrrfaci.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gjlzgmynv.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gtyzyxong.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggrzzdkwz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gljnmrmqv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gxptnulzg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/ghqpqdbip.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigygsvjd.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gdzyeyxqs.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gbhwjoauj.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gqxpqbsls.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gauumegxo.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gvvyzihjn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gwbhgmaqf.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gidlbksuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/ghzlodyol.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gncdxxman.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gdwrsyrfz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxlavbcez.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gvkjxqcpm.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/ggrudjtxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/glxtnoonz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gcsgsoysw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gbbqmuvjx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjodfbxst.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gnrcaqewp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gujutbxsi.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/goqeqsekj.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/giisgjdsn.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gveavcqox.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/ghspbexiw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gnviolvhd.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gyzihpnup.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gwqnvpwsu.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gqcjvsbma.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gfcrtzbda.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gucpoliij.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gzoubitxi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzgpgpuhk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gsuoehrqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gioimnnpj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gbllxfqzd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gwgqqagef.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gcemagbrw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gwktlfwxs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gmscjhape.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gxxksljje.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gogrghkzj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gpztidscz.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gsaliddwg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gupzwtlig.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gacoosvfs.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/goemnrywz.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gkgobdifp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvgbvvuid.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gnyzvufoc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/goeoxsueh.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/goptywjbv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gixovtbmc.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/ghpkujrcd.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/guxzvhjcv.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ghjbtbgqs.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gfxezsewv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwewifxnm.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gcqvwkvoe.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gyysvoxus.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwaboju.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gijrhuvxb.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gbcxmeapl.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/guiqvakzo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gfelwswxl.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gkfqyqkax.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/grbacstyi.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gszpszswc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gktigdlzp.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gmncnbbfm.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ghxholtat.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/glsifijxt.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gtjpqvdcq.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gctsmawbu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/golhwokxa.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gcnubqjms.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gvnxzvozh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gmyopghjc.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gnbqjjngy.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gckeeeibo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gdlygyvtw.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gktutxtqr.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxuconhqf.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gxipmoiqr.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gwljtszky.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gwokddzgl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/guvladpkl.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gyhuhitcr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/ghflizdwh.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gtrdhxjok.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gtymlhjjn.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gdaqnrpkp.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gqikgzebm.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/ghdqyaxlz.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gthxqefip.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gcnckalma.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gvloasart.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/galqqquug.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gccdkcpvi.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/ggngymulu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gqyjyafsq.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gpreyscdx.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gmcqshxao.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gsfyjfvhs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gmkptutpr.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gawmflwff.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gtgveaigz.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gabwubhln.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gxzjkxncd.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gwojwwxya.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gkkkeysqu.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gqwmtmlzr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gbvwzncgb.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gualmsufj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gqhoxapze.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/grbjcneyl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gvilkppku.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gihhbimdx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gsfynrfal.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gatutdbqu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gsncaljek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gucyfrnhm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtxaxet.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/glyjwrrct.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gfhhvforg.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gepczrwhk.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbgzeydxn.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbktcoqau.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gdshfbvlf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gubmogspk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gybdwoqog.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzvinzrpl.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/grpfgmblh.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gbigbcnvo.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gajbmjnfb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gdkiisqnz.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gevimbpdj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gkcrvlphy.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gylbogokn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gupucwcyf.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gqnnousnc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gcwskgaqd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdhqnzgqn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gypszlyut.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grismkdwa.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gshbkqkyf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gaqsmnysc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/ggstnsskf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gjgmmocup.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gwcqhqqba.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/giffhrgcu.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/guisblhga.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gihemlale.sHtML


<!-- 参考信息 -->