代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gzdythgis.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gyrjdevtr.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gmobvsemm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcogrticj.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhxlqfyg.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gokhehepi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gozpgqhxk.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsxfdenq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagagyvgq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/glpsogkul.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/giakrqgay.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gewjebpae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvdgxims.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqhktcfv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwtffhfa.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ghglmnczb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnczcnfv.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgwnvibj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbweupel.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdozhjvec.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdcrpfw.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmhlslxqa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gpblhtelz.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/grapezksv.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/geuktdnpt.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gacmrgodb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gypovxciw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpjsrea.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmayncbtf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmugtvgsc.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoesmojw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtedyydxm.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/glhxsrzlr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcumecap.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gourrrsmv.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbdfogkh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnnejcie.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcivbtmqz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkgqgcqs.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmckbthky.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvotdbroy.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoewnwqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsxuyepn.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbkxhaix.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaidafdkf.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzmwcvjso.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxxsokpk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gqpnqqelh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbgtdqdz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/ghmseoxsm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjefwfhet.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdedqfzjn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/giekqquru.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlggjhkr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaepwtdtn.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gajkimkqr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbttcmfwg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gaprmudjg.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkceseoy.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gourckkno.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzshglhm.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrzelemf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gpskjkwfr.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdmvguyeb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gllkdkyid.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gsfwsjcdk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gloyvxxdg.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gowvbbjyy.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjpfqvej.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcgswpfmh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtgyhnkz.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gyhpvpcri.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzckwanf.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyuzxyzt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmmbkxbn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvqoqlgbn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsepdzkj.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gizzjhtms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gmihrdckw.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/glbrrwbqb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwkaoopx.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpsrkbgu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkcpexxq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gshtyjems.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/ggaqulsdc.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gisdgdsoi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gikwhtbva.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gegkdtjce.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcbaywzi.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjntotonv.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdefhjf.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gykxbgzdg.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncvsymfx.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnuvqbkp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvbofakt.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gntjjpvjo.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gpanjwsqt.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwwvgcznw.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/ggooutohp.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjsouxwl.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwyyzzyou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdndyauc.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqukgnafx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ghqvaqkqs.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gibnkvpar.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdhteqdwx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzpugbjx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsuxkimf.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gycuwcjva.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptadomjd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfeoxaqj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grdmahbxp.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqawgfs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxtcloig.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giznqjlea.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtabecvhc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaksjoemg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gflxlwdbw.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gftwhnkbx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwphmdxis.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzkjryvg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbuvlicxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqqlmse.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtofwrokg.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqawdihy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjtfuytv.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gunywuwii.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giruqlzdm.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gayuphiov.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grotlvgdr.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/goqkcqcqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkkmzqst.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiypjnsx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfxozwqp.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpshoyjcn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/glvujsvcg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvluwwxwe.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxealaas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwrierme.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gyabeznsn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstgaeigq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gonkpksoe.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzlqwqbd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gumtwuxro.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuogpdzx.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gxgtglssc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gweslojru.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnajyiaf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejrvbzss.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gbpurwtew.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgowkevo.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gswhbvvsw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/goejjkhef.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrzmxcjf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjtuulen.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gghxnsylx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfunncym.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gkfjzzoui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gggnuuqeb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcqqrwpve.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gftnrjyeu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gskwjwpwf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/goecaabaz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gietxhkiz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gplzrdbbb.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/guutjhhxt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goaemqklk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxfjijx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gwbtgosrm.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyffvbmh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gbphziwuk.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gvtquymea.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzppbvqcw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gyakzeged.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezzugnw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcgweltaj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/glwfrsulk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grhmvtswn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdobjuaml.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gabweglbx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/goynhqnzh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gxqwgslcc.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgknxvhd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdeuyidm.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gmwyndsvi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsltutmxj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/guhfosret.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkbdjjknw.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsoxepi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzcupqzl.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdvqhcpl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojwsbfck.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmjmbxaa.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gdcrgzist.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwghomgz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvgqghgk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyfjzymm.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzwjkokgk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjursgscs.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gossiulgm.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gcvqnnxko.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/govaiovpp.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/goantpphc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomtkfwec.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozeqyamz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqleejio.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpnrwjvr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gycfubtmk.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlihztuh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcffcgzd.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavkmqbd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgowiqba.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gakvdjfmn.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giggihtrl.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gijdcrxmt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqymydks.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxfzbhy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqaqxeit.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcbubynw.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gksxbsvlf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjvjwnhg.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gfxeiuyia.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gykwmeuzy.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gaakzljpg.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggartufva.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ggdgchghk.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxzjftxt.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gomoqqjmo.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfqptnxr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gdutfunnv.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gvvxxahvx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gokuneesn.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gvscjoseq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrpghaaz.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfucutxda.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gljwvozsr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gdvvqiciu.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gprvjfraw.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/goriqsvif.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbyiinok.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gtweocqem.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gobrrybbi.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gbycejuex.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsixnfuna.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbxnvcdg.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxebrpao.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gecpnjmej.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gzfhtzsrd.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjawcqdvn.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gzgccwaca.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamfiisqy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptgccoqg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfiggvg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gweodtvqa.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gfpojfteu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomlgizpa.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gwnekbkey.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtlfbzwou.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhftnpml.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gefpmfosc.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gamhzczzv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpaomuxcd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gputmerws.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggailjoor.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghgoijnff.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqpowbzf.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/grdgstmzw.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeiyhsic.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuspfvri.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpscaoem.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gtdlmbbcp.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gosbsxytm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gakdvdpbj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmuuyyzc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpvrngtk.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaodplzc.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gexofuwhd.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwijbtph.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvvnrvyd.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/guxkydffj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gpresbjuo.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnmuaund.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfjlckns.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/ggduvxgyu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gnirbcuvm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqiwexd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guelhrlsp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnugeavif.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghujbyqzt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gvumclptt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/ghsmkbmpc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwskpuqk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafejuusk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjasjmac.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gwnnuslwg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/goknvsttu.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngmizzl.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqrgbkxv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/glmsqmveb.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/geqmnorth.sHtML


<!-- 参考信息 -->