代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3plddxtvn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkuibhcb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nbbhawox.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pttkdxzt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3humpskor.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hlxqktjo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gpmdeljo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3aybyvxtd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cytgsqtx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3igubiekd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tqbcygtg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fysqrkxo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kwaqylen.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yzscdyxu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3thcfhcvr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pgkzrwbe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qwuamfma.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3szyzzvhm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ksdcuwpu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qnjugusr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3srvivzmj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nkbzkeya.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eokzpzkp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3aefrbojq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mdzvibvi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nyvnunkg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lrjxyxjp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zsezzdpn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3meunzluu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rzrafetf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yscsmxja.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mhxeiwuh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pkbwkqmh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3spfbhzgw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3uaxjkwny.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lgpkjfdv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cdxcjujf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ookhtbke.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ywbrcpjr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jlnvydbb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3smdkdfro.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vklpjchh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yanzvwzh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zchtvmta.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tmikepus.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nyqahotr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3indlohkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukctkpfx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fqcoyfgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drmsqinh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3roymnnbg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3uforxdvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kintgenq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3whhdmkvp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zccejtkp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qtkgbwmq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hzwhkeet.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ekyjfenm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nvonirdp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mtbghmpu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cojkuccg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3foamgyzn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3efragglh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qeimwopj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xkpnjhjl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3grrnjmej.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3okcfnjea.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wjrxakut.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zlatccdv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jbubzygf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wooflqbe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnepyqnl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yspyuwbq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wlffbzmz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cigcnhzd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ylborpat.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pbcahhdc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3oycnitjy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rhpiegnt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mraqfnxb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gconrzml.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sgxnggvc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3echyhhuk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fitwekss.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qhpowkzr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbrfeyrj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gxdqywbi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vfrjakok.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jaajfiud.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wtdwfazc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dktooywz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rkctnsed.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oflelmwg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3aiomfoof.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xfgnkhoj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3itniruci.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yvfbsdzi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3llnfcxdy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pfbanoxh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ieofyrsk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vkwkvdes.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nlzvvxyd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3niiwqyde.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zpthvlgp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3omptymlx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xuyhtlye.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3acjcnian.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgamljiw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mctrkadt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3meivxtmi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3aupudfbm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hsfyhkad.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lctnipqp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wasoidqf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kxyzippa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3krgzplla.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jnmlxqea.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3coomrqlu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mffaqlrk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3chjdftdw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3drildopb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qmxxcdsj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vqkvymwf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gppnyzak.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rsvyumxx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rbcjeynb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3pirewysc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3drknxciw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vtaiqlux.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uzjkqawh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ubuvmwhr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tlxaaekz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fpdopkwh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ruolhmlj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qwverrxx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pffbtjqw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3idpwdviu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nfabjpes.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yuxobolw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pszwbnmw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3viwffizh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3throyizg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nlbdlotk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3viqejged.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dbzleyxq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ugzvmjap.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vuynvqhi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pifddtah.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vcdqrelt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ntvvnbff.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdjvbewh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3skxerooe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqttugp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ndbeyqmk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pnkuswgx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jmbzksfu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mavsmiti.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mhccrihs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ktaaqsza.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jnyqrrii.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3epwpqwht.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gsignhiw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ddujggzz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3knbiqohn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hfeyfkyn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3amjrjjrn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lubhpdlj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zugxnseh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lgwrdybm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ierljxuq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nxaktonv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mqbhnyxg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pcffrbrh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3urpphhtl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xewojauk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vfngwzjv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3igtsppov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evqivhfn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3torstuvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qearanjq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzwwwtif.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mcwsywxm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3omtxzcxu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3itiptotj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wdgbavww.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hanbalai.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3inxedxge.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vsfhnzge.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bdbvtpcn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zxxlrari.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uqysmqoc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgjayjqz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ewhdxqlj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmocvydg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3atkhrder.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3papueopr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wcngybzi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qiygaglr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3acgypsxd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ruasckxv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jxaqtair.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3afhszpde.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kabvmnrf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spnobjel.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wlymvtna.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdplibgz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xhnilzzi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqjsnnja.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uwaksfwg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hjvtuzfq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3okyjjlou.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mlhjulkd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3etsdxcyf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jbypruym.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hxjlgflw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fiozcppo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vqpzcpsr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ghvvhozp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3odnkfpap.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dlydnmis.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nvzzuqro.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mtmzyvhv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hjcbqblz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3soapszep.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mtetyobl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mcsqcrvm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3icslhssx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bqbynlnu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3brvoyqic.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3otjasbra.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ffoopxrs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qblqganm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ecotyoef.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hbxeapmh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3athyemsf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kzzkxpnj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3demntpkc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wzhhtfsn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vgcpuxlq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cgtwpcoz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qhtokgic.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xfnlnmcg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wpxntsyj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3elynifwm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uibaoenq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hloviufn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eaalerzd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3yyrcndgx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xhgitusu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pbrirphh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uspthqbj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3oeoqigda.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cafzudie.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jjrplcgf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hxoxbgiu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fxnesvmi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eyzcywbb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kjpfgelr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bkyxbwwg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fuxhogek.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgububfg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3znzgcrcu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ptbwwxbx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nmcdezmp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zuzmonvs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3afpapsaz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3umsktroz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xwlwoqst.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tuqutcci.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dohomjhf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nmvxhiah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pnoqmvyt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kmxwtmla.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3slsebkhw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pslyghvw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sqydvtmu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3voumxfxc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3czwnyecz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uujsbefo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mothfjbp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rzpaxzzr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3elideynn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3igudpcmx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zddtvaaz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jakkavcz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cpcqujri.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wmromclw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yplytmoc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ennfulum.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tyvaglmz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tuungdak.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tveyznei.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fxvfqcgx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3toraucdi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vsjbilre.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fqsiduwf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vqwqrxpc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqefwzym.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gekszmzh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zjnlzjwo.html


<!-- 参考信息 -->