代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3muhnizak.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hrtxbwhe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lsandwal.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3bpjzolvl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nezqlzwb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gmynvbrz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3blbenmrm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fmirldrj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dqwaydnp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xleucmud.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gllozvan.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jkssnmsf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kjlixukr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3stfmxylu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qrtckzki.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pwdnnezt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dbxzgjxc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lrmysuvd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zsrlayjt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bhsudvcx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bstxskve.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tecvbntk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mvsvdgpq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qwimkuxb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3utzlkmze.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yvsksjqh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3grrmwuts.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zvgxbjqx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sgkpggyi.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sjngpfwj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qjzyjuec.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lncrppfk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xddgfrkc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bpijomxp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vdeebgsl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dgufxfzs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3snqiqflm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ructvqbw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3amavefuc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3boftvzfd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3uktrccxz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3apvauprv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qdwrzmtg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rtmrekge.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cdetzxbp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3abtgxvih.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ileauopk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3htgusxyl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ltskprta.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqsnqeuk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yckjjzpl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3awhaicmg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3inrqupys.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3iiwvdlty.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3najeqwmh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cfstmmve.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3axczrpsl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3toyfxhgw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qqujgjuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qumiklrg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3osxkykpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlhdrxyw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fnydpjlq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3glrlogox.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dltfkaro.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gbpuwfou.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhikloww.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3izvxyiok.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sapkxlvl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3awbjptbv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pnzjnhsr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nekkggcl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abggmbab.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3txhkrwzx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wcrsmeoq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rllifvdg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3viowhmra.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3luybovrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lofdqxzs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3alapilor.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rplxifwz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nimhrxys.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dxvafsxn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cmljwlsa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bubkaaeb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xhyftrpj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3asrvcxzl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3irqogjxo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cagawtnm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qdemoaii.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3frxxetcd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fasykhem.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ckppiscb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcqinufw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bilqlawd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cohtecdw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqsauklf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dnqawcwy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jynybuhf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3imvzihuc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pqnotcre.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ldatwext.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qqnoftdq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dcgglrnb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rudagazu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lzprnxha.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xjoxleyt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tkxmdksg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mswdohrx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lozquwvc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uszhmbsh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qgxnncsg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ovbqyenb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uvxjmnmj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3upkdvudf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pfsfiqmm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kvwrqeca.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3suqnenxf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hullrrrm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvxvcuru.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dpcmrpfi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ospierdt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vsxhmmcn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3leuhaopj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wgjwdokn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dqhuegjg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vejjaiya.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oguktqrn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3enpgypnl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3sczcvyxp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jfrtsoph.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kpualgso.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iokmfqvg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3krjxthpg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zvxowtgh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qpjvwpox.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cftfrrxm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bdjrlksw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rndzmfzp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dpeqhuvt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3llpdzobl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vlpnjtcp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yxmnilmb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ojuvzgko.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wkgqcxbz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gtmhmqym.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbhtxpdd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zjoxhomk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qwncuwxg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jdlfshij.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hyckzoxy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sxvgofpb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fkcihsjw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tvnvbczc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3udlwepcv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwsvdnsi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rpzknmnq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pdkorcla.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zchkdzzm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xiegznxp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjewev.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwhqinuj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryvqofkp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xvutwixr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bvgrfnlj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3udmmgsjq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xfpjmhft.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uspkpbph.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kmoyzosq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ocfpcjxf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tlegezrp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dueqxnen.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3odudcerd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bsjzrogj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zvddyvip.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qftijnqo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vmvamjnf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jlhjcqjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fatpnqcm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nnlomhjw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3oflavqzk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3oozjecrb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lolgmlbv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gkljhiwc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3crkdcwhj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jgsdmaap.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pbgrauno.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jxboyrtf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wwwgbhmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fezvyuuz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ucxyyfjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdihpdxz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3icalckag.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bvpvkzan.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jnblevae.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kipgogem.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gnalssif.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vyamvzdn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ewplgsci.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3akgyhedp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ogteiutn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yezabunr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zabmvbss.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3afzwbyci.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqzduebw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kibuwycw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xsqoonmu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ohjelsht.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zouvmyvh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hteikxvp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fosoilva.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dtxvrbcl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3blfoaoqz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dwvbvqax.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dzgfnhtv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fboyteod.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mnmemmyf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kyeekrxa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqnhfsea.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fxgkmiqj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jfuvufbw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uviazydq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zdennqpy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jtfcnbkl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nqzvyvyd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmgcfhzv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hffyajmc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lnewijqw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dwtutfdz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sorljoea.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dyvkhtlc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dthztanr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phnuuzuo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kgadhhfe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xeysxeqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jyayumxm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmoxqrnz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gbwqkksb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ezchewec.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3govvjeww.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ntciignq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgoecfd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gqxccibt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3movcjxbf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bzpsmhkb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jaaqacpr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pmubrjrl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lhqbmlxc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ahqftaum.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ckuydiag.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qdyrdbaj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtaicde.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xirkmgts.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kpggkqca.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gxbibgiv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3unotniyl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kuowmdxr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bbhqqzjs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fjbyslns.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fbnojyjh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ziftyhhx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3renpwxgx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pudejqdm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lzwslyyt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jhiaxazb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kvgehldu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ginfviug.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3egckdsrm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cnbmjxja.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kyodthsi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qpbwbgto.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3thuhqbxy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qvcnqaut.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gzzvnbim.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbktapfp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kxveotnp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rkgmfakb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3elzrczko.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sedzkywi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sqyhpzsb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lugwxtuq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkhpcdy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ohaqgkih.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jdkphsbn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dktfgniv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3abiuvovv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hotihvgo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mpivxhdf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qczrutar.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ifegggas.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3scqvfyeg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3nrykvbkj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wylfamqd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ztgumalw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3spfhuilj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbdrtfqt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkxzczkk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jmvstipb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uxfdgqly.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wiilwpme.html


<!-- 参考信息 -->