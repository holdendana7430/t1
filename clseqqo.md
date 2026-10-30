代发 wailian999

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpjlfoyf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryeybzgx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkquhafqu.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ginejumjc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gizyqmfnh.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/grqjdqeep.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuqbuwyw.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gtufjywbs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gpimernci.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gngjmpdro.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgpawhsy.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gotdniwee.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gaqudwotf.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gizgihtgu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geltucepz.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/grsyemzxe.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gugkicvqh.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gluezyyno.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybkzyhtu.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/grgvvkahv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gvfnlqcrr.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gktpndkat.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/geuwagrto.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvmfdsau.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwficnams.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gsyxnhzjx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gajmwdrhg.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprkzbmds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcugyzyu.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goswzratk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gpuqtints.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gxsjzjulb.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcryudgf.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gykzaeezn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gftidpvby.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjpsjxn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyaudrmk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbzwklgj.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gywglgbyv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplwrrctz.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gygnzsomw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfctpqijz.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflvyhigc.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gtwzsmglk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghauxzyki.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/glvgamlge.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/giamlzeji.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gihgvtpqw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/glvuvjpdy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuvdwdev.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gftmhlrrm.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghekmgxjl.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbexiyvtk.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grwjhwsyo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtteepgi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghclsvkxy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ggcspbrkg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gmabxdyrk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/girtxzxot.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ggnnxgxun.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/githqpjyj.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gpobvwvnr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gheputgjp.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwycpdsmd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/glfsmfamk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gizcwcrvy.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwbxdrhxb.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glbcjrull.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gnczjbxlv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidtgdsua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gfqabhahd.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gvvtmtfij.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gbddhzcuq.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gltpelkve.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjrawyxp.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrzidlvo.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyckcctpd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlkmkbqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwqqbkdz.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmmyxpupp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/geptidtqk.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkdodbwzz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/grhuaizct.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuwnwmnj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxkwlqq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjhrqhvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyqcetlh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gynujbipk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gyprgogfj.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gofruppwo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkorhspfb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhsqpcjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbdsaruz.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcbwljcve.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrrpqlrw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewvfzwxb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfuipak.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/geuvnokbp.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzjllclc.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbovqrbdb.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgyqfhal.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjuppzmg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gauadfquv.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/glxkstzlf.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkahqqfnd.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/glqddrksd.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbwrwsyt.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grawchcqn.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdztzpcew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchmjjzaf.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnwnkyhz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gjyayejki.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gweaohbmw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvrlwtean.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gymsvtwuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbymlpgaq.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjqooauu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glvvsoupp.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gjyhgxhxv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gecijfqlr.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gshyqwhew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcynwczqy.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrcqpaov.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrpmodrx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrqyltwu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/ginhdnyxv.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcbztgzcn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gsjxenosw.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvmfnnfzy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/giujxvxgf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/glprosaon.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gkzwmzfor.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gelebwcbb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxytrawip.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnpjpwwt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcvvhnnz.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwztxmls.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvgyizmho.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gnhrwzzxh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjvsvecv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpccjfuii.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwiygwwz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkctyzly.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwcqvrmi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaeujhdy.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvhlpifyv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuripfqw.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqkbajlt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbmnaohk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghncuctnr.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjnchlyt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcdrsxdj.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpopneggu.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gsnitvadt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gcckvkkbn.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gkarspfvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/guswkhebe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnmwuuvz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiplabsx.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gkxtakfls.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gluxsahto.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/geryjduuf.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gtqmwkalb.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gqbxpwvzk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsgirtzz.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpapslqa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gdyphopir.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxewzomuj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtooznul.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghjmeiqjh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ghacwhqfa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhddkwmy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnrnticr.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyrbgoob.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpurslpj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzpaqewl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhsarcra.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjxrvpuh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gicbpyyec.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gsimoxvqi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gonmgqeha.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gxbvxknpr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/grhimsgyd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmrmcxxle.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gvotbbisd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdqfevag.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrzhbryp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gaepgtbke.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gilbffjli.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvmkflaz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gyimtfabm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcufxvcnj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzmefigb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorkneoq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gzexjvjib.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjezoqiqg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfchprav.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugovunuh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdeuysvc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaxnthes.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsdzhjgf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/grdliyjgs.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gebumngvo.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxafcjwzt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcvezvfw.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gypqfvwcr.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjfuhylas.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsciirlrv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiquiwbe.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gobeejovm.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gegdbigrf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gcizohehg.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glwtvpbdf.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcrxzqqb.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcvmhqps.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/genrdemrr.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapebvdcm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtghsoag.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbjqcwmg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhxyrsap.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/grupaahng.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqycajkaz.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/ghizyjkme.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvgryjkl.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjtquliel.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfjkljbh.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gthxohuwj.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsopngprw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyngthkbi.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gmzruhziu.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvlqbcpw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaodjeoc.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghhsdqgkd.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcavklnd.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/guorvwzam.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdcuire.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzjfdfak.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gzkfxfphf.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/giioplrrm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gczzwaghl.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqhbydgl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfjvdase.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqynvipas.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/giekliiue.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfeoguam.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggokjrpbj.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvzgsnit.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgikalxd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqnvcazs.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxvbazpv.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gxjqyxhfd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdaafdv.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzmmutgz.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/grccfshzc.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkwexziu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gffvcinln.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gyqeuptsd.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gddacddio.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeycwmyr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpuzswgbs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjrehcef.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqutholfd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glgzbtbxk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbgidfdv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getlrietx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxczbodw.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbhwnlzui.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gqukmtqjj.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwuexmxe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzomojaph.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhbqbblo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqxwtsrw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuahtmsw.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxefobojm.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/genweysej.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gogkejylu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemelqdal.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbfkgowv.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/goscdllam.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gqztyxcpe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbesaxhu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbjvimuz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjsapxjv.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gytlcpgll.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gpksoalwn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/grematclc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfzbabzt.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxnyrfma.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjnmcgd.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwfvumvfh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzydvbn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsepalyme.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gufbgyure.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxolijfp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnnhbwue.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfapzxsxi.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gvmgvnmpk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjlkrnal.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiwwaknh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gccobwhsv.sHtML


<!-- 参考信息 -->