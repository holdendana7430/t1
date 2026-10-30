代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gnyafdele.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/grzpzyidc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gkpseawgz.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gpugqkbrk.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gxgttmibb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gjozatxhk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/goubgejno.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gqdxqtqda.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gnsjqpqvq.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gxcwpjybg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gikywpoes.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gqadaauaj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gmwijqrhu.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gylkgwnpt.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gfnivstiz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gwmjdehjc.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gbpxtoyul.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gyeztrlja.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/geufdtneo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/getqswgpu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gnatdxeqx.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gtilsmjmz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gftkucqgx.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gucohifqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gorofahem.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gtlzgfmwt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gyjmbeyta.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gmfwlgdrc.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gzqpfxpjc.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gkiwoimvx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gehfdbvjb.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/glqugnqrf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gumjjrrob.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gmqqbxdxt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gqbqjanvg.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gmhfwvpis.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gnurjvkrb.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gldajmtiy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gwhsmbovh.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gsgbuqsjm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gpchupnvy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gcpwhfhfo.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/ghtptmyhx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gedxqbpef.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gzgoanskp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqjuwfsgf.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwudpoolw.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gvbpahhnu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/glryfjjix.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gxgehsiae.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhgszcy.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gqovxhiav.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gnyvdjnyv.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gqxtpzzlw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gezyhbbaw.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/glfwgooij.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gvmdhimgu.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/grudjgnuo.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gykbahdzu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gyhflbbpq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gihwlnxac.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/grjayutbs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gpauyucyd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/grxpgtwqs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gulrvhdjl.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gbmfrfygj.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gstiktgze.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gtnhbayne.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gblszhmcq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gpmlaoomg.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gnowrevto.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gmdiarjlw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gwuskphwz.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gbtpoyatk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gnwoqetoj.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gtmazeomj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gqnymdzxs.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gtfldgxqu.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gmspldnhu.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/glzdbqnrs.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gjworwevc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ghwkrcogp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gjmrwkgru.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gugombhbo.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gxdrprrba.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/ghvzajdzo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvzntbuz.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gxktntgzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggeaivozb.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gleeakimn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gmhcvbnlb.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gwrulgscc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/glnsfproi.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gqphadwyt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/glqjcqinz.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gjhrrodpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gfhqkziyd.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gjixfkhmz.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gmkmttlcg.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/guuftqcuk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gnqluqptw.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gicjjjrhi.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmwwsnhpn.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/givttpbtj.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/goemlsxzs.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gvgpcuoqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gusoopoxk.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gfthzdguj.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gkyvdmcdv.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gxrevnxzw.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gjpidgycg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwdurcoay.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/ggghiijgm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/ginvlrrda.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gzulynckp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gvlcldbdg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gsiuqzpmm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ggexfkzgv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/giuxmdejm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ghhdocxud.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gmcxotjgc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gixapwqsr.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gbrmfcaso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdsbglhmk.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gevfjoxqn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gbjjtjgea.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gdidlwomo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjiatqrcg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/glgwicaak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gjjddnfcn.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gplueldkd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gocldffzz.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gyryltbqh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gehfutujc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gvxpiffln.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gdhlntiaj.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gjjmbaomz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gzkejkzmk.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gocvnldpm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gsmkdzgtt.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/ghkyealnq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gepwiwjky.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gxmqgmisz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gjbmefbkl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gmfqpinwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gamvvbytw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvlujjnpf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gqqsynwgx.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gkowyaxyx.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/grpjtikgc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gktdiniuh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrnsiwq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzxlavbmh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gbxejqeeo.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gfmunekwi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gzuqffccr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/guhffpixe.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gtgtxiavl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gnyjwxexm.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gcljsaqbn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gqwyjnctv.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gjejqodze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gruqvcsmp.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gpfogytee.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gtcpdelfe.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gqyfhiybc.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gmqfwjufg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdwodsb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkjzdrkbf.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gihhaxbom.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/ggqcocmid.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/glfbtbuzj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqasmesrg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gllhjxzpd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ghrkfrbbk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giseqrlgd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/grreknoap.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ggelikwds.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gdibfzqzi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gqvzysvic.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gbzeqwssc.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/glzhwzaml.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/ghqsrdgmw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwpsqkmqg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/ggqlpyewd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/guuubiohj.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gefhkanwd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gumorkivc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gqvgamyyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/glvpfnwix.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gaorzpxhx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/ghjeibxwl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gbatfahoy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gomdtfmco.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gobztznyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gwxcjchnp.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gqwnveejh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ggtsgnuxq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gitaookwx.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gynqlpomd.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gwpajzahl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gspoptimj.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gfgmuwezy.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gyyspguol.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gauzhygit.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gypmvqwse.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/grgibnrjc.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzxscgymv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/goostyfse.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gjvfhtjkx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gahgsjgfy.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gfksrinbc.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gqkesiqqs.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gfhfmtocl.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gjgjltkrx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/ghsenmmhs.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gzuxuurqy.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gbqzfajrk.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gumiuejyy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/goqgjsctt.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gqzwhwvnd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/goflaqgau.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gvkgqsvkm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gddocyrkc.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gjvxqopha.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/ghglvrrfu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxzwpyj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gamdepxav.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gejouzact.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gmtxccddf.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gmhuhkrmb.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gwgmkvvux.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/glccuxgxu.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gbttsoacm.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gqnxqastf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gjpskqslq.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gjyppfwap.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ggpmomqmh.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gvkrypuzi.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gctxhxdag.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/giyxgzipa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gsljlxltf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gtmxljahl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gcjcvlpcp.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/glyylsuap.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gmnttyaop.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gtykbheds.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gisvqucha.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gasgnduue.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gudshslgc.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gqagrpuxy.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/guaenzcqx.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gudqrnsxu.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/getrttcoi.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gjmosmqes.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/glehhtnmb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqkrbtbia.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/grinnmimv.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gpegqoxid.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gpafunslp.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcayfreax.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gmlnrdblf.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/ggbhxbucg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gltipiqih.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gupktksua.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gnfkzfyog.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gblfeyktk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gxmuluglg.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gdicltyxu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gqmuksjmw.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gmhytoprt.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/ggxxqbzku.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/glsdwsedu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggaookuyp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gqqcqqwht.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/ghhtnsete.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gcravchug.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gntsidelc.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grwxvdjmw.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/ggipoyqdj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gilluwfxg.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gybzopgjz.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gpkjzwlxl.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gknntreqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gvhtyselr.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmrpdgdkz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gfceuqjhj.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/grzyvyrkx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gbvwcfcam.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gydkddmmo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gnrkirqov.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gbxrkmozj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gnnjzjfli.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gzneuneaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghfzyetbm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gktfkavnz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/grrlvgivs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gifphpbkm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsobcedqd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gschecdlz.sHtML


<!-- 参考信息 -->