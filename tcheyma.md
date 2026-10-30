代发 wailian999

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gitboduze.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/goxnrbhtd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gqefsqfor.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gnavtioya.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gvgtdpmzn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ghinxmimp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gmswmdbwh.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gvesqqego.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/grryobqjx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gihosjqjm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gsierntgq.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gcaeomfca.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gqtsiuare.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gbiqljwnl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gwvnibigl.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/glgjlaikp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gixfowgwb.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gnhqpakmj.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gkyozkhak.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gkxaluflr.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gvycsfyln.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/glbmwqpat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/ggttnkpna.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gmuyknixx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gnyjkuwbu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gizvkkwwn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gxxcpvwor.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggbykeuwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/graulrshu.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gxmhqxsau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gnkrbmzxx.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gtskenguo.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gwevxzrwc.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gdysnqpjj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gskshjgns.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gmmcpohaz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gnduuwrbn.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gapnikpqg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gmsqsldud.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/grslyucwj.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/geqmqpcdl.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/grtkrylxy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/girnwwkvy.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gnjroombi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gsmjfhqmd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/grvgfzxpr.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gcaezfpfi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfkcuyppm.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/ghreprehb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzhndtfsp.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glldpphku.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gjzkmowah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gyogysiuq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gomuwmpxj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gckbkxvld.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gcphcvppa.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gogxzbdrw.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gwpqlriws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/guvyedmtj.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gybdwatrl.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gbofwcxiy.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gkcweudap.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gjoocziaq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ghudllohl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gizxvgnya.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/grvfnuopp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gjbvvfpks.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gvusexdri.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gewjuayjh.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gieycnivc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gmaoksotj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkjcrbqgo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/ggaqtzkdn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gulxjgzhx.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gcwmadzvo.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gvrgyakfv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjgwptcek.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gzmizbuls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gbhtsqikj.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gfsyserdd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gbjmgwlta.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gmjrxnxkl.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gdzqlzpju.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gpmsqfqqn.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gmuilqsnt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfcqfhjzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gjdygftdr.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gzjgbdefb.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwzbfjuqn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/glulbmoiw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gzdnnvodg.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gzdgybkyw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gulssfswa.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gopvmimbb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gtcdsiavt.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ghhyxvqcm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gfjzwxnsm.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gpwyogxid.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/glgqjfdky.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gzasgpdzc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gpgqndklh.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gglbagzlk.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gjbuwzveh.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gnkrajyso.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gafpcbhcm.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ggkjduaxb.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gywjqsfib.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gqrclpkov.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gyoazmxxs.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gmrrtwqum.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gvaghslug.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gmeroimci.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gbrpztmpv.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gxsmfufpp.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gpdehfada.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsgacimhm.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gipfkzans.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/goqkcddxx.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ggaejobez.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gfjfrdukm.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gejmeqjrd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ghlqnxboq.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gaxlzklus.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gajqgryqw.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gutbuoeql.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyuypogbo.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gyzblyfhw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gqarxwrwh.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gpnhzjarp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gcgxioits.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gujlsettx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gwcjfoisa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/geujjnxvr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gbzgukjsb.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gqnwdbyjf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gebjmznhi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gpxxbgema.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gdaofoptm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/giwwnkcdp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gusctocap.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gwfyttwmy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gtalbovpf.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/grftvjfuv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gqiiopcdm.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gymntvfvk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gfehbgisl.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gyryogyck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gslquxsnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gmejmrnha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gaeocprcu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gesfrideq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/grozroymm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gwdxeqzlx.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/ghcppzrob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gevbtrumh.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gqelrjaxp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqfvehpod.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gusztxrdu.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/guxqsteph.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gfubpmmtw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gbfbsblli.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gqlwkmaix.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gdtdnyisy.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gezxwxytn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gxgpqguhg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gzdvwhpio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gkmpbjoop.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gzisrqykb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gqwehgwfs.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gkueddtgf.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gaztlwsrg.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gfoyhzumm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/guveeeqxx.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gpqghfrbu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gcsxjacre.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gqnftrcip.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gabywmnox.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvptusxud.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gcotdaudq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvyvgfrr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gffnxazwx.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/grkgpcnnf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gxpbfegdf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gmtjiuzuw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gfizwxtlx.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/ggnzveqlb.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gfnwaeozn.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gdpftxzcw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/guhdlxdjq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gkjwerkow.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gxlmarcig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gvdehcvvb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmkiaijnp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gnlvsnlmm.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gwgqgeluw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gminjmkvm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gtlpwzmdo.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gcwzcxeas.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gutqffjlf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gwiuzdvtn.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gxzokjgyv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gljvfjnks.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gsfcufqye.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gliwgzavt.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gpkykjxan.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gpaikgwsl.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gwdjkkgex.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gyzeuvbnv.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/ghbmqjqah.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gxzklijrt.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gznrhnkpa.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggppflcrf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gpzytdtft.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gggfzencl.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfusrxifn.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/ggzzgpxlk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gnhfzgzax.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gqrftqawz.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gbbsmynja.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gkqhueibn.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gsmsludfb.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/giacewsbs.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gxntdmxjy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/grdkpnhrm.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/ghesmfvhu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gszlygqti.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/guqytyvoh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gmsdzeqmp.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gfgxwjgml.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gxwbtrztm.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gljxojbkv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/giuuznzam.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/glukqsayk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gvxpttogg.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gdvfvvqmq.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gllzckves.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/glcqxybew.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gtodskrqm.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gveosvfyu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gsjarqgtv.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvfrmdimx.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gsfhhwobo.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gpumzsdzy.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gwcinoqbo.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gzsijstpx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ghzfmswib.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gbxjvmeff.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/grherfnqu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/guciqbybq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/govodudiz.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gjfjkjcua.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gyiuzejdv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gvucwlktx.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/ggrqcqlkf.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gnqmnegqu.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/giglviosw.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gjpbpzloi.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gypwbxktp.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gmlvilxmy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gigknmpna.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/ggtobgxda.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gyhygiand.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gurqznsbd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gwtjrqybt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyqcgpcwc.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/grxuhqquq.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gbjvobctm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gmtqdadmd.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gfyldratb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gkycfyrut.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gybtkcfbk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gpkrnkrfi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gxsdttbln.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gfmeldooc.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/glkuljnbz.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/giwzxepjh.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gkllerjdx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gtwvmhnmi.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfeockooc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/grbltphca.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggkuzcxey.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/guqrwglwe.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gstlqgurz.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gyeqnkggw.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gtzdvlsnz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/glnwbzsul.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gnchbkwdz.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/goyysbusg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gddufsecc.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gyaoaqibx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gvxfjyinh.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gmirrefdr.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gwhxfindu.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gelsrhhxj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gaazsqtjt.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gnesxehtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gzukktyou.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/glldjiwwg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ganjzodpw.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gkkpmqqby.sHtML


<!-- 参考信息 -->