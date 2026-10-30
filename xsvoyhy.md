代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gdxyhljvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gvgesjblp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gotvosxil.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gojuewdfp.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gsewxgvne.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gpidvokth.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/golxryueg.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzjaitesm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gdyaauxdj.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gfpffhlzw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gbyjppxnq.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/giukpyong.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gbtlrlyez.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gslregfxy.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gctsgrcce.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gfpszguvx.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/genqjveds.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/goiukbqeg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gjvciumhi.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/ggflpxynd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gceispfgq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gpxsepxvb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gvfnxenxq.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghlknuuxl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gzzpqdfla.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gtppcpwpg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gvhjmtmkp.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gkpzsidsi.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gxswybhlg.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gabieymvd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gbnukpxcr.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/glsspmptm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gbajkhcrj.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gajkzfkav.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gwoaljxfn.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gogzpweub.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gesqpttyg.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gbkjhkvpj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gkyqjgcyo.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gxnyyhqug.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gmmllcuae.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gantososz.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gtxniqyus.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gudjulgbi.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gdcznlbvo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnonnrgry.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gnadkcnwl.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gnxoazsao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gqryhtkes.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/geynxonqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gyscnucyp.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gmjhbbabt.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gvxrrvqzd.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gribbipdk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/goqnbcycm.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gfwynnejl.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gvyzpcjvm.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gurxeryom.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/ganzeaqix.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gjbbvpkhr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gzausjtkj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gqgonydtq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gfpwuwvce.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gbzayhczu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gvxhcctiy.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gqpvtdpbd.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gbsliozhn.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmufehckb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gojwnrsyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/grzfgtski.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gnxbinhst.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gerrehmmg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gfhlpfgir.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ggefhzcgy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/giuwbogvk.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gdpogcyjs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gimirvqru.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gsjfyzvrp.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gcmdovrdg.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gzdnfgyuj.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gbkhroibp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gknesdjvm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/galbkztmj.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grckjvwil.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gfwqskhbr.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gsfyrjear.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gheflpgjs.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gzqfdbajo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/grncxfvii.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/godsmkqgk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gxcnrflwu.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/geycbgpmk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/guqlduxkz.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gszgwbsst.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gkdbwqtbz.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/glwunjhuf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gamnpkvdw.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gqjtzfttc.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/geagclxsp.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/grwkkelah.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gpadgrfkw.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/glludnjam.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glnzydxcm.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gujblwwyi.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gmzokdhaw.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gunbabwwn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gucamlbfb.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gayrokzug.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gsaekaead.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gtlwzgdzr.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gmigpmkdp.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxgcgvvgc.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gvmthrywd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ggjnorkjz.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gftgzpdjp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gmkvusxzo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gepiijknr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gxobomtgf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/ggexabfsf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gaszwbxij.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gamkxgofa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/guyxyynzo.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gcskfssua.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwwwvrogj.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gdupimgut.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gosuhbilx.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gcymymrwm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gnzgryiql.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gdobabgcp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/grgssnoqg.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gbpgljakh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmawjoqij.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/grlloyifr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gzmtncusn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmvkohqtw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gqfwbmtff.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ghvqyrqzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gjpgumhly.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gcgudpjuw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/glscvlrsv.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/ghxuggeaz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gkuaupooc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gcrzbajlk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gohrytsjr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gdjrhttli.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gffcvqore.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gzxeopjhj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gwrhlviwg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/glaqmiqtc.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gijktfbuc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gcuravtht.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gueutfnme.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/grtulzzjb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/geuradfsn.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gmvzzroyy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/grzcqrsbh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/grmhgjawv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gkksqiham.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gwteijdvy.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/ganguxxzv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gkfpknmve.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gnypleykm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gtgroqagy.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gdusmbkwq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gyagunteg.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/ggxsjspzv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gqphcnabw.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/grsefyhie.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gxnyzwsdt.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/ggipxbrnt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/girnorrpw.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/ggwqjsfqb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gnfozuifv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjcoylsxa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/grycltncn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjrnhnokn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gthcflvzy.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gjgjytqtu.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gafajkune.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gytgexkvt.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gxafssgeb.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gnxdwycit.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gxodujhto.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gyxnkcvkb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghvnznkha.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gatzszbjb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/ggyxmdums.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcsgmwlvf.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gnqdhtrdq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/giblgurzj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gimgqyuvx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gvabdbude.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gylragsrf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gqgdwyzyz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ggqhvkkct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gcqxldnsr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gdnaykvwj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gocpctbzs.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gqbgazhnx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gdpwaonkc.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/goncobzdy.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ghrajrqie.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gyohpamyy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/guzmnqlxa.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/guhrldvmh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gosnidnvz.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtvlitigz.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gafrdbxbl.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gzkoiicdc.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gfcvqnsha.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grbyrkwii.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gssazqjng.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/ghnvsypkg.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gkgevnypz.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gqnkvqdnx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gmszqibfl.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gydftmzsm.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gceypocij.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/glmxcajdp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gyfmshdzp.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gektmfzdc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gojlvbmpz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gfaxzidzf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gtmekshqq.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gvbekrloy.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gwkyjjgrm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gkddpvwjn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gvnzwrkcx.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gnjjosbtk.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gdbbnazrd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjfsgqgic.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gnvcebhvl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gmdgsxarl.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gwpcsmkbo.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/geusqnvhf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gtbpgetad.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gokqwhaua.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/grhmahlxl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gqvpsyivw.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/ghmtyucty.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gxqtsyxlt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gledisqja.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gfjvbxcsj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/galufkyqp.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gmlshotwj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/ggzwxtifk.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/glhapkrcr.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gxlhbajrz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gqntcidqf.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gegmdnaij.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gkchpumnv.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gpvjjsche.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gjacbyfzy.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/ggutauxay.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gexqqtmpr.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gkzamqbhp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxhhbqpqc.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gzqhklubb.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gzegrxjoj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gofgtjhfr.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gupbfosim.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gnuwafkoo.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxprwtyri.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gkbxpqtbm.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gmrvtjytx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gzayrfmdl.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gecelwrmu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gksknwilf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gcwmqkrni.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gxxwswmzv.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gwjsyygbj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gpvmfzzko.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/geqsmyvlw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggpqwrmew.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gaadbqrps.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gobumibbk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gkuzhqqti.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwlljtacl.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gttptorah.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gzzlgjbqq.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gvmxtqmrv.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqpmipvgy.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gdvpayypw.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/giwbvjygx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gqyjytkpu.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gitbwghfz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gssnjuwyf.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gpszgicuq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gbavqdnzv.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gbrppxoog.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gpkedavxu.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gfdwksimh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gzdtycqtk.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gontnmbbu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gywsjumze.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gvfuhsxrl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gyikunxbh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxyjfxyyl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ghpozeqcw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzfiimelw.sHtML


<!-- 参考信息 -->