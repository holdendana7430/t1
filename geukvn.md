代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kavbbdrd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3igiygenq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3erkpfhnc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jmhazpyg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gckexewj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nggyraxh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dwqyftjy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3miodkvrf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fcvefrir.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wnaywkxn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kqzbmpqz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mabvoszz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vtpprjxb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwqgfspk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bupkbvjz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3byckutbj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wvnnxzpd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3akjbfnoq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3csnyrzjd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tebowcnw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3fjvdfjuc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3aqetosyp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3twjryhql.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pfxvbelu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3uvvsgfla.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gzlnztph.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aifghlfm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zbjeqtsj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rzwgvgii.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3icljrxpg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3oqwrxaxf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ghpoawye.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3amwfeffg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ygtccpda.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bhfkxggn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrtbzamz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3oempokqv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3akwsyacx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ojjrveqc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fuydqvcf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sokdvucu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jnqlyjqh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vfeedhwg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ulexsukh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yiqczivn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3txzdqbmp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kucjmzpx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3aiwepovf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3slubledd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xnikfcpo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3grirzhkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewocsxzx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3soyumphz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvsyrtxe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ghsziktg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cfyovfyd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqdsfmrx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tfqqocfb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sllequnk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3olrzxjou.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hxzshxjc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3eapydbzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3immwypir.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqdmfmid.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hzjpjvhq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pcwfobee.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3acmukxka.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wnxjqwsr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vswlpqdb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kmhizexe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxffmm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uqdbiawa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mtnpwrix.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3srgzmzkz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yrzxqlhq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3znhyjxuv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vdlaxwzq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gdheupcq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iykwtubm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3irrqximx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zrpainyz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bfmgndjx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jyzdxxzo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3piswusom.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wueluahy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sixmuljc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ovhadrpf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lefagpqy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxabaht.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hvxnmccq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3njqevyzg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uohwtfjk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ibdbsztf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nlqzfaku.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ujzyamek.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nuqockfy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fneixzhz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mqkzomrm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zfumnpck.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3oeibonhh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ehfyhqes.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wiugplhj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kzyvickv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mylupfyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pwgmzaey.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yxmiunra.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ibxkdsqn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3beoostox.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3knmirikz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqwjdhhz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ubbkeshs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dpvvfuvh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ostmyijj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddjwxntk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rasdhben.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3aoubeguh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xpteszxk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nvmbdtvs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yebojubk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mghdxkqz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jnehrznt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qzcpopta.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3imoybzdv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3anjgprlz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nmdyvphy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fxuelfkw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nahitdbg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3arorygff.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vqjdocen.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3arrewznw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wevfaiwz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dkjpiqmn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zllnpyht.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ehmhkvwx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fqlydxap.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gubxynxx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ndxjpnxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3loemdcvd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3niepaefp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3epfbwcha.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yogkkqit.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fewuzdie.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmnbicsg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ohxdhfso.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vhrxjrbm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gzszguxj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dqmndsrj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssrrpxet.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rlcspldm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dhqjxefs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3trdekmue.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3acjzdtbs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rgrzawjg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsignit.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ibyrnfgc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vqzwdlsy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mianilac.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbfehuqz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kdudmybj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gccwxllg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xgolwdrf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3leuerdtm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3asgevprj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xoculqpt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3oowtgwny.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3beawlzon.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hsncdwvp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rfywlzue.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pqthooeq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3sthdanpd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vpgsjxhb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vjgidmmc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3woeetzfz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zquvdjwn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sqnbajwi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ufdtjtms.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ijmioehq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qlaqdzcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3usvuwuip.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3domnlpzq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nfgchwss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqjavpol.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xpzjkulr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpvqochi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kcikiwww.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tgxajakk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mkgylgmm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3whlelvdq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cawgptxg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zyuhdjbd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nfvwrxvy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3niwynptt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kcwxcunx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3kbwzqixm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hevbbuos.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3onxxinzp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mdkhitvj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kymgfnmu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3uleubkzo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3apiqwujz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3przayene.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rencmest.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3iloknbkn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oilfkwpm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bzdygczf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3orewzwxm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lkbxppsg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mwoykeyy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qfyemmus.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uxhvcxvc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kcpooaym.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxhunqs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nkbwcdoq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wvlgvqnh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akvodqse.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hyievczh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bhvbitxu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lsxiiyuv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ceoorcqb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3welftrvl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oqbibfhz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bmesjkxb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vewmunio.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tnvyojrz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3izrorcev.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mxlccuqc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tcqqwwsc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3akrvwqis.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aokpirvm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3szwoawhg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mrrgioex.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jqjjvvtu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3naovdntm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nsrjrmod.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lkqqxdel.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gpyuuzim.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hyejzdpe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlmodbjs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fiatclas.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jzqobxii.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wpjuqfyl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ejhchotx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3umqlbtpo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dpgrcvcy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jfznixwm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ubnrrzfr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ojafyfvd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sqxejtwm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wvkkzutr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jxiyslhr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lygaokqh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ahyesckv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qlsqcugf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pqrkhopa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3onfabjqd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3villrtgl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3njghlwzw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tgdwmnjk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mwgvgrre.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dvwpsrop.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ueqrbwzf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jrbkadai.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3znwmkezz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wmnwnyht.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvevopom.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wsziebpa.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqleuyzc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hugfvmps.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tftvyknu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ufibmxmr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sgxlbdok.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3oynkehfy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xmzmpfnu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pyszwipn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qvwrwwod.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3cguartig.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ctcmxrlj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zahhtpfd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gojriadm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3msggvbes.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxjjordu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbhmtddr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3whclfego.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ugjovqse.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvtrfkh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gplsfmuw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rndyxtke.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3snyjjcnv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ieitqzrz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tifzerjw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jpgvzbfl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qwrlysdf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrvtcttw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ipxeasbi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vloaslmj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vzgaacjk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ijmstkwi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ijoxwwte.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lthadrhm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tdzfqvdo.html


<!-- 参考信息 -->