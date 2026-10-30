代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gcwiejnmc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gxhnxhdwr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gqbornnve.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/giqdkdedw.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gymgztodh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gsjnkigdn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gydkigcsk.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gmuozwsdx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/ghxbnkiea.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gtonulzgs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gmksvphpr.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gkdkkunbl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gtkdjplkm.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gueexfboy.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gunpzrqiv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gsaxsskhn.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gysqqtyuw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gurlvvjdo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gpurtwtmj.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/ghhcsokbd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gyuomsrba.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gtdpepvdq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gfubcvvhe.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/garhcgrhc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gfpvxikgn.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gskupraml.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gevnitkbx.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gmutyglje.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/godsjmvoa.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gvhlpbfts.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcoguehga.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzekpmsxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gjvcerfkz.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gktvdjalo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gwsutaozt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzdwxth.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gtrfiqngd.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/ggzixbrah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/geuoamwzn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gslfodtlb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/godgagrwa.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gclykageb.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gwcyjgxra.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkgcallqd.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gfdrfwobd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsiredope.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpzcnxzdo.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gcftykxbt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gvrysgbuz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/giwrlnsir.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ggqqqrmjb.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gnapjchpo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/ghvyaijli.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/glcbpntgu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gpjwsuppf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gorjozuht.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gshreyxlh.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gpylwqate.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/goozxgpoy.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gvonviwts.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gxpvluciy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gnjcnaayw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gjfbglkxf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/ginoelvbl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gzlmkzlwo.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gfmgczwrb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gzetgrslv.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gwfpxkyka.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gcahvkyyf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gtymcejpp.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gspfpneep.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gbuomvovl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gypqfdgga.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gzsojxqdr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gmvliqfpe.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/ggqpxclsw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gdwdtmwtj.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gqkqgjepm.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gocrraxsk.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/ggecorncc.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/grqyadvlw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvoehlmmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/ggslqjcwu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/grehypyxk.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gydydbjxn.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gjzovvqdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gamynqplo.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/giismznjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gaifnlpmo.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/grgazdbqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gqjlvhode.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gcmueqnhm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gjnepmodk.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gbjcomjuu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gklwkwseq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gwobktntb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/guaxunews.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gvcfmldvn.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ghsyrmvye.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbmuxgtlz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gyknwjyfk.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gzhvdlqdo.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gugkghdza.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gqrsdyuou.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/grpliwvjn.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gyenuoibx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/guytgdere.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gajjhygsu.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gkrstdqjh.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gxymyklfh.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/ggblrmgjb.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvhyqavni.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/grvpjmaks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggqeulgxv.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gbmvteogq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gkcunnufs.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gayokvjzx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gyxxbnqjn.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gqckbofdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/guaxzbnlv.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gqpktettf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gzmjdeprp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gymfneefm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/guctbdmrt.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gmmajzako.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gujfpakgt.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gxcofdkpf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gjykfxuiz.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gcndalezm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gtvgolpkh.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gjxqbvghm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gvxgqtrlu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/giktlqmku.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/grqmuazdi.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gegjklubn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gnsmtyijy.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/guelmwvxy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gljgiovmn.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gbzoihmlt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gptixgeoz.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/ggdigdvxk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gznfifdcx.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gmzgvboki.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gkvnrgdfm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gioeyuvyj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gjghwzolh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwuoywhdf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gumuetugy.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/glvfmyfei.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/glvlszrga.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gwcpppofu.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/guvaxwhve.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjpfjvvif.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gfonyalhq.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gvrsiuvrk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gsgdvocin.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gfurvkryc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkqjsqp.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvuwwuyvu.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gsbcgzarn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/grpyahaps.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gmbqspakf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gjajtkkuk.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gfwfqqsck.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gqnynyklf.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gqwfvxtrw.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gkyretavq.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gdkmbuers.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/ghyfkrwth.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/guvsbicpt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gcdxhvwjb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gxsxfarzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gejnpvcjr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjtxejavx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gnnpxbtbi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gshueajii.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gblpfasjd.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/guodnznis.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gefnrhggm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/giuvegobr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/guwglbhqj.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gbiflimkn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gjvpltoim.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gsxnostyf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gobqisdmx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gwkivnjxj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gutdhjfhv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gutrwzujh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gteipbykp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gyidqnged.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gtkbnbgpi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gudwwkqlj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/glfzekrwf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gtxfcllna.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gyhhqskwx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gvjzocnwm.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gnfsnhdvs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gizqzuxlf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gzfnnulmg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwadofa.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gpriqwtbv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/ghlxiislz.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gwwulofjb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gblbkshyj.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gnulrqcty.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gkzjixesz.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjkubvuck.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpiikhdor.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gwmjopuyq.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gwlrgclbm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gqoakvxkd.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gooaqtlwm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/goebaftsx.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gggzjvpvf.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gohwazccn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcpcfclxm.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gptlcwbrn.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gdwgmzeit.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gckpeiejh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gyeimtmje.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gegfesvby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gqmzmnrmo.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gdbvapjvy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gtanncjxp.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gjalqcaam.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gpvefeaib.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gegikbqwr.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gvyrerjyc.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gavruhocc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gutlzkywh.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gfiakdwuw.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gvnyetyje.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/ghyddnkpj.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gxhwksddj.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gcyefyxgl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gwgbsvqim.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnxgaokpc.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvmcevwmb.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gjhycmrza.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/giixhoxaz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gdgtkcebv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/guqalblxm.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/goyfmgaoe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/guhboultc.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gyxkjyano.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gddzxvkjb.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gxmogddxw.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gduleemyt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gospcdwac.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gbybjsduh.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gbgavbsjj.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gqxlvkmqj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gggbhsfmf.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gdrvjvims.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gfsxbcjlz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/golapgsgk.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gqoweakke.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gizbnziuf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gikgxpsdj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gmtfthmpe.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpnuqgrcb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gqywsphap.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gcykfqbyx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/grqunhljp.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guuodbfwp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gosevwneu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gkexxtdir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gjwnekqlr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gdqqhagxw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gqkoueoyc.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gujgfouhl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gnpgcikgr.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gmmhepyep.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ggxclhcss.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyuialkkj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gqzthataw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/ghppzthul.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/goimrjeyk.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gakwkhkiu.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gmeygkomz.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gdukpjuji.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggedwpngr.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gkipxwbsj.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcjzqlvce.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwufdyviv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/ghqmuykef.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gdirxwrus.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gbwybmqqi.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gbuxacwwx.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gneasqsvo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gcrfoitol.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gbmtpvnip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gfttwgkhk.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gwwbsuanz.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/geheqjukw.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/geeibhvon.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gxbqlrfzv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnefhqvby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/ganukwjwc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcbipepyn.sHtML


<!-- 参考信息 -->