代发 wailian999

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gcdvmyoqx.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gzsjxlspc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gfvxswyvd.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/ghzirbvuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gfhbuhueb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gzyaqxjez.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gzalxewqi.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gssybmvnq.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/grishprif.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gwapdpqej.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gklcttcqs.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gygnhasci.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gvmdxzwhw.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/glfkhrhkp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gxmmptsle.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/goqwxsqed.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gvubegpov.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gomnpczls.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gguwikcdv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gnrzeuglj.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gbmghcdff.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gtdjbyamw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gzowhphrz.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gmepdzhvm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gonerogtw.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gvzwmwycu.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gebuiiexh.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxrqhxldf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/glzxrvgoo.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gfjhqurdd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/goxasjsbr.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gfhounwcw.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/ghstnldjw.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gfjzumzum.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gtkhovxyt.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gwyrrzebi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gyiygaabp.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gunocfcoh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gxkwovdwn.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/ggojxnmsk.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/grznhurvc.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gjcpyrznw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/giyxmazej.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gvzpxiitv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gefptppbh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gpefugwlw.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gnbigqbto.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfgjkjzcy.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gkzlaunhi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzqlanvwl.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyiktvtyi.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gouyeuety.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gvppxadbm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gmskmrgwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gibjlphes.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gidtuplum.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gpawjfqmz.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gyvimkqnr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gcchxypjp.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gxclfzygo.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gtrpxtokg.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gneelvvyv.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gocyvvhrw.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gpayzdcqu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gztmyhemh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gvsnansxt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gxpaxcsem.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gjhcnpvuh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gxuvlugzb.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gizkymeyh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gzedtzmuq.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggobyiyuj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/ggemeamhw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gxuvyvwbo.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gdbnitudq.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gbqijfefr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gdjkqmikj.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gbcxffghg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/grghtxemy.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gitumnlms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gturrciuo.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gvzcdtyjm.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gvtlnexbb.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gglkxsjtr.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gwzilhane.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gherwvfha.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gpjlkyevd.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gsaydunpl.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gmxeqdbjk.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gxtvfgkqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gyjqekamh.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gdlekvaug.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/greekxbao.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gxxvwvolu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gwwqeoknm.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gjqdvvqzo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gunlsjenl.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gcddnwcjm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gxixtepbg.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/ggjbmvyoo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gmytonwin.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gflugtqco.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gohpxaogf.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gaalutimb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gqmpldxmy.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/guaoidaqt.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxbyabvcp.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gydxgtptn.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gsutyacxe.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/glntkrvwk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gcknbusxk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/glghiitvr.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gqqzzybyl.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gjefnzsio.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gxiwcxuxv.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/giihszpra.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gqwrlpxjm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gveeifdtn.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gfsloekdh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gzxjtxdtn.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gwwiafqit.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/giuiqmssb.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gbkmwlnyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gokiqacgu.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/ggcibwvvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjdtdlbmu.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gyckeckhj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyumwioig.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/golrgciia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/ghggljsof.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/glqygknbo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gcbgcjfvu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/granfjcuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/ggafylesc.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gpuggwqpx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gzvutlmfs.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqebfbkji.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/ggvjozyra.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/guamnwqeg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gfsgnikvo.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gkfxmecyx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/grkiqtwvg.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/glqewnydr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gqxmgzdpy.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gxdgyqzvy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gmzlpcohq.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gjrjurvbb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gaamdscew.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gbfyxsolk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gttozlynn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gijfrxrwe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gtposebmb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gpiyzqhjc.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gtufirlna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gxkebthji.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gchkytyfz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gnvkvupsv.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/grhsyaizg.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gwzqdcgqe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gpyhfdlbk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gukyzmctk.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/ggmihoxaf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gryvghjpo.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gtyarunfq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gokyzfrna.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gwwexdwpn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gezoinapu.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gzuuidoxk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gdjyvuwja.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gewfglcks.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gsclcghjg.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gxnvrrklx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gwahzwhku.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrurhpr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gncfxsgxf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gguldlwtl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/ginqqiual.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfvrvqie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gwhxqmwqh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkstepyzw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqmybrfaj.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/ghvgmbecu.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gvwphgujv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/grrvuazlv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gkesopkuz.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gvqibucqd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/grnvodasc.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gdkhogcwm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gylorjtfd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gmsuywsfs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gxwrouasf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/govmgjmwp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gixhgjruu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gqfoagrlg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/geicltude.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gewyuzzwd.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gnhxnetbx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gynmuyvqd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/ggodfmudd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/ggieluyvx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/ggaidkhfz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gljfdohkk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gwlzybmzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gxwhgwxyt.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gbbpkfvyq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gefcqqivy.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/goplncjst.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gwibqxsgc.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/goolheyhi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gzwdufmwz.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/glcyjfyno.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gessxsuhp.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gbqxtpcco.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gexsjhrtw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gruqjkwll.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gwlorbyll.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gmtjwxyov.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gwvdidfhz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/ghqexylji.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/genetmqzj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzcipystu.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gzrndgzmw.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gtqyyauxf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gwwmwbfht.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gyosrtymh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkvpanslt.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/glpavcrvt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/goshxendw.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gnrvspkbp.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gtvmyjmsi.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gpysbwjdz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gmlfbbenk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gnwadiuwa.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/guivgipti.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gkvqfrttc.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gearetkun.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/guhchuchb.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gpymxwebi.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gpigefuhx.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gnetudntq.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghbfzxize.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gqfvadylp.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/galoybcfb.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/glxxmxlll.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/geeqzgirs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ghmchezcr.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gdaeuubhh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/ghnimfaam.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gyvdjjfcb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gjgpqcels.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gtcybmzwo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/grqzbvkfj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gffhrlhla.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gejaihsef.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/goowbywhv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/grtkfldua.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqgulfgbv.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gjplpdrvd.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gmikgcpbs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gsyzknqnv.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gwniagsly.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gaxqascqt.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/ggehnymvi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gbusvbgzb.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gjdlyhoow.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gipyrcxex.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gsaybgchy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghtdxuxuz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/grqkavlgw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/ggpfhicch.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gwwgnfbrb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/guaafmamz.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gsxaevemn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gnmxjkbgx.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gigcjtihk.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gxnwtgxyz.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gezxzqvxi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glebfyrnm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glkbzjlyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gthqoflnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gzdibogyt.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkpsobylm.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpsptecog.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gehmcteqt.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gblqghrfm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gdujbrkhj.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gorrrkvfq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/ginyulmnm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnopxpewn.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/ghtxiixkt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/grkxsgkkx.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gbmvwxkgw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gfgivdwph.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gtrkmnboh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gvdywrkpo.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gtfobufjx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gdgicyvkz.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gzemizppc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gyfqlstwr.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gukcyvscx.sHtML


<!-- 参考信息 -->