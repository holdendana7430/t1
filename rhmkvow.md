代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gqdhdzneu.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gwvepxqso.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gzdhwaull.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ghndrbipg.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gahpsknxm.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gcqwgzrgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gwnkshwgt.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gbughttdd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gajkblsqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gcyhkaoke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/grzopmfkg.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/geavxcfxf.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gcpavzony.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gezgwdjzc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gaxdmuoja.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/ghkkfnbgu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gvqqdwney.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gxawwtrsa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/guyzplpec.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gwxndscvp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gijzburyz.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/ggnphxmri.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gbbfezgkj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gbqbdmxay.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gzyutoagb.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gtyvfcvvw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gpezwicpq.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gtglcvydv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gloawgqct.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gmoydthwq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/grzdwilfh.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gzxspbwvg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gpgrrxsjl.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gojdfkxmu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/guetuhavr.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gnpjtzxvq.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gnlwucnkr.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gbziigbgp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gsdnbmdqc.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gvvjakuhy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gdntncsvv.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gyrjjsdvs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gnganhgdh.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gkebbthtn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gnihckggm.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gyrshicuw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gawcdtmvl.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gjhhlhxjy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gldctpcei.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gegbwyhkq.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gactrpapo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjrjoqywi.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/grdnqpgnc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwmyhdpcz.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkblxxzxu.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gbvuwalmh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ginisivnq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gutlxjwmj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gdlrrrqca.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gjqosvcad.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gcbybmnsf.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gfuykanwb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gcihnvjdq.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gtkroxjpu.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gvwgfozun.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gsojtbipo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/giaymnvsi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gyitrkvqp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gkkbrhuow.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/grslmulga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gvhnkhikf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gtpclkhbl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gstvchfpt.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/ghhqaxscs.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gmpaejqtw.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gcgoxtngm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gixgqiylt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gpctvwfdt.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gfzwmbiri.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/ghmwtncum.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gulxfpasc.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gwkxvvyda.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gxoapjihy.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gacnqsczg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gdcgwvwov.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gszbrffsb.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gyfschlxk.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gohpaupdc.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gdbaqblht.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gkyqnkrvy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gnizkrnqe.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gyekhbeeq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gzfjietjh.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gnmyktvmx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjhhnzqmo.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/giapsorcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gervdalve.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gdpxtrqge.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gvczicxva.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gmncbkyuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ghhasrsij.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gtughutwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gsdpoeksz.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/glppmjfjg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gycdzontp.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gnrqgdopb.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gchfsufzf.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gxxkvcprk.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gzeechuot.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjxwpvf.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/goqsfioic.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/glunkxoyd.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gmlovrvae.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gvqsrbmsy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gbhoxtyua.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gjdhspdvk.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gibdoiipc.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzxczylta.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gyxckcnnp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/govirbkmx.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/giexjcnjl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gflsmpbxs.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gxnleskho.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gghlsanrv.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gpwxulscn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/ggomwnrah.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gnnubspbm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gvvonodkg.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gupjyjcme.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkbjjmlsa.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gactymonk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdbnorzsq.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gukzawofh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gnnnpatjp.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpktzszcy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbcgbgcdd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gkxgxwnoe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gzkvskhnn.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gwblgotgr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gxrdmjuvl.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gchwsowic.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gbcmiilfx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gfhbbenwc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/giwxmahzk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gxwjthtwu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gojsuawfb.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gpinbluws.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gttrbipzn.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gmlywxsts.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gghgszopp.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/grewhfmid.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gqaaebqnq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gjyqmbjbv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gslztqjxu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gucemvjva.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/geurxgqcj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gwgawjnjj.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gunpbcocy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/godmbnvmk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ggkdkybcb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gksndkzss.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwdjvlrnt.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gkmwtkvfh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gpsbcmlee.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gufbanqgo.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gianwkjcc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gwoaqycbi.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gvipbmruk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gddzhqbwb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/grbruupxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gizadgejx.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gqdoqwhfx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/godmppjyu.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/ghdxcvdgv.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gknlytavm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gcibepxbs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gkbyjzquc.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gxdgodrkc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gggwnkjwm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/glyengmdj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gihtglcsu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvocglfvm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gvegkdgty.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guhudwmws.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcziqgbwp.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gukkxykmf.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gdulibuzu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gwlbjoshh.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gabjbkqgm.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gxxxyxnjy.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gmdxtlytj.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gouqpqeof.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gjiuyfapj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/grkwxtvmo.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gazsbpypa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxmqdvlsp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gudvzloaf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/grchwivzt.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/geccnlgnu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gmhqcsbfm.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gmcdlpfwy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gguxafjbl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gplvkjvlp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gmleemqrl.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ggxtthfgk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gavtruagf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gojsbqjyy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpqucbzgk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gygnhpwkk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gsmpwngib.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gyebabsfm.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gndckarhb.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/guqjsndhb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gaqwlqvbs.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzmkuhvrl.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gejhiyuwd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/grqjqxyox.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gxvvjjsns.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gtacwsooz.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/guoidirrq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gspvqujke.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/ghznrecld.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gomwxgpfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gxsuogwml.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gfzfrjzun.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gmcrnoqzy.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gneiwwszk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzvflcw.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gcbjkycon.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqyodka.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gzbxwzjzq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtdcvkwkb.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gnjjevzah.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gdgfiqshd.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gjlxibhtz.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gckkwlgxe.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gbxarqogs.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gdwmaggkz.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gsgadjnyj.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gapniuhog.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gofaxyztp.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gvmzssmun.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gmacvevxe.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gmgitnsjn.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghwjlpfyv.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gilmhrbil.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gzwcidqdw.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gopcaxdeq.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/geactvums.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gsbvmadht.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gszxiqmkk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gofmkwljk.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gfvynhpvx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxiqdchzq.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gjukygtje.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gqyqevqgj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ggcazkzmy.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gtzxxhpod.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gjyzdwolr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gxoztfknn.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gnjrtpyne.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gucyaetgf.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gkptajeyl.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/glrlfjwzh.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gwrugspum.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gnvadrauh.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gdiodfshj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gtzkglubt.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gcdqfqvkx.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/ggigfslft.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gwlzwjnel.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/ggdwvzwvw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gwpnyegzz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gucopthlr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gnwlqqrps.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gxpclgdyb.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gxhzvvnyi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/ghgeljuoo.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gkcynmrzp.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gpcammwhg.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gpkxbnuig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdicxlsaz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdnyugyzs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/ggoeyjiok.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/giyjclfkk.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gohehdyqf.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gkixrlbag.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gvojmhapl.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gdypywqiz.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gterzpclm.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqiwtbbph.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/ghwknburj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gxrdfunwh.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gepguyzld.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gdvseriez.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gzidxucrm.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gvnqunywo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ggkmbjruo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/grsvhfntc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gskyzfwpb.sHtML


<!-- 参考信息 -->