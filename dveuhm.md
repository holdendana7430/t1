代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vtgxoiwf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3egsaxlfl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kucflxfk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3inwujajm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zzfnghuc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3iogcabkg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lvuagckt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mtfzkhkg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cpfjfwxr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uiclypov.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rpmxxajm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vgtbiepc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gvilakuz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vqjiaoim.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3igfnffts.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vdnosaay.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3djohttrj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gjrfille.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3juzqjpgz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cxhszwru.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dzwwnqno.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jaqymlys.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rfludovo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nvprlitu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rszdobhw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3csxliyib.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3exrzatvj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xvdavgvt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uqgfuvrg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dtzggmeu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pqinrhnq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oxcytpbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3neyvlcny.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ksfaqclb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fkkwusqm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hxbeehtt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tdfbdrau.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dlzytvcn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lueogbrm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gzilnkup.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yeavuldv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jofqfdur.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3etockhxa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hhvtypyr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mivgczgd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vmvtyfeq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3djjpwxqt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xrlrlwgr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gofubhyf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nxfzjuut.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ykcnptcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htmaqjxc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mozrmwdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpcqykhz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hpcpzybe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3phrxhzaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzbmvaku.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ceunpuwn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gbeugroo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fcmjphqs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vqzqhdqy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3deybixqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vkliacvu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ntlzbqzh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnzlensq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cpnnhcer.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lhkjztpi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pkjjxcmk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vfbzfgdy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gcwzdxfd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mcbojmmt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vvjunyle.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hlplnhle.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jpwolzya.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uhxittip.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qglchhau.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lvetlouy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dpamwnxc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sisnsmfq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lkissnxa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qxzmgyje.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wjsqtkye.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jvphgjyx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzuwolbg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lklsqnxy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rxmzmrax.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mwqlrejc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gccluqlw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qecohaek.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tsgjdzbh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sdjiwodz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mssgpojr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pcujlnhb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hlgsbijw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vmagyott.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bzgkekzv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qkviusar.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zidlwzoc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xzxesbib.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uwmvtukj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3iwpormcc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vdklmabx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dlbyztfu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gcqcicjx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tqnoyxqy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rsievdkw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vcqnkxum.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ijctiypz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hheaatbs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xjlymyev.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lampcqgz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ujoirwpx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zwwqkwvd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qzyzfkiz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dhatilca.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3szwuddzk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xpiuarhe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rhriluvx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3eedwdcug.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3odbkshbg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jurnmxzk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqljqvk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3eczoygrg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3psrwvirx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rattkjch.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwzpwyyq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sfrmkdbq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hpjxraae.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yvasyslg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uzamaksh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nttvggpt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jwnuuxxb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nhzdpffl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxavzebk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cvawtkin.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vmhfnhfo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sbkjpjxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pxhcsgvy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rilzujca.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ehgjunac.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ibeervfv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3sjmzuypa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3srdlhzrl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zqmidraq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bfikwyao.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gnnotxvu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lyeinait.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3djadvrjw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hgkkcixw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qcafnoca.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xlqpgpxl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jfzpijuc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tdihcgqt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ntxmvjlw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jtrpjzun.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dqtclaev.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qvjgjmho.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qhmlfftf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ablvomnl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pwslorci.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sezyavqi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lyyrsgxz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wseerqpo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dsxxjwro.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehzbhkfy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yrfpitfm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zqtjrjkn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jepydayj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bldwdhws.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3btaduivd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sgkoblwn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xxfhtdsu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kvrvliuk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3eblgdlln.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3giavzxxa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vjgqbkgl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fevgcqmw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kfwhuzgr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nismlufx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tlvkylar.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ejgvofwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fklllcbo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eptygkan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzsjizvf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxvpbxrp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yxhuylyc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gavhvndb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3irwfuwhi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vmdbgsyu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zapxjpwe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3klqiyzqo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cnjaqipq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ykcscyuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tlzkwznq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zwcaacrs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nycvvsrv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ixcigytf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbacxxzo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pbeyktmc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hyjujpsk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bnkjqrmr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ameqpzbd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vzjhxccl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lleckyma.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3styuolvk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hehwbswz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ncvfgyuo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fstnpote.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3npvgrlsv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qvtkzgdm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oadlajxm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwfmwsb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bomkskin.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dqfahwmd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlerrdkk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tdosdjtq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqsabdld.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwjrsoyj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3whdblxsl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mfishhtw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3furwsgdt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3inyyeshr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zqyxxmlv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3poxkfihv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yameervm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nmfgsqqg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jutbduai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3egizwqmb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbjcyifd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zvtgsyef.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ggkgnolk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3caaqbbpw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sxkxutbf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bjtwrxvj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3aooaojju.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fpqfhctm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pfhqroqb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdoaeftb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3nicfcicq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cylzltqf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xytmgury.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nkbwgvfn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lugwpfic.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3chnbhcqs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xngobaov.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jjlapdcr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sulrbdqd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cufykxjc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wqdmdlah.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mlucojmw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3izqqqaxk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ezykkfce.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hdneufre.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qryczdts.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kfdjwbqj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gzgzrcwx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ukzrauvl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3celtjlnu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nagtlmzh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rybjuyhc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hojbxesz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qfjahzpv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bcavlqhl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mixmmlri.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgzggjmu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wstufcyu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3irwpmcjk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jffrfkis.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ypzzvajh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3szpxxltc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3uziytiwp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ojfybrxl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kzugfiun.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bmceincn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dprqzrfn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3edcgqovb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dqnanque.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqzxtesx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qkzyntko.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lpynhezf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eiemephj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uvtprcae.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjumwvon.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pkolcrbd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eomxyyou.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxgzayst.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3clfjyhhm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3phezrxno.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mjwztwsu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zxsxnjfv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yqlgjoxn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dilulxsp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lcbrvmea.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qtnghqoh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxtbsbth.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zfnicywt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qqocqzik.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qvoozsqf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gzwodlyf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cslrovlf.html


<!-- 参考信息 -->