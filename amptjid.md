代发 wailian999

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gbyeyihzc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnnmdspf.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gakyjkofp.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyibebgcj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gpiwmmpjt.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsqqzxnb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcbykjqk.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkwxtxoq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzxbyckn.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzwiottgk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfshqsote.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gyzghdhgc.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gymcqjkpb.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gheiexlbe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gffhmprxk.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjuilbot.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gpwunrdix.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gsqojftof.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyzupune.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhanlqha.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxjupiog.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtafysms.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggohqacdq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gublijfgt.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gaswizmxf.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoyvllzw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpatflqte.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvpwyxeyl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gtvplsrqk.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhpzugl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtcpgfepp.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmnltxyd.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gombdpvzf.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gldpxjjqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqyxfrzr.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gsprlljhq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqukqgchv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gljekybuu.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuwmdjat.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdfdxdgwu.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gnonagqgp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocrrjcg.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsebrrja.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/glggncxms.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmodhfik.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzzhgaif.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtuzihug.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbolxjpa.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtigtewbn.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxctudu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkxqpxhz.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqyzmexp.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpmzphuft.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytegfqpt.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/giedkdyrh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkobxdxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgmwwyyv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gdcbiarbm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gypqozrrn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhjyqldq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/givudwwts.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoyuapoe.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gckbybrmx.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grvojyhii.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/grfiypisj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gknzttruj.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjtyrubv.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggccvecrl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gogrbzvbj.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtdwdfcb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gpbudxqnj.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqzfofos.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssvvtopk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtinqixwf.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvljpkxtz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfzwlrep.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupviujqb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glryfyaev.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gezzrlotp.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gofxyzvnj.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gczrfdspd.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gosseegbm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgimzlcm.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvodjeaqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkupbmqmk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcarwhcj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjvysqke.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/genwoswsv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfblxaibn.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjrmaixb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gcvtzojch.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukfedzcj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxxyfoif.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjfwawijr.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gefbnuhjs.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunndvavv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/grkjnurpq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gyxccsbqy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnewvkwu.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggkxrgrvx.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcyfqdkd.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvqnpudo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gczbfodsn.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgcrwtic.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gyshearrq.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmmxpmim.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaojuuzvd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdngoewzt.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gicclrlxn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gskospwqa.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmrwjbcdu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvgerrno.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gcpsqpygp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhsfnlxx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gufaxrumf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/getntdzgm.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjhfipre.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glerikmgf.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/ghudmonsu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwmmvusyq.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gacoduwbz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvnzcdhua.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqouiqzti.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gtypjqdfl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkbiljebf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gwqtesqbi.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gownadzlm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkakcnonz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfyfyhor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gwmjmyarx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwagupgjd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gqaakqupn.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjtahizd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiglwema.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfrowdjke.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjfzsayu.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gulghozjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpairjhef.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/girrwlryr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwdlihiz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyuelzem.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmlwknwu.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggyqqyrfp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gfngtbhhd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsnpihli.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaxlmtfql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gomvhtldb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzngdoajb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gfmupnaqd.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlyntopa.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gsvnzmrvh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gmtljwlkc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvespaiu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvljfslon.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsygifzsm.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gglmmmkmi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ggguraytn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/ghmnrjgkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/goxmodhvg.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gyngkignz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdsxcnxq.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gyyforufg.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkpuwhkaa.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/geocxkmsw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcavveph.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gdzrzglta.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gbikapomm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghzqzfwek.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gomehumoc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbfyomvgx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvafwsgj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeklkibo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbunsbjiv.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grpyvdhdm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctdxsuil.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrqkcmu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxxspzsf.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigifrefr.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqlfphgc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gpcfkddzp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorogpjy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/grvdunrhu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gwarwwmfj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gecdqjcwj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxhznfam.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gncvfeucm.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewabdxyk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/grswaicwr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbtknwawm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcugmhtm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganhpbrll.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghwxpwmcy.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gpjhzijmi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopoldhkb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqfnvjd.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpbsqfvrq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqltlygl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gewcpqmbg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbnuxzdl.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtveshoz.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gdqholusm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/grosbsous.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwmwfveh.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzwmmikn.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnmszjpa.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyidqkzr.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gfqigxfjw.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdehtmhlc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwlumndg.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjlfnjhi.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkwcuzuu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrncfvfr.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqreipdk.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grrclngsr.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwngndsq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqrjblup.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbmqlyec.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gklrxpymg.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmcyhmbb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnzlknn.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gopzgkgom.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaylbmyvt.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/ghbcvcqot.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrsgjtbt.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbeirfma.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbjzatfl.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllyhqmwp.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzwhlezf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyexnhoer.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawboumco.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcnixkcp.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gteyvpoxx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzdohxdv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuwrwhkp.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gznipureo.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ganrpemcx.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gnyrdasig.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gesaugugr.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/grfkpudwm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gzgxmwflm.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihhzjzga.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvwxygpi.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmshgcdyh.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfkgptza.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/guafpvvpe.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnurcszr.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyqpwyfm.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqertmefm.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gejggaaae.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gilcfzvlr.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdemvwvho.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghexydnlw.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdgipsies.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gohdwvyjm.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/grmsswnyr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gerdbpczy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gouutvuru.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/giywdroip.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gojskenrz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrqnajam.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfvksprn.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsxeudmuc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzsoayre.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysrwhkjl.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjpuiodc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkdduynb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbpnkivh.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhxuhami.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ganxxfmot.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgoxfkwh.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjjcyjdew.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbhoqtse.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbdmoqt.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzorgqkz.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwsrlnvc.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gobqandcm.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gajxozmrc.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwpvbgleg.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gusxokoua.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gxintqzbe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gczfrcwyc.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjzsanle.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnwvuezl.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gcalksrpr.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gftmwrurm.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtybirpjg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqiozfcc.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gcesfbele.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvpqlzav.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdvywwmk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbbcayhf.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/goqdyhboh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gosuximfa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gszsfacec.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzotwjdw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gingwlwrt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gteajmbwz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gwukhmdix.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsneunsbi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giommugka.sHtML


<!-- 参考信息 -->