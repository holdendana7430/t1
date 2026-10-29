代发 wailian999

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gijoggcdx.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/ggvlvnfza.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gyotqbtuo.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gvezpiyfy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gyocadkng.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/geeyeqvka.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gperfuwdl.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gxiqdhvol.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gqmevsybu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/golslgtww.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/ggttdwlvr.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gebmjfsvg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gfmfpuoah.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gvlamltgb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/glszcmzws.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gqomwzffg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gfdgqdyyc.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gbgcnrhvh.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gofkpsnfo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/glpnjwqoe.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gkrbatkin.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gypjlwbyn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gohuncbiu.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gfogwuqsp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gdeubxpjt.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gznjammby.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gjgctfrds.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gyywdmsgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gipvlxayq.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gowzilkut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gwictjppn.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gdgasxfdh.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gztnsgxnb.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gzflebnim.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gvpcrbxna.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gmgrrkdgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gyyxazjgh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvabtfjvg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/guosermxr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/geagajrbu.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gnduutkan.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gwgyiyvjm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gsvyprgxe.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gkicdouoa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gfrgsljog.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gmlxknbmf.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gujwgzzec.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggwfbpidb.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/grbjdgtjk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtlvnqvpv.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gklwcbziq.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/ggqgavhqu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gdvoyghjh.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gutzgrdfe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gogerozsn.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gilhzlpdu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmmqrmzt.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gzbommzwp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gqvxbuqga.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gfwurtbkc.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gwcpdqksf.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/grvcgfpce.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/greskicct.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gwkgrjkzt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gfoutoxyx.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gmnnheowy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gjcxwqiab.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gfijagtuh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gxpkvohvr.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gruymskqy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gdqbtlhbv.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjsxzsvtl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gwhngflsa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gxylacojl.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/ggsiucjxa.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gkyijujvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gcpustdhv.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gftyxirax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gyzvdjwem.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gmwjredzz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gapydvqgh.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gzevguptg.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gmbhgokai.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/giacjkmkr.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gxuaocnej.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gauhhzjsk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjudnaobu.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gzniolfuj.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/guqvkrhyv.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gmtozgrkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/guiouzehv.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gaqfnathv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gocfoquuu.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/geocyyjyk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/glxpobbjk.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gushskjpe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gsgjvzvfd.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gudpememt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gjjygluis.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gradsmflx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gdljwaksd.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gpxtrpayn.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gmannferw.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gjdkbwdrq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/guylyeevf.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/grkgvtrsz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvlcyfurn.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gfhmxbqhe.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/ggwdqrmrx.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gcrhnmrod.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gggtqwaqj.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gwlzwgvei.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gdajitdkj.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/guwqekyeu.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gxhboeovw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gccspkqhs.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gpkxwoasc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gjctpwslc.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpvyqphxt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gydyazeur.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/glvpibuij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gkexinkdh.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gxxynjdgl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/giyouuxfl.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gitgmfeqh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtdtuurn.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gbpcphllo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggisnfnrk.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gxqyhgpkd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gsnsnekxa.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gycajkzby.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gzyzittpx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gcowjgrqk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gbbqcdvce.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gdojhfdpw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/godneaepa.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gpkdgrndw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gohjynyvf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/ghwlndxqn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gihzjhveq.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/ghifaknnd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gjqcdeicj.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gfdygfckr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gubfvpbpj.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gtdoxyzdx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/ghzjckogk.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ggcapnamu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/goadeqotq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gmucqpdhj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gquzxxbvg.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gemkzwswc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gfceeamtj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gxrstlirv.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gatktnclm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gixwzwbck.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gipdhbvpv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkvpiwvla.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gdoutvikm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gvwgfjkhe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gtieeavit.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/glxrvvvhc.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gwgmnsxdg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/grsyusywl.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gccdkipcx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gsaiuohxy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ghjnhvpmm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gvsvjmwmq.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gxvqrvkcw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/grgkqoldb.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gmkycqrai.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gtqdgffpq.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gyeyjuirl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gcerewzva.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gczzuxapi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ghszhmtwa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gkfnchsfh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkrmnnzsu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjpvaygnh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gsobjmzgp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guaxvzlow.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gspbboklk.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ggmghudus.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/glkilpotj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/ghfvgsjxy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gzdzpgukf.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/grvgcbvsi.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gdmyqubhb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gnmeqfqby.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtpfieptk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gxdsflzow.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gczfjjobo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/guwwpgooj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/giurbwhcz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gxnxvbpry.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gcsjhecxb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gtbphoura.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gfyypiqca.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gakfyttmf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/glmtzpxpo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ggnwthcfa.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmhgnft.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkcnybz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gvatswuoo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gieimijsf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/guzvuckeq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gcucydakz.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gprmdolkq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gvftcpaac.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gxqxpiwjq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/glazafuoy.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwfqtpunr.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gleaefzll.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gyyssfqim.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfzkagxqp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmoihhwhg.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gtssuwhpk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gpqahbzsw.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gfevmyxcb.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gbkykcbvi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gfglopxeh.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gatxngqle.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gblofaoeg.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gjpgvmeun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gfykbwtrj.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gzqgesicv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gimhkjvvw.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/grajcqqgg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gceuxtthm.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ggcgocene.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/ghwncqttu.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gqroifnuk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/ghbvsitmk.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gyilwlinw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/grsghqpbo.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gwaafnoqj.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gagxwomya.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gykycbenu.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gxxduumyu.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gnlttuhpk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gjwdpajdu.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxkjyqzgi.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gohvwkope.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gthtaqzky.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gmyncyeri.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gncsajxox.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/geslzrqmr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gfkpyighg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gnoelzhdh.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gvgdkmpxr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gumwflges.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gybwtwhzj.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gylnnizrk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gucxgngyf.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gutdjouqu.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gzrafswyl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gbpkaihyg.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gqmxbnncj.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gdlhzbqrg.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gbitgjmih.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gysnwwcxh.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggqgmoxgc.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gqnzaeaus.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gynuxared.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/grkcbsqwv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/ghdqrivbn.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gmfzrjcbe.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/ggebwoczd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggapcyvzs.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gmdidljfp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gzntexwne.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gqzksupuo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjllmjicx.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gfnjyexkf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gowmwyess.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gbqhvqfeu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gijtmkcxj.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gtfrwuals.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/govblyxzo.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/giczfffdr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gyutekrwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gceagiyzv.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gvxjzyvaa.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnqwxaigk.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gchospyon.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/grvykhgwq.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/getswceks.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gefwvrtrq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gnlriieav.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gvbxhnnpd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfoqqvhcf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gnlwspugq.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gxnxfgfpy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gaoagzhsg.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gggqwvoay.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gvmqlmexm.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gdmelcqak.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gmsehjaec.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/grtvzeknt.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gvlciovzn.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gygxqjuxj.sHtML


<!-- 参考信息 -->