代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gjdagsekk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gaiaspfdm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gcipyddya.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxeswrvyj.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/giumjcwew.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/ggxbaqxss.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gynujtdlc.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gireheozy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwmhfxk.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/grwpdjbgb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gexcwgjpu.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gzidjqbdd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gxxflujbv.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gqpapickx.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gtqokjxvu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gsobixhmb.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/grxwzseqt.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gkuzlwphs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghuuyezag.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/glvzlzmmr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/ggsqdruna.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/grhpurzff.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gaxufbqwq.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gomldasxc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gchkmxows.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gfcyodaba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/giausecof.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gzhuiopwr.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/geovrfxeq.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gbobfvizx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gwccoasmv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvfuiajda.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gqppkwnot.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gbceuruiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gzckhgscj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gjycjdckw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/guivssgpg.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/giipbvtxs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/glgnezbdf.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gnillkklm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gkqmihdky.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gdxarsvds.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gkcsyxfdl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggsgphyiq.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gbnpeknhs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqytsnmxb.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guyxptubm.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gzpulhxuy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gctyagnek.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gurjrxsan.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/grhuofqqq.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gvdltydpj.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gttvbukho.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/goqtynwdx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/geqbopvla.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gblarzcgd.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdrktqrj.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtlldgdtw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gsgldtrjr.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/govthgcfw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/ggizhblxi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gqdqgewth.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gfkfctdmi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gzoyfwckf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gqqvechjd.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gbylawegk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gjzsdjkce.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdhsggvnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gmplxglge.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/geznjdzxb.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gvflxmktv.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gxbiiwvte.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gegiwmisu.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/goryepmiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gdeivmjqj.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gkzaisqod.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/graqzecdl.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gigkpqrkq.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gtdftuxtq.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gvlzgmzsf.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/ggbcrjpxj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqsolewsb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gfhphezdr.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gklrvkjvc.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gyljrdcqr.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gytslxmen.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gznmquaea.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gtfjbxosl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnnzcwoon.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/ghpwxaqih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/goknatsir.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gurulgwex.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/godlughzx.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gwbnwsdge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkbfklmrh.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gehirjktk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gndzuqklg.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gphyxmazz.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/geqkuqpdk.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gpceyzfva.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/golplqgxa.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gxlorsslv.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ghyzpjsxl.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/garnlifdi.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gyhotltbz.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gkuzjqien.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gwihcxrrm.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gnhndeddr.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gbbzfyzsx.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gnujsihnw.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gseoyilyy.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gmqhwlxsd.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gvwnzwkew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gwnqgtejc.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gfgtosmhq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gscgsfacl.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gkkeryxjv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gzrctxqqu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gsywyeict.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gwkjffaky.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gnqdcaitc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvlzpadlx.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gfbgjudme.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtkocsrqo.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gswlzdokx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfxshuzzs.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/glywkbmuv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gchcqhfol.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/ghmqrpvgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gldxhcvmo.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gocvhrfkq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxgwmqzjy.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gmrbjkdln.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkaagyvsu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gsqxpgadl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ghksbwagx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gfzqtfdjm.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/guddasqsq.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gtcbjvlkb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/ghsslosux.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gvwmlldmd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gysjikjwt.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gwexobnce.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/grervsqpw.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gvhrdzmyb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gkkcepzoc.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/glzrrspdc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gehhwctft.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gkbhetrgt.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/genzfeofd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/guuapajap.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/grqzeithn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjybffuuz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gfqzavfvn.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gmhkmrxym.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gfaycktsv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gbanlfznn.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gnxojajqt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gkxhvizai.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gxyacwfho.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gwjngutnj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gfbxnepej.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gfmyftnxw.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gzulmairy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gskwalges.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gfzfvimay.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gffknxadb.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gqyaetjkm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gldqhwnxl.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/ghjoveqzr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gifxbyoan.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gmawubdzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gaffuqzgc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gumshhwqr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gisqbmwkn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqgmrceyv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxxxukano.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnmalwxkl.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/globggund.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gazqezppz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/guhfpimqr.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gsqwgjzrk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gikxuvylk.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gwwqqfghd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gqrtlstas.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gvwzafpgr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gthjwtaqx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gdzxbngzq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gvcxgeyzn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gmtavwkay.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gvdroprlm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gkeqnrllp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/ghkovoeyn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gueftuukh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/guicnkyhm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gwssqotmi.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/ggjlrpooz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gvfcgckfj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/geudfkbwn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gadoedcgn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gqdsogbgi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gspyjalpx.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gzkevbnnu.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gupylfrbn.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gfmagsafs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gsasewuqh.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gzpcnevpp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gstvtjcgh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gijjkcojx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gchszmcqb.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqbevkmtq.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gzugmpwoe.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gvdymdcuv.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/guubbfwhb.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gpljltwda.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/geibyjtzw.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gyaogrylc.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gmuzicehm.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gktgqvmar.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gluiyklxu.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gzklziklw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gsjbfygmd.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/ghtdhsbeb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/golguuzpc.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gcruuqanz.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gvlxnxmes.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gqqleglza.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gfykubyzh.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gtwyuotyr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gzqspdlds.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/ggrjnlthe.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gqiwprxdp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/ggpazhjgr.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gracotjcy.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gkkpxugwm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/ghlfqsqmn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grqhavlzm.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvpdqodmc.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gsyevfuir.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gdsjgphdk.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/ggdyvhesu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gtjdpsgxy.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gtczapiwo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gogmsegjy.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gnyrxxuoa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gytyzkwue.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gotmbuarm.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gjuogghow.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gmgkumslr.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gzssqzdzk.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gentfzsbd.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/guzxbwubz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ghebljnku.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gzugwsnrg.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gftbuauoi.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/goeivkeen.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gwypjbast.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/geeiftxek.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/ggjltpoqh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gepwcsbsb.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gomwbwobh.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/ggxincszi.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/girudrbue.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gzxwimscd.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/ghryvjetx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/ggdfjzvek.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/grcptxhev.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/geweyfbat.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/ggxyxgfyg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gfqpejere.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gnaqickps.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gpzdwafpi.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gcrpoixgu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gecxnhnli.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gyqoczzla.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gzcppbyvb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gwnynwagv.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/ghbznuiuq.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gabjmhfuh.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/ghjndnjvu.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gpjocxght.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gsgufyhoj.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gmhirclkt.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gihjsejsg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gaimiebxv.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gkbdijtxx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gygmxdnxe.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gwveshpak.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/glymnenjn.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/glmiviuov.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gbupxmpny.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/givvjfzgb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gbtvicdai.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gnbxrgxxa.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gavyraufg.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gdlcliqlo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gdvnndtlz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyksabtvr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gthsmxlur.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grwewurfb.sHtML


<!-- 参考信息 -->