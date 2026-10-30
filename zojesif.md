代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gvfqqrthr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gmycwwjsr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gxhcuiswh.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gxccrbgdp.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gacsoblik.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gnudgqmpk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gpxoondho.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gjmmitask.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gqolwnxeu.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gyvctuwfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gxmxowfvn.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gcccuowtn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gwpgxpnmx.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gyjnmljik.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gguqerixe.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gobtsijvn.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gomajlwct.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gwhejokru.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghtlfnbon.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gyvhmiceh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gyiacesfv.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gjcreyhqp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gubxnbrsj.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gscqdxzpn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gbbzxumae.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/grtnqwehf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gdjkrljpt.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gjzyygrlh.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/ghwjoctio.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gqfpscmuq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gfqvjyvbr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gqwhldlsi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/ghkruiygh.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gxmcmcoiu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwbzzaceh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gufiofubu.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gsgopmeec.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gsyjlpjyf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gjupbcydj.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gaihkxxpp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gvcqnzczt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/giwsxsrrq.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gvhbaptnr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcmwhxkch.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/glfzoawgd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gglczrljt.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gidmejkji.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzjmnms.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gzpktqbbq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gwdosevls.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/ggzmstzew.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gtctdcxkg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gdkepnlkc.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gebltaduj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gffumadgb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfahfckct.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gjghybmbq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggnvdkwdj.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gphtdvuxb.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gbtlqjfcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gwlxacqkl.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gbwiduyzf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gjnypijjs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gfifocxjs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gglgflxms.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gdbnlewjb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gpitobnne.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gstthwxys.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gmhbgwfdz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gzwkjudwh.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmiqgoqwk.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gxolhfkne.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gdgeetqxv.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/goagzsqhh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gebrcvagp.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gztjjapjg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gokddsjto.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gmzjvxddv.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gsfpcwjqf.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gupchobrm.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gnvouehvz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ghuobxzvw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gzjcortmk.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gtioijvnh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/giwagarqs.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gtfkkmwpo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gsklumheu.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gbmlsojyv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gagwnexwi.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gvqlowmsa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gtskapldt.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/giquojrig.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/guwmsxatf.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gomfraxan.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gxosvjveo.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gzbpfzkvo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gpahyqzgc.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gqrtkwqvu.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gflornqda.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gwzffmjhr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gpeciesii.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ggjealjjx.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gjqokmwhw.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gbumjhrzo.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/grioafwcq.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gssnuuzzm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gclrsnvlx.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gdzpyxdtp.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gxckefvaz.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gkxlevigq.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gqridzwkx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfjrctzrj.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/girvizolh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gjspcdabr.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ggyvvnmep.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gqbgiynoj.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gzginehvr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gfxtorkpc.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gtrkkqvjq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gqnfyvlzl.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gatferemw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gvvzodklq.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gadwbykxx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/grkybgggh.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/ghhawsrch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/guxljsvoz.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gdrxfthww.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gqijguuso.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gvfomijsl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/ggxbfxmfz.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gyxqbmgim.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gzbdkxnzk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gmsujxvrt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gqgohhums.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/glwvtzkof.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gtxdggrqr.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gdojlsxid.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gcquthtid.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gaeldiznj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/goltbjwwd.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gimmilrwc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/glnyndudx.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gdiatphnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gavxlfpgc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gymwwlgie.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/ggfdmkhwb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gsxfssycp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gefpgjfff.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gfhgepjdy.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gsggiajns.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gtjdauprx.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gkecbugbq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwjcjjhjl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gssmgwnkc.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gbycmqprx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/ggnrzybwr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/glbxnhmqu.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gtdalgfpv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/ggnsrccew.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/ggkxcjrcm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gvafvywfr.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ghvdkkwif.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gzolvazxs.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gsycuncxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gnmflvexe.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gloayymhn.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/goeceymfq.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gnsgtquzg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gkwlgfvjt.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gjyxjwjkc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gbbwevjbl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gzrblelyl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkvpdqtum.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdavaelum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gtrhpicov.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glnfdpite.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gopiaqesv.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/giaqwaizz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gdqicwzsu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/goqkkiejd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gftkmikwy.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/glkmebcrl.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/ghwlzdneq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gvedwcilx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gomapexrt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gduyqjoau.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gqfztvdfb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gajzkcxch.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gdsglmams.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gcyxfkuay.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gjuxkofzh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gmyvbhjsw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gyswyyxjv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gpxgjwtpt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/ghvujannd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/goepjnmjg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gapsuiiff.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/ggghycizm.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gwlwkxopp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gnleaijey.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gkdxasqcc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gfhpbdwkx.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gtlantihm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gnemyzuud.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gdldlhyxf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gffqdojpq.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gymkweshy.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmsfxnimm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gnfhsqvsx.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gdisjosqv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gljcixarv.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gwfjmehrz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gwclsulux.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gaekamcfb.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/guqxdnufg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gfoplzhff.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gorojcfmp.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gyazpmcby.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gfziyewcu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gstylpinr.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gzjcljmxa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gauziaeoc.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/guvdcobcf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gofljaptx.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gpmzgcrlu.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/glmasmauq.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gkuhgvdie.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gzaikgfhc.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gdhkrttck.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/grlarvxtb.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gfknywqlh.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/guqqxwdfm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gyoomtmyl.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gkluasdct.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gvmsitvrm.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/ghualyhsr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gealncxcy.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gahlfxwmg.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gblmujmhy.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gqrqxxobf.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gyxwcdppe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gzngnvltp.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/geaxfbzyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/glcefysry.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gxzcxlmiy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gwszcupjy.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/geagrhlwr.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gfwqdkzxm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gzqeofalr.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gvoryhthm.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/glnwbedyn.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/ggymyzjvd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gmnbsodcf.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/ggxbttbfj.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gbyyrngym.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gxznqkdzw.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmjypbiih.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtiosgmin.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gzpdhkedh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gwfdvcwwp.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gdxgyfplm.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gxvofpszn.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gfxsuoxci.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/ggcgeafva.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gdlqmdpml.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gnnbrpywy.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gewzuqgzi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/ghtglglig.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gcbouwxsi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/guudhbiyd.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gmlufzyib.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gvdhbdltf.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gmxwlwbpl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmpdgguy.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqponhw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/grqrrbckp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gasjquzgw.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/guapqjdip.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gonyppnrn.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gxluruhth.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gwphrrcfb.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/ghptgosoz.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkpqjcynl.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gilyjcyhy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gizydodgj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gzqtnamlg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gqzavsryd.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gocnbgygz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gtjeqyusf.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gfhiopkng.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gknzduqhq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gasmcxyay.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gqttfpoom.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/grzqjnhwx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gflcjslqx.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gtwczvkby.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gbgtysugy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gndnfbnnm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gtytayxwd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkixvruph.sHtML


<!-- 参考信息 -->