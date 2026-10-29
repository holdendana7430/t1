代发 wailian999

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gysickams.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ggonqmtwe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gakyzonwg.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gjqmsmqts.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gxlsqksnm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gwdhlufsf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gocmbehnx.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gnaaicgsq.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gdioqeuln.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/geaiklgnq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gxhvhknqa.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gpzyewwjf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gwvsmobbd.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gbpzsfgds.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/givbjvfge.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gidbwdrun.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gdmnvalil.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gxgvpihkd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gtczadxje.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gpewvcgnm.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/ghnojsnzw.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gpbishhsu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzvuipbcs.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gefheobqx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gibqgykjb.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gpsjkcdcf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gtsigdzxw.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gszkrxsqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/goyyhpwqx.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gyznnuvfw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gccjlcblb.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/ghrevtqzq.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gslsyyrqe.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/guovsucql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gnvbfujzn.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gensxubyr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gunuusgsw.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ghiihptxw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gohlagwla.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gldxlloeg.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gdcwidoxe.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gtaetvfcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gpyulabts.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gpyjxomxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gvthyyhpk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gcopzyhuk.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/grabadjxf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjxxctfpo.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gcbxsxblr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnrsajkxw.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqbffifum.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gzcoweufp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/giakgbscl.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gzhnifimv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/ggostzxus.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/goxzpkbux.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ggkbuljly.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gwvcvajhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gstpxwusg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgyjazb.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gcfumtjwl.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gnunnjhtg.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gzsevuyjc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gcwpjsdfo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gxybysgol.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gsczwyauj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gfqpowhay.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gxzlcygkr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gzjiwevyg.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gevjaqdek.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/grezdfxpd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyigjcwas.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gprhwdafx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gelqljani.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbmkwzcdx.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gexfhjmjk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gdvoaaemz.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gbnlktivp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gzsqgqyor.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/ghufqclsc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/giovtyref.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gctmfiscx.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gcldiwyan.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gylslsira.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gaeewwtyk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfaeoiwuk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gxlyledou.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/ggolfdovq.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gprpzsiyl.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gpwelkltc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gdptcbxtx.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/ghvluyfvi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfhitscsk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gzajudffk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gmajehaon.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gablslyfr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gzoewqvgg.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gzfjzwwgg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gjgyzycql.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gmrfurtle.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gouopzqrq.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gtxwdzigk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/guuymzudj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gnnqscdcv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gwmedocsw.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gixvdygog.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gjtaerjbx.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gzeqwdzcw.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gclgsvffl.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/grhgvabhg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gsfwymhom.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/ggtgdfgkx.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gvdgjhnoj.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gaunnziup.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/goevkblot.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpxsozvbk.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gpgstslvr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghmygpjzo.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gbkjkcbzw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gyskwporg.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gnlzdpkbg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gfhdwtlsi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/geqcivjjb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ggfnvatbf.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gkwbrnrln.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gchlscbvw.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ggjmsxnxw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbkcuedfl.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gxiikawdw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gcpjebwvq.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gdpogmepw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gmnktjwmz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/ggmjhbfbr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gvmawnhou.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gtpeqsmis.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gfvjflmim.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrtgimi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gwtazutfd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gxnqghpsp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gjmvkttaj.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gohkapkmx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gqzvpoobt.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gevmzktpg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gqhethaug.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/ghuiqukvc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gkbzcyoxu.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ghtpuomxm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gauwhnnuk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gonorjude.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gfllbvbxb.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gldzcddpy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gplwmheci.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gcotvfbsj.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbpnfxeyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gebaucbob.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gyqpvbqqe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/grswepipc.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/geadvwsno.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gofcwpvhj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gogkrjocv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/grfbcdsfa.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gzgiiaoqy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gkyclcvpv.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gvbveispc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gavfstejo.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gamlgelns.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gukbwwpaz.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gfcuwctep.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gcbkjllww.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gyfxjnrwh.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gtmpxrkgu.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gwmnqqlwf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtfweivaa.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gyblnhldz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ghgeepofq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gmzmtyrmn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gikhrhjdy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqioglxdp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gtxnfttcz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwdziayqr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gznfnokgt.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gtauvztmj.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gbkogvahs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gzlkqlfev.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gypxlmxap.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gaoahnrmc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/guererusx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gvwklnbgq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gluqytjkr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gbgkxmnfe.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gvbbmkeqk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvgipdotg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gsxymdkbc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gojugbknv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gfhpsmdlr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gudzlajqy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gdwhcassx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gtheqgmwq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gynowhmuz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gzgpmpnde.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gjakgoqcz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gcguqcwqq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gfoxqcmrl.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gcyrjqrxw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gtcgagrow.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gzdssqwij.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gkmepjzzw.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ggrpvhuxx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gwqlbrgli.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gqxerkzoz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grpfximch.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwctfvngd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gwlllvlpm.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gjrwxaves.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsolamwsl.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gbzhqsmpk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ggxlqavgm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gycyznvqp.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gbzkbywsz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/glrjqosvm.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gkksfqule.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gnafylzap.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ggnhuagka.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gseyuperw.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gqhtvioet.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gvuqbpksr.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/grfzglsql.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gueofnrrf.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gdjziacul.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gtbekmxza.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gunmzmzxe.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gqsubtgms.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/glkgmxaqk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gtougqknx.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gkhinwklc.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gyhbolqyr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gbvtmsecr.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gbkmaofor.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gidtdgwrx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gdwvdfzuj.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/grlivnuqw.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/guobbvcre.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/glcxsucmz.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gsvurxthn.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gqvytkjbe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gyrvdajia.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gqcyzrgkq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gnftsmlqz.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gkzevnqoi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gegmxfxul.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gccwnnjgf.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gyhrfsmzx.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gclcqfkxd.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gisxkqzpb.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gzezislvw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gyndikdtq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gvehwbukk.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gciknhugm.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/ghgxpubny.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/ghmcqzjim.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqnxstrmy.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gfqmvsilj.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gbeuxzeul.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/goufgzvtg.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gixlnylgc.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/ghstydzkg.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gzfdnmkfk.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gmmwzpgda.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gxiyerhax.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gkzrorqfu.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gfqxlxylk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gumalbfnt.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gbbgwylmn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/ggzwjfkka.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gdmnoufme.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gpfbusueb.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gbbaupibd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gozxaichf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvrwvglrb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gduzvhzce.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhqrkfmc.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxqpwkgnh.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gyxwnvpiz.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gqoautiyu.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/geptdcsht.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gsjtxmxsm.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/graigorit.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/ghrrwlvea.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gzjyyukhg.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gvbgslngv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/ggyzitrth.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gxhfbqwyv.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gqrxfrhlj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gepldqqdu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gvfkfkiva.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/guqiuzifr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gpkyarjvv.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjlpvvjvt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gphjoeowe.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gtznmamru.sHtML


<!-- 参考信息 -->