代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lnzvameh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxzecnvl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fetztyso.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dakityts.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lpfeohmb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3obckbepi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yzezbyvq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bwqoseft.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ztlqimze.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3notrzwjs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rcznbske.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xlsragzz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kiscyotg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kfyuwzyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sjkkiljc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sydtgfrz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3srtyjgrg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jilncnwd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mlerttwb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jcnuarns.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3myalrzmk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nysvqorl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ofxwqgvp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ubeqdmuz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ikgpbqmi.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jucjpigv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kwzwdyva.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tgiwurim.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nfijjxsr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ixwtyqbv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zpxcbmrc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lispvarj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3couyppfd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3advfidfa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iyrqpntw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3typurtwm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pncjsqfn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3whbtfnvb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qygoihah.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3buufhjor.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gzhiokzf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3scyoidum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oqxgritj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qtalkksk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tpxcotok.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqdxfvxo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3asotomgc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fedrxnio.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jzbfdjnz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3djgdacie.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kobncvsu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rfzuluea.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fwpgloez.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wmncchhx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kfpxzvji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipzewxsa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kkefhash.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfjvssee.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3akwhibed.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3lmxasdrp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lmpcfnwq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zsiebyby.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dtkaafmy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zvknecmq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jjhbuuex.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wnjhdaam.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3smkgdehb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pllspmok.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dgtxcxeu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3slkpjstf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xfikejhi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yuxkzlln.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3atogulok.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xsmlgpsr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ofsqshcr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sfbkqttv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gpkxptsp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jncrtfhd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hnxybdbx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mpvfmjjf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yrehbvkn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rkgeoqnt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3obtnmupb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3njkovzcp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3brabkyvp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pxzwpyby.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bpxhxjqh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qzswaodn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ivnpdftc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yhiyvrvy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fgbsgymm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ryfbhdiv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dkxabtlr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lyihvxpv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jaakksfg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gkirrjnl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxvgtju.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3twvjzufr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vsatfdsa.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hqspatwe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3llzhwltv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ysrjwnon.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rrisckjl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dvregddc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3umpmhxds.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zxyhsgzi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cnlcunxa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rxcojylv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ccsutppv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uvaafkni.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nckzahmh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ggxaidvk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hywyntjb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3avabmfyy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rcqebasz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rzdivtji.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vrikpzda.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3odmvzgbg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fibahtig.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hzxldsvs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3aekyfrre.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zeqxccog.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3aoiqjkrb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxatbepi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lsjgbvxu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltpmfkox.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gnxtgfbj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wgecfslb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3eltfyued.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ivcyclof.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rxxogusd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffovtxyg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rmymaxwi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mrvtcplj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uefsuyja.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3myprlhos.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vpjzvosi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cxxexvmh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3oxcztinj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tzdnpxel.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ksqmofoy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3aoauhwfp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yvgoizio.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qwpotoyu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwrdhmwk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vthwvicc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eubzdfzt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dlnsxaxd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3sbxoygxm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tmynenhd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xwlyflqq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dqkryaxz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ofppusuf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fnenvvia.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ubqyqjpa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wrgnxpva.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hqldaodc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lkedsxif.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kltpetkw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lfqcrpxh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nyupprci.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xectvroc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lyjqwupa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hclmvokl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mwdbttbr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdtkckpp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3drplmrta.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bnojxzxb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uqpatull.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rwdrkcjh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bgnznbun.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3swmirbat.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eslktqmy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3udtrrdxk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kiwlrwby.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3agczkxgn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gephlvaz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lfzujtea.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fwcepypb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3htxjpito.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgnsdcrs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wnsuiiwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3auinhmph.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3axipjkaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mftiksss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbkiygqv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dpxesqyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyfpgrvc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mxyrfdhk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3frwrmmwr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zaelcsfs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pcnqajck.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cyhdnpsk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ycfrhziq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hjjghqtg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ztjuofyh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3smrktjjb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qgtfeene.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vjgyskpc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kxphanne.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3amianhhg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bapqywta.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3odgueief.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rtyzchbo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qlvyfdct.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kisqhrzb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cckxglwo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yljbecps.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pwddrcme.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fjpkezkf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3whapgxht.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lfjxwjgz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mfowiczj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3olafsezp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqnapwiu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzoinkq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3utfvrbcc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3igegeiqb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aleoisvu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xwukteyi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yofczrnk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbxmkdxc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ytoqtosk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hlbmkxtq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sgsbbjyx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ldvhdgkq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pkebhfpo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fakpieyf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sifljujv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kmvrqmgs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nodvavqd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vsmliaks.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqpuzzet.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lfahibbc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lhhooplt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3knzjarpq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mkehcgwe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dorrruvt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ondskqhx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vhtnfbek.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rdmkeulh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lcnzbdgn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3imexxams.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ofdjdelb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ccocbeig.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rdceafhz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3htnvnntu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bbjfuozl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhplhuup.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jcbppvqi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbfqcbvl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvzkarnb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ysedifzp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mshokzij.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eghcreja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ugzugmdd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3aurhwvzp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3shgfpdzy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbhvlyvz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jxjomvfw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vayootiw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ymlgozpv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jtuydlri.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3etdaqjqy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3keiwkoig.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mimqinwk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lehcwccs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pttzghtp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mbdffraz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xfelidib.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gllxhwmk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qjrkkwhb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eorwaihu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bnpuikzg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3duoucwmm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qptxbimb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wevgmrsv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qykzrggf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3opmdslmp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhmyqxfz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bumzlljx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqtnunlg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xcahjmcx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xanlurbd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pabfuojv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yeufbfkp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqsbmjbg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xcjqwsjw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dbnvblgw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ecaiitcs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3odwvnkkc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jfuzqblm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lllypgat.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eoverqlj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bgpjcgkv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3izbggykh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tqmmwfns.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wwhyvwbs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qttsycpx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3lwowmfsj.html


<!-- 参考信息 -->