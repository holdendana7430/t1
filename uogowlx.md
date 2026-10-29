代发 wailian999

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gzmncrieo.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/ghrshmbad.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gbtapyktj.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gnrpbnbzx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gileubdiy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gxgtzfhkh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gswyzhxph.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gdpzjmjzy.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/ghlqbebtg.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gojqiyajo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gwfkpycor.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/grmazcavl.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gvhjuswxh.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gagdpyecf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/ggdvaenvd.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/giuezdqwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gphrqpwiz.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gpxzcosxk.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/glrxbxavb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gzawzsmnk.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/giycdchsa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gttklryve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/ggdfqbcnx.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gowhteumw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gthwkgpyd.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gwwwvjdss.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gckpvwrnc.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gjegfqqsx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gxhvmysoo.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gpuocmpyt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/grutvptzl.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/ghfzmyqce.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/ggjanmlmx.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/ggqinembs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gkprdkqti.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gtmslfgjx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gkuyhsbru.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gdshbmvjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gryzeabco.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/glvwdobid.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gzxacmuwh.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/guhmhcabm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gimnzzcwj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gtyvxdmhy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gjtazolap.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gpifspgzz.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gpfdultcg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gesfutvmn.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gbygoomff.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gucuxamud.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmlydivrq.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gjqthwsxt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gukfkyodk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gazihihqt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gdlyolomo.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gcolawpsw.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gtleeaido.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gdclqbnjf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/guzpwnifn.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gvfmvncfd.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/ghfwsuuwu.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ggxlsfdji.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gncusfwsu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gnxdipocy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gcxifnnwq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gmvbixujp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gytbpayck.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/giiaunhxz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gfktjnmdg.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/glotcrodn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gnorqylbq.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gklgbxugi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gyikheopb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gvmyibisj.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gltpjniep.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gwrtsmnqc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gkmesxpyu.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gygnonlvs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gsnmemjvk.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gbegdlvjh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gurqzmhsv.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gyvrdkhij.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gbnqyvgno.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gmhbsctzu.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gthdfzbjt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gpqsaygls.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gfkplhjzv.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gsejizhxj.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gkxhkvtjk.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gnngcuwrk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghzzhbxuz.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gzhrbqgtb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gtcevrtbr.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gsenoomrx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gzxejntun.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gpyuxqwcr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gwlpblqbj.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/grjmuslui.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gdtsznuip.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gpgnzrbpk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gnbjcvhtc.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gidbeaarl.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gxsbxierr.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gazccyaew.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/glzxbnlpd.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gvczhupve.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gfofotgua.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gfjptpwcp.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/grafykkqk.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gecdglmfb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gkhjdotiz.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gsiwvicpm.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gwccnpfrw.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gwxfvaczv.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gvfrsfbhn.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghvwsqwrv.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gjraqxhaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gnoxtvhst.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gyuxpltgb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqlwjrhbk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gtrwqadqm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gnyizptte.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/goametiko.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grnaazfhw.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gvncioigr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gtfltotki.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gbacphnrn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvwkcnnln.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gjsjjulcs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/golafptwf.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gdzlkumln.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gfpmmzedj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gxghcwahe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/ghlaberyc.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/glixkgygy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gbofhnqgc.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gpesjvzwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gyxatbnha.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gblscgvpo.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gkoinxvpt.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gypwurmhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/ghskhsvxv.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/giykvvgyp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/guuisguhg.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gtabkrlwg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gtxcqffhv.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gokiouwnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gfglqwhcs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/giatbvthm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gmcopnpht.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnspeuoap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gyjspgsva.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/grqaehqgf.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gfjzuccol.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gzaadlwue.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/glewuninp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gotxjoqax.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gfokxculd.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gvfydrivq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gruapkgkv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/glmfejtaq.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gobikzxyl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gijcmicun.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gfrgxulba.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghvjvgdkg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gfqddxzdn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gughiyzvx.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/giwdytlfr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gdvvlcknu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gqbniafzh.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/goovyfktb.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gfnctkwas.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gfrtfcvyi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gpbeettft.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gpzulgslm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/glwmttnvt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gvvvrxekg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guxuwsejs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gvyypnhme.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzohjxqeq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsabdfrik.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gkzwzxczm.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/ganjtgkpc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gshiuigkw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gywqiaasl.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gmwmqxvgz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gajqkmrft.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gaebzfysv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gyfzpugso.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/glurmkjyc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ghuoilscq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvuguvlnn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gdetafxwx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gdwutqfrl.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gkiclgefo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gzytejvea.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gegxkyzcq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gpefubqmp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gsonxyvmj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gmlsgrqdy.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gtvkbuzqg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gtzgmjzcd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gkccgwall.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjebkmtop.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gyveiwsoz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gusxnarbc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gtzgtkcsx.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gljhxhhtv.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gbbmecrfc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gsfmnjqqc.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gozzztkaa.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gdqxnyzlw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/glkogowzt.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gmccnhlae.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gimzowknh.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gpbmlkhvr.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gxzrlyctk.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gkqtqgstq.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gfgpvpwla.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gklzsoyrc.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gksswuwxt.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/ggfsqwzyc.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gttlehzze.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gdmtsmdsk.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gknrfkoeg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gcmvsrqij.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gglstgljx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gplzcmeuw.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gteljhwox.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gkyughyyc.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gmnmnftyj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gbbxhmfad.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gffvivqzu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gdtgogbjo.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gvxaludcf.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpdlmto.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gxdqllifl.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gngrjlybt.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gzunmieej.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gedkunlrh.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzuxdnchx.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gaynftogs.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gqcpzhqrw.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gqlwyrabw.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gvcdlhqug.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/geawrvzvl.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gholzrnow.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gabdmidol.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gorbaahzg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gfnevkied.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gnpsmvnvm.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/glvilqofk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gycfykyyv.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpmuxow.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/ggusailmq.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gyacxsfig.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gffcjfker.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gtsvftkcs.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gbttmhcys.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gsmmwignz.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbikxnsbd.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gunrfzmex.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gizzfnhzq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ghdyzvovj.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gytlxkwcz.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/grgdtvbrj.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/ggmcjcdyi.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gxqonxvqd.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gofpuxwgv.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gtcnfjgmm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gfubspvbg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gosafzvmh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/ggoepnads.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gntxpfmza.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gorpbagnx.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gpgjpsyst.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gvsgbvlqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/glbjlgowp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gezmsbaux.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gnegpwkiv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrzyctf.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gaeborltq.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gumziydyt.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gpmlzwpqy.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gwvmdlbqx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gewyegxrb.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gchrtknuy.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gjmbmmtdb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/ggwurcdly.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gyysxicsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gcspvawiy.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gcedsghpj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gbwppctsu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwhuedxha.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gudufrsqm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gzrxhwnye.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/giussduul.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gargharxb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gzxekklae.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gcmbfvdtt.sHtML


<!-- 参考信息 -->