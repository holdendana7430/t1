代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gltanaomf.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gymwzoerd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyehrehdj.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/goggtggce.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gncxmfazc.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grapdcphe.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gekxvcyqp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/geupqwkjr.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuyrcgrs.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gihphdpvo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmvwvdsyp.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcgxkfpe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwlslautw.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gvwynsniw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcrdgybp.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggehpxoie.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/govjzzxhm.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gldatplso.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guydjidvq.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grewalnfc.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gioqmwhsi.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gekmtpfjt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grallgasu.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuaxobgh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ghukdivtp.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyiqlvko.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrmpcvzj.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gxaazufjv.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/geassovor.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqpobwlnb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gduqphlrj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcxmxefo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvrsktpf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gsvryeqsh.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/goaguajnf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoginztm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsubbqfg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrpxcuzv.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grmilpruj.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkuyqxyt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grorzobez.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gscpcgqkf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gzwpeqtmk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlvzhyrc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqvqjqul.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gaworcmyo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gbojwrvyf.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grxgfdjry.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyryvjuh.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gubwiuhaf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdjhxfgx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmrqnvcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gaidwgwpy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gsnkbybys.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwlgvbr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpwnobwy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gopggunzs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzlqxrcl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsoqlmah.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gucnywrow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdeyuvmq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxvahvtz.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glzcftakx.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggovchhru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gebyomftp.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/geezfcdnh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gnpdrlypp.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhcjpkrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbupnozft.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbunkfs.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixikbeig.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gatcsowio.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrkbndqd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghsuisfss.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzljbnluq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxouhjmzn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshqzonhp.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gopjvabjm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliudgsch.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/glenuubec.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gepzdjyfu.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgfrsqfn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczkgfsiw.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gruijyopq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcfbwfyo.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjeybff.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/grgmsbtxf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/glbdheyqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gntmktsvl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwhvmhdw.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gpptrqjzp.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gseclsmrz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqbxdknc.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjszmjgnh.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgetfifm.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grvcfnsde.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gogbjkxxa.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbdlfvhwc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwtdzdia.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gwtacygpy.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwumyggwo.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gzctugjes.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyzavqhg.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glxnzpbdw.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/ghezslejw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gitlafqcg.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqnxqpty.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gyhnultpx.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxdjqqkt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnzparry.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gerooqhvt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gazhbecqs.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxneaqwse.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhyjdeku.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/grxhiydkh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gokmhdqvu.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfnzjbox.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guywcbuqm.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrcrpjeg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gawdosvza.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gebfrlphy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gytkcvtjz.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsitlfiu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/giheiekww.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/grvmrvmqo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqulkfro.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtfktuqba.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvehwzars.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gymqoipzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/galiqkozl.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqvrihpyj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gagdkqtdb.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigqbtxos.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gyeyjosbn.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/govkvtkeh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhyrdgdl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcqeanim.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpjkggrj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqfdwkkb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgpwctu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnpivnyj.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuzusdxb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrcwonxx.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggburauvp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduzagefa.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvzwhdmo.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/goldrkuzt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gredmsany.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftkzrcmg.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqgunarl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxknczfe.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/ghqkxvibw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdeuhaqaq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gtusbljbb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybsdkukd.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gejulwxsu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpudqerq.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntexhkp.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjkoufqus.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gerexvjxn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpczasku.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gvluhhenr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/guvmeqhcz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiqehbye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/glvmqaggv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxrcivbql.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsvzkctu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvfnkvtat.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnxgncjvq.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gsplqurhx.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxowsyp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecqskpfh.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gzgtokpki.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrjhjldt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgkbpkjy.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gnrxwsmqy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gefhqcgtk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogwmysrl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyblvnmm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwqnxcdf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspetpdvf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxlhvcpx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gommnqxak.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gahotbzip.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjmdakxh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmofupbl.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glohvdwos.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gynmvnofu.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gnbvexbda.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrzvqseb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gttinqsqx.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gclzbadil.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gndiutcxt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkajfttsv.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaoxbudd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoefmoub.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gmpylekrp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gblfgzuty.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnplcwdpq.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvdnkmhl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuofzngp.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gccyncpxr.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnkntvkd.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gvqgyensh.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/geellkgav.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/goaophkvc.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gxgbpkkks.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwmzdwmh.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmsuuhrw.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gcllqimaz.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcrtbaiy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbmukdnvf.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdxebwmqm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrsxosex.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gqbmbrgqz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadfjgkj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtrefccb.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/grpueomdf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthfdljmf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gczqtdxds.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glwtayaev.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnwpjbtg.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gncfkbprp.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gizvkjkdo.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/guernlsub.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gilbyitqf.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gohvbgjvz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekbxemhr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozovkmjb.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqkserlr.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/giblsglla.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvlounxq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpklxwhvv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gholbiqyl.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdldqsdb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifowcbhe.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gpvhowolo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grpjxshuo.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbyvzunr.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhlvuknl.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/ghjzdtjvb.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gojmlkuil.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgwsgmdl.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gibfsaqnj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/guuwtdteu.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuozsyos.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gyycdtiir.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesjpifnu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyixdnos.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddjiwod.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnstfhcr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlrmoipg.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgqwyfho.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gpvxxflvp.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxztzhbxg.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjguuzzmh.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkyicvwe.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmkvhbceh.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gszhflkto.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwajnyyl.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gapbmlfnx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glscorkpi.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gobvxyoms.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gpzouaaut.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grlfxkrdt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gznroykhj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakhmize.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gcuuhadfq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsmrfvat.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfixvgwpl.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gmrywxoui.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggmmphmgw.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdqoycws.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwiuvwnv.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gxrbekhhk.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gjupdzkks.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdrpsmk.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmgsoyfal.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/grcpuiwtj.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gydmpxufv.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfmkvcq.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwcynrnxt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilqgdftk.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiwtrpba.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwzxhwjq.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/garzdmbto.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gabhbwbah.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqmmucwz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxnuegjp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcizjazuj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gydfsaudj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtktmsohd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gorlyheml.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjukqqqw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmmgzpyk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gggjpiupr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvjxtxua.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gffvicqnw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcxxwtnm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gqvkuhvrc.sHtML


<!-- 参考信息 -->