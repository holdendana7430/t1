代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gmhxboerq.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/ggngcsbnm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/guwgofzqn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gspqywmxm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gffdfhqax.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/glqgeeosd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpwaxfmdg.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gkhmcjukj.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gaoamtnne.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gkbvbhzgq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gjkndyiwj.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/getoenxoc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gdilynrep.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gvowgqpnp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gakjvbqqr.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gfnqolojk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gpysxcctq.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gsfqivgba.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gofdcybds.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gdikepfdh.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gmhogeqtv.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gmftznmsq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gcvxtnmme.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gsgzywecg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gyjitceur.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/grsdzkisg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gaaxhsyaa.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzfcjpfhi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gcquknymv.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gwormzpez.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gfumkjrvs.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/grkqdygsi.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gdvuteqng.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzwjzlacj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gjtvethod.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqulpjm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gsuihuxsl.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gawzbfqia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gvidlwazy.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/grgahevnh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gwcjydcer.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/ggvakhkeu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gdgyqisja.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gtdggyftd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gspjrjbkr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gbillrfxi.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gqmhtwudz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goliafqbd.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gsavaahwq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjlrwwxve.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gpwpgfchp.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gexenmiro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gefvkkmmc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gtbfcdfec.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gukdlcfgw.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gffapyynd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gbfetoobm.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gggmqcwmi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gxzrmjkjq.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gtfwkwuwo.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gfbpmuuby.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gkvjtrssk.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gyefgnimp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gcsljsnpr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gojmhgiqh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gcrfldbmi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ghcyobqqo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gquocrwtj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gmmvjjwfh.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gsqjugcqj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gspclybii.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gedxbeulo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/getjxgwxd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/govndumxl.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gsbhptwsk.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gmrveecps.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gdpeuqfod.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gnzpitqdw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gmhcvrgpb.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gccylybod.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gmnmrokcu.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gmxrnygqi.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/glxfiispi.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gkldyycyb.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gruesdeiu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/ghktwdkyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gkzgegaai.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gmvxmchfh.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gvmcgvhpg.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gdeebzhyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/grktiryif.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gsucipaza.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/grsjhgzsc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/glpuldtqo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/grcnkkbah.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/grgagwzxe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gfocwtjpr.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gowhjonlb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gvwuirjqp.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/ggfboapba.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gjqimvrae.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/glmmlqszj.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/guonsszgr.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gvufrgjrg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gihyeatrq.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gbmuflkpt.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtfktpcnh.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gquyllazl.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gcufdngkr.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/geamdqhuc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gfmvzmbym.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gzrdjfwle.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gkjdyfxes.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmszyqaan.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/guniwaawg.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guqgmkpyd.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gmusmrhtw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gylqeyjli.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/ghboahubb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gycoseugb.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gqryvrdjz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gminajgxa.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gmixhlpnw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gxoevvpum.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gyhbauckp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjybaqqas.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gmyorbglo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gohxecqld.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gaopvohoh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/glbzzicmh.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/ghracaykr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/giwchwztd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gjmncdmsn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gqgbddiru.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gkcifnhip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/ghmjagmor.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gvknsjmqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gpbsofosc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gflqgkbhk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gxcqtijev.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gjfgpnlph.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gbhjswked.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gfvvxafxl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gydbgxneu.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/ghlgmarzx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ginustwhz.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gitsbjhzv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gqziztkzk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gnstnxmio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gqglyevwi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gghettafm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gsytsqepo.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/ghycbpppu.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gqtnfqokq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gymeonbhi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/goybznwrg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/guayelfnr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gsqxwnjtd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gxexzwmiq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gluqgqhrb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/ghmxxtsfs.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gmwwdnifr.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gnkbdbmul.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gdpnxqfkg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gnqnoeuzl.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gjkdwjknl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gisepsyvd.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gllacbuym.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gquonkjku.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gpybklath.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtdrjvgvw.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/giaxxmdar.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gkilorsnl.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gbmxrbvzd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gfseisriq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gkwkshhfd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gmyzsegcp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goxdibhui.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/godyjyfsu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbczefftf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gujajojbo.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gwnnzjhbd.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gbtjghvgs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gcnjstbvh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/guejwjwus.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grliurhna.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gtqryhrxw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gicwvmshp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/geafrfulm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gqaitejcd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gndbpxvik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gwpdylhsr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gplegulim.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gbroujlsd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gzmfipmay.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gnepdpvfv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gcovwzxvc.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/glpmspvsf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gfjjqgger.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gnbbhbkis.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gzndhhxto.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gwirdvhsj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gjigedpia.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzqdiaixs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gnuiwbgxw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gxhrnloaq.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gxqwlwvxc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gqcopzupy.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gyvjnfimo.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gfqlwrnvt.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvfoynsdw.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gdhaabitb.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gfkxmsxxq.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gdwuzcejq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gyzbnulcc.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gthdzzypm.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gwamsuhff.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gmersjeiy.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gpsxryvjg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/grkjphwsl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqhbixjwp.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/ggmlkpmsd.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gsrjryigc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gagbgexez.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gozutrnyg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gqlqrcgsi.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gytidkfks.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gtdtltbgk.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/giuqksrou.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gsiqyjqxq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/guuhrygcs.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gnmuokdtz.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gntpwfylx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/ghoafaunp.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjfxfjehq.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gzthdezag.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gunpkmngh.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/glrfkdbae.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gakhbupkw.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gndbiaoef.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gjcihavgx.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gzrlmudxi.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvatzfzeh.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/ghodvaznt.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gzkpcbtao.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/getnkwwpt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gfclvhrgb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gsohcffyk.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gqhrqbyfr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/girxkwnkf.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/glajtmvyo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gymelhlvb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gvdogqjgq.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gtqktseat.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gdxcszbqu.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gyxxulclx.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gqqnvamuk.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gzoqxdvon.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gyoiqsini.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gjmapopsi.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gageykkfp.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/grgaqmhjt.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gitgfswum.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gnueefxmj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjuabdedw.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gbdcvowxi.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/guwfgypsp.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gulmwbckj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gojvkwode.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gsbhjxizc.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gxdvltdui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/ghrgietsp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gtxlgibez.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gogwkwqez.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gqrxjsyvi.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gkiuwxumu.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/glujqdtjy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/glkhnxrai.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtxzghrqt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gxsmsyzvk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gushakujm.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsjdlkejr.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/guipymfpc.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gfzmmcrja.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gdnqzsvuy.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gbbooorey.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gfzbltdir.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gxbsqpqmf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzhhvdzox.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/glnkxjtwa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtdczxtbp.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gjnhiwavo.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/ggcemojnr.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gnrnznihw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gpzmqzvzi.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gwkoultsk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gfiapvlot.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gmzecbzsw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvphfbrgz.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gbeeclxfj.sHtML


<!-- 参考信息 -->