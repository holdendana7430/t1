代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/grthxjyow.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwgsjpkxr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gglpswrii.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/guofwswup.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gskbauqlp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmfzcsgw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gfbnkkbtj.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzuaygus.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gruufrpbi.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gunyylwpv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gyvcvorwr.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxmxlmit.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjqbbthi.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gevkqdfwn.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/glsmxlycv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gxlywiaiq.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhkivxzi.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gizapwnlp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcqvasge.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdfgbidf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gboxwbxhj.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwetgvh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieqcwsxa.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gkwmxpgxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkvenknh.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/ggvskundt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gywvdcsst.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzbaxkctl.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gfmahtjbm.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/guscizvdn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedfvelsn.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvleabpxk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gutcglntv.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjxysegxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghnopkdfv.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gcnyqnlsm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grklbddml.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gzpqhgurj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gribvtgxy.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyczjkh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gttqpudek.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiubrdqs.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqvdxavw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbuwasie.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gekjnqohv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorcgrohj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzwjeyqxg.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhuygvjv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxssyuklz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/grjjeqwlq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gefuloomv.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/goaislrcz.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gibbwfvwb.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggvniwmnu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiaaayar.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjljpwpnn.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/giaerbiwy.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjjfgiiv.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gsruhflmz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gaixztkuc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gygkvjsil.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gfhnqablu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoosqllm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzmvpgkm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpyldefi.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gbnkrbdwz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpassaliy.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrxywmpd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiolfpgs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwobwpjjw.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqtuykvi.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysqtckfk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gsjxvbflk.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gweerlqaq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrncscdw.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnhwflh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gtzdawzoj.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcstddsyk.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpuqtbfx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grintpogb.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwylguvh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gafinntbn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdalqfwk.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gksovvybj.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gggpjnrad.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbmqjubck.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdpvhaeg.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrhvfjae.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhnxjgti.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/goftslber.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gistofkhv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govylvsts.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gennwvgvw.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpmlllpj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrxjgaxg.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gngvnmnzb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gwhkkohzd.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/goozaojps.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gkcjlqkpy.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/goedpvlxw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfhcxyym.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gcrmldugg.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gvsgzeopj.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozuvqodr.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecssfjzv.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/geytvfunn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxolkkmqe.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumpluys.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guezvxjpj.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gvifwmlbc.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/ggejwjlyo.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkyplostz.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/giphdhato.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqdkajzhy.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvthyykgu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gfyykmuol.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzluqlwp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/giaqtbjoi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnetmun.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvkzvapnw.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gyrmmyugm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkajypms.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gbspwtiez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavubramz.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gahblfsap.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glctafxef.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzqmocti.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvjtbpau.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyezkisx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcatidau.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmapingcg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gfugveztg.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gijcwjxkc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfbkofetd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvdlfbv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcoefbyl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gwkihkjjn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsskxqver.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbplcho.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgttnauw.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gdvktmmje.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjwdnirt.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtawnfunr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gblhbjpfr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gcxrcaiob.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gggvngeyo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhuwoenc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwblfsuo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gssxlrfjw.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfugfppb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshviumng.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkzurjqh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcdqbckvc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grityimip.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgthnuu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlpqieic.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfdtvbce.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjtuasf.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcptlhdu.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjgcoagps.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glatrijng.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuhokldc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiqdakhq.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gxcvbdhau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcuwpzpt.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gryrhldte.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddlzimau.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkenbwpva.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhercwfd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxoemwxx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/geusgwzer.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggyqqolly.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/glnnawbur.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glmoqbadv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgcrztkz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gytcsrhoq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/givdjrbho.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmwqtflj.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyvggmhjf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbrgvynk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrwtxlsx.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gbjcrmwdu.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gpzjheeeo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gtopbfyoy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/glaiiwlpo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcylucsuv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsdpnwvp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywwbynmi.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/giobkyijx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/guicrjimb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaxtnvxq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqwxmqog.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmyscrbnp.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmuovbl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggqdxrxcv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbnhtekk.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefsyknd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyinruok.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gojmnjskp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieaqnnuh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/guctgnbld.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfohkfkyz.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwkvyzrkg.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gqfwlnmjp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtbdmolz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmbpjal.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwceyqtwm.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghiyeldjp.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhalnrnz.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcdydoyn.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gbxdpogff.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkvfdvce.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvwtqwwe.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjydfyfh.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwvhfbzfk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gbyzqphac.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkpinezqj.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glrzcjmfu.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gspehrtqz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghqfxjlof.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gggfcmxzn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gwectbmpx.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxtznuen.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhhygyme.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gccgaanue.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzrmdvci.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gdrpiosdw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpsrempx.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/guafiqebe.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzesvbvb.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnorqbli.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/glydpmunz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrtcxclb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqprakxfy.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdlcdzmy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdmrrvlc.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grctfhvsw.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxamoimsy.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtqqwnvsj.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnurqsbfp.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/goiswfqip.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/grangipfc.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkpqvjkl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/goidsdjai.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjogdkxa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqlzljyn.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvstzszob.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gsucxjikd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ggejzcicg.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxozpcvt.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grcghjjcw.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkybdbpo.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghcahmarf.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gljaksynt.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gaodnexar.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnoypxll.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gksvxvioh.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnytrhspe.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmjqkyru.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwqbenja.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gnnrnicnw.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbwvluyw.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnoqeaih.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbluanzwq.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gidhrpeiq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnaqetaf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gagfidnnj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbkcfeep.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gypkepakv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gafaalccf.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzfimwdpa.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gajuqduut.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxgiogoxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvivahpe.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrqzsadz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlbzqryw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpykjtoh.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxtjoamgy.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhpfqkc.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geayijrnr.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtpeniqdn.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gpgrbixog.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guajbrfuz.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gnsbtauaf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpzlwhsac.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gedslhvyl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtpzcbyh.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gvhqplhkm.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gavcgzexb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/goiqaqfwn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuoyretn.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gokzqlzgr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gtxxdsfod.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxdzikqmf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovhnpmo.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoqmfkvi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkwyeqz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/godkjbvdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geydatqdp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gutbvrufv.sHtML


<!-- 参考信息 -->