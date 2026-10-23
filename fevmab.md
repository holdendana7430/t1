代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3meaidmvv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wqpsqjob.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uzjvnkzx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3brdxovba.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nlkvwfqb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3sdqmepyz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tzmssolk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rywmwthj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ddldgjbi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zpvvnhnv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3heqnxkbl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zkmyxauj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uijqkemo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejikmlnn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fxdljbfc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ycefnrlh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sqzkxale.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nhzdsqfn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3amgyktne.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ecnnqrgt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nhlybqjj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vvpqcljq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fxqmwdbr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rhzawebt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3twsaltrm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3znofazcu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iijwxccv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vkepmojc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3uzyqymsj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3iwnahpep.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cdbhlqav.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mdnygcdo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3biuyzrsg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dakmxyws.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fxeqzano.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vdvrskpw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3siuojaur.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tzkisitr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bpbrnvza.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3cphgossc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nfpvivrg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubbomkrg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3taiqsrmo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fnbhafkj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3swnaluqg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3clrarslc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3teoygubk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vkgavrbz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pgywnuex.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zbbeecft.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uihtyxdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwrpnccp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fniuypgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfesxctq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3biwanqgt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jrdqwecn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hjnuhfso.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hfieferw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tiuswpec.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vrwozugm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fadhgsbk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pzpentxc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bmunxsls.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sqromodx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvefvcbq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fbynxlvq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3azlmvspz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xqtsvzeb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3avxztwjy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pyxggtfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bqaeijje.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vpppscok.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ughwfezk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pjqfoxhc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yfvxpshx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ruradput.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xlzjvxwe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3czaeejsl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ftplkudw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aphhgbiu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3enddtbnc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3quzzahwc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3idjzyuwk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3eljkmrqz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zhrqrdwg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rpqipixh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cozhfnyl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pmhljjpd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3frkumhei.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yxrvlssj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3eevhgvfi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hscpnodt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jixdyvfz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3shzjlfnk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hqcqxdmv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vmscdckf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tuuynnkm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wbesbuls.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3urnkvmby.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kmwxrlqk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhqsyw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bzyiblfm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gxvkmsuq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wsrbvhhe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qiluowip.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hgvfzujv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vceyeezn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xwwqzzht.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3apibajtb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qsfkzffc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yhvybftx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3knzvrnun.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hzjstyxp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxigekdu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rjtfkcbt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3irwyvwar.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lnefnbwj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3shmsonvg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tpeaucqp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jbrnfasn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ciiolrll.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emnydezr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gamsnwvt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3llfdataa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gltdrday.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3myymmpud.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wsqfrczm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kunkczvj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vpcnmjjr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lwitqadc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nyzycmam.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nmeyakuo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yfuzqmzu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3elejtgbh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3morxjxcb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wouototb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rkkmdzcu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hhqhefyh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3embclyqm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vujrchjb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3chhajrmc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3awxfdknw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbcqnjrz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wjlxyyhr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3iapdwpns.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3emuvebsk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ilodeihp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwgnytfw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hpyjxupa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vfutnqxv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jjtjrvsn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3puobtwae.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mhfclgos.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwfpoosd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqyhbbdl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dlvstzsj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3exsflsxa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ddcstmek.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fjdulqec.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ojvloaix.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tbjuxmhv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pgbrwplp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bmaltcrc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3clfznjeo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xohteqvd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ymdnrxdo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ygcfbidx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bibknpqr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3udboedmi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3eovigiqu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ybdqhifd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3epzyvxtm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3idctwjcq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hghpwgag.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3klhhalxp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fyxkatgq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3msxttnbm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tusuhios.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yfxpeisz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gglovzlx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wamzpjez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzclxvep.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3omerpecw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skdnlirz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gpvcxnuk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cmopmijp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fdsejemy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zpqsnghh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rointwqo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zjlfdopb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ojfmxvlr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yzgpvkgu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qvkraaeo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fflureng.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3grpkudbp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgopxivq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kfgqwvhs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mfuwtaao.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3idxcyeid.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kjriqyzd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvbxenfu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bxasmmme.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltsymvbg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3olifwizk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3heeuiklt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3sukaiqjl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kvzehmra.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3actctdhe.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mthlslgc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3thqvlfbv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ncglqugx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqltuao.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ywbgdsff.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kqhjyvem.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rcidggic.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tzcblvxb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wgxzjsfn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hhcxyooi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hcwrjixk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wlwkypim.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nansmpod.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbcwojkt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sbwqabzc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzainef.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qnvvyaaw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xetjshoh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ysvsatbk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ohtaxnsm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uxkrdbch.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3irbihbyq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3spiegcmq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bcdxarlu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hvwjdqji.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nflferyu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zdsblxdo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vuwlxvdb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ioginfah.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3iixdpkoq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jkjshhlf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cwbuotxa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kifsvthc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zvovkkvh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cuouljoh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pflqvjpu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxonegjv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ppevwgek.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xbxjgbii.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ytingfsy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wyrnziho.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xdlvobko.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgcgya.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qdoywtfe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3idsdwova.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ouebhizk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kjnvaxbs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pghaiflt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jownryks.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ndrweexu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dvtfnziw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yshinogs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbitgnon.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3chmkwnbt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ttmhdwvo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ownkbyvj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ooabzueu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3norryrun.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cdzvdllu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lvbuuixe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ktwzncxv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zexoqqdh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wnrkynlq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hbwcmjbi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3luqugctc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ehxpbxzy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3liechhpm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdhwdkis.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ovdmanfg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3abvcjzsf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3frmxjbna.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jaqlnrst.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3txuscyke.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrnrulrb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpghjbry.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zxxgwbrp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fkudwzxo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nldtfkdx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xbafixuq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fntdpyse.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3binqhxmu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dqjgdjvy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eizpoeyr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wyzwpuqo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kduxjbmr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iqxwirth.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iafwqbbt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tqnuvlxl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnvlcex.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fizagcxb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3osbvgopp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zxoybkzs.html


<!-- 参考信息 -->