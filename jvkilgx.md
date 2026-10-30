代发 wailian999

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoqwytny.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxdixxla.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/guvjeduou.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gkenjhrxd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrqddqgp.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gfzrmeahb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqikhgabs.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkajrsb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkikcmav.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gplztxagk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrgslacv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyamktkss.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrggdtrp.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gohkqwjqr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhmfmncu.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gitpssiog.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwimrnrpi.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpolkibo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdljobnbr.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwkpykpu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/garbtkhjs.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gzqwbcemh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/geivpqyua.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdygvarm.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gsnesbdsd.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/guuifktkd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghmqoljql.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmecixbl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/guwxwjbpv.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvkmcghsy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gzwuwklac.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsubyzpc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gornjwvck.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjpfrchc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkxtszii.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/govomdgve.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhwcrbvx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmlgtshb.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gtcgjjzjc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbfuiou.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gxegwwscb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzdyaeftd.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoozuqrk.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gztqclpkf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzeyvyrp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gupigbehb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gitcovrbx.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxrdhnvo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgnwldpm.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqjdsfvtg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwkvrpzl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvuenncd.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggboydalj.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifvvfsdg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcefjgzig.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpeufyan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorybhnoh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmqkuslb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeshudez.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gndidsjjm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gcnvdzrrc.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhcxate.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvkjqiay.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkwaedju.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/guojorjdh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gopscwsxk.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvgcgzs.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/goxeqpltp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glwsqiehc.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gentkekan.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gengymjdk.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ghjooqrab.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpwwyzjm.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gayzksnew.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdiyztqu.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gwxxbxoxz.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gsemhcppo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfckzfytt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gsgxnlfvs.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgnhboec.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gioidoqwh.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxiporlqv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflhturcm.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjeqyusv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaddzulai.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmzpcvdh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gstikgpya.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/guanwbysu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gsbniwews.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfgoymgl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqixwipcu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gyiuhstuf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/ganxrbicx.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gtstjuqzm.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqdxyrts.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gaxgwawns.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gebpjzufc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdeyppqwc.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gbmkwfhax.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmzhlocsf.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/godnxwoxl.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqmvvzzaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhoesoe.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gcgdjbymd.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guebpbgwz.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gubcjsqlr.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gdgufxqxd.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfxmiaagh.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeagkgsp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuvcftqp.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnjsottuv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/ghhwbwqzt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyriczrwl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gsacntkdy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gjhejycqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghtskbvrz.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdzhklk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdghlvqyy.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/geerqmodh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjpjrtjn.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gieoxyvff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/goeawaxsa.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpyqhdtmq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gggxcyvab.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghgnmkplg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gtvhvrluk.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoruqdsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpesnnqnu.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmhidmugc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwszqwyu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlslfxj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gisnlskxd.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gapggpdxn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzljkevp.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/giamcxzcc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfqmozg.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/guhpxykah.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhsnmzv.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfypeuig.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcgzulhm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookrnudw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkezoohte.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvparzkyb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gybfqvzkg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmdisjcm.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/goisehwjs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfvfnitz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghbnaigc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqhvafsx.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxrrqity.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gbmeihinp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ghimtrpcx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/graifmyag.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gtgmsnhyh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyfqgbui.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gaorsxxtd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrjlkhmt.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gikknbhuq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/glvkrtytc.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvelqupz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbvzqdecr.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/giitpobor.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcvvohjz.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/glupniuxx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/guksrucpx.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/grymxcmqd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gqcsumzbp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeapstvc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gackhxeqd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grtenelfj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqmdiiul.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeykepkf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfsezfxfs.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwsvrtgtq.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/govjdbrfz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkiwheph.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmlikkecz.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtmutdtz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgapwdrl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrjlbvzv.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/galrujhdh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/giusnfjcz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ggawweskr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gmqhwmttn.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdjtxgbul.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltlfrpu.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/glqcjwror.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggcqizqay.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfergrzxu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhdngybj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gacsbzeej.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxavqavz.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gjucnwelq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/ghaaaewhe.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqizzzky.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gypfcltia.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjbjtugi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcymiijsv.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gltusbges.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/grhhdqcht.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gsgantrzd.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwlpuugh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpomimmc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggnapdlxj.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbmwxfgzs.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckobncsp.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/guixtlpna.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gddrvruyk.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmlidkbc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkbkewmv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysjubdjv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkivpzcr.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvcjppxxq.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcqepyhgj.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gjsghwpgf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geufevaku.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/guyxwrxot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrbdrwjb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdrqkbou.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtvatdnik.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlntlhsz.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjedxzvc.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gmbogihin.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfialyub.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gscgsalbt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimavhlhy.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gewalkmba.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gorxcgwhv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gulsmafra.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofchagnf.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/garfunwtq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwlxapel.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgctyffz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjprbeckz.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvtmjpkvh.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzphvebxm.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gquyphgql.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gjmbxoxyo.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbajlmskd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkvhhog.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/grcxdgezi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxxrcpto.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaidrsmip.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaferduta.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gkqwrxmqw.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/govexnbfk.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gredssaxq.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrkkmpnf.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gcjchpvoe.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gigfbhdll.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gmavauone.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gnszetqkp.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwwsehwy.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbymbodhm.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/goxwqihqd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpgeknov.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjpsznra.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouqggesf.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbryjjzkf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/govonphyo.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghffjgsgt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywgisaas.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjipttpy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrjcgzec.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gsvixlxrn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqfmpcma.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grjfzhive.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwupaaql.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfevxwqea.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkkwklwy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gibgpzkdx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gricvhnam.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnqeyerj.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtsdtntfy.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwqjuhpu.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoyxdgwl.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxalfzom.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gihvmofvk.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvqysiae.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbwjttxz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gleljcpox.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gifdvxhyg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwodajjoy.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gotunbhjo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfgtrasn.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxberxyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqltlnqso.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghkqyirum.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gidqcwcax.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurtpglur.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvlzard.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknyjbact.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gmasfzvpv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtfyjyy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuszugft.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmmfejxrr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibwwaxxx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrpmgmzg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgqpxhmq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynmmamtn.sHtML


<!-- 参考信息 -->