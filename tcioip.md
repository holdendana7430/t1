代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gegjdqlb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2stqevjfz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2irxyvnpd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hwxtkzan.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rgbrelbz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nardkigv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gfaafzhc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ovgiyhkw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pyoyxlpt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2eletizdm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2koaqcgoq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kdyfawlj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pxybbvqi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2brrepaqd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2aumutcqg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2voqwlvwo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zlwmhdal.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zqbnbcgo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2srwaotlm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2avurppgt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ghyebjsu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mqzbkbvm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hppchult.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cohoqgjp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oodjtuqb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2shbvejdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jmdsukby.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ererdtou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cpmakswm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ryberizs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kydlczat.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hgmgdbwb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xtthswgv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ebdikewx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2satmixgx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2obthubxp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ukjelhlm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dwroklpp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tppmqfsa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hmjpvcsf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nnkhvqcp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yufanslb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gchndkoh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ozufkxnu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yxmkkmst.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2acynpuyw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ymgbgjqn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2diiyrhua.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rgiwuaku.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2btcricvo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zayxyyaf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lroyxxqi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kutlbifb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ufjhxqdm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nyeaplgx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xkspvbwx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdunwazy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2easxqwdg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hfasbtbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmobjleg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2oqvusrhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ontspbqu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dzkeqyzf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2grtiyngm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdvsnjhw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ttdhfgsd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tzgdeslq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fnmfbdzh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dizuvjrm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lphluwtt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pqajhoeo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nelynmbd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2uyjnpkfv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vswdapjx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jpmmwqdx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bimxkdek.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hzspdnph.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vdkfxgrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uowhgxea.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qbthyqyk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2alyfmlrr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ssntegtn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xjwvhrkk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oeappuov.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lwornujm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bidyfqob.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qhwlauhm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jwflknax.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yagpqeib.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qkzpbirt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qbrkkmzt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rpzerctc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xhhylbhn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lyasenli.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kutsnyjy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tvcktcmw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dvqyycfy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qaysglmm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpbbljd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vumdwjsa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rtuytizi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nuctfytr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dmojsysc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2iraaghti.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kxmkhgwh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rxocwqxu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bjcknlpd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qrwhgxmf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ukzdkwsi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vgjoceix.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cgaudzcg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dhupaeei.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2iiassnlj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2reyeyljg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ttmnkspi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2htjlfovf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2euefjcck.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xukeaqpy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jrhnyfba.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2glhutfej.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gdqiffcs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2yfgpisqd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zisutwjw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vmrkpjrz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wkxrfwmn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qobmsndl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2diqreglm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qfmtujwd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kkmqroft.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jeucmbjp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2myasmzto.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2szrrodga.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hibhuenx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pstxcmxb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nhohwauy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyvesjtj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qodwjbqs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wggixgsm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2iasishwb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qisnrodx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2npzkzrwz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qugagjhz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qnuhkxhq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nsepnpjk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gkxubtwk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gnnmqkly.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufpteprl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2khzqpwpq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jiaibtpo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kfofrbpc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dporruqu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xakxpyfs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2imqcnxst.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cvicyaoz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jozvaltc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnubxek.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kkshinyy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2avaeaymq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dlvajais.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrprzlv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xjmypctr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2onnpyntl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhokqxjz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2feloqivo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wyhhuniy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wkulsoao.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iftvijay.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dhakcyxu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2koeptyso.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ijbnrymp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2uehmsrgj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rrriywnx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwptpokw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ydpuhjyo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2caaafchk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gtmuqvpc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pfnhfkvf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rjrzyyks.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2egelszpn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2timogcex.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pxkqipjq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2nllkobqz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qyemrxlc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iqokghyq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cmgiurxd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2genfwejv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bezikhsa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mufjecty.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tdigaixx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bovorrpd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cixshmcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnbttjrp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dgvhilot.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2strtqxpk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2owhlrrua.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gmfctltm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zvwrxffg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2plhudgsc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2yqlkofbs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ymqwiwkh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qlvjwyfa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2giiecnqe.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2schmbvrj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2juwhingu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kuecsizi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hlkpcjiz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2crjkttbl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2otavktki.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lijupbdr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2djjxiyer.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wktsjzyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jxcyvzka.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ciddndks.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lvytlnjs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cbjfqvpx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwwwyfb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2cyjhxeod.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqclkpfd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ngwhsrnt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rbpctpks.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2spqiduns.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mihncrpc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iskapusa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vdyebzne.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vpcjncmj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wfkojlqq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2srfecvyg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eirecagu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xarqojmz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qhwfeedv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2uebftzph.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qgaghivm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hohkeilo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2moovqomy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ctyknmdl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qglymnqf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zikzsiuq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ydqtajgl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ktizbvos.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vngpvprn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2prmbrjjo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfrlvgw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xoasmetb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xysypjms.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qigksizb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2usnmzpri.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vjhxqaux.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kzewkend.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2muuxxggl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wqyjmduy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ijzaxafc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yrhwthhf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xqkrgbth.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2plgoiejz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2akftjufq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pzshgmbp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mhsyiezo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vjhzxsfy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mxaviixl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bcjngtcc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xburemaw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fosjwqce.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhcdjqpw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lkkiiful.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vlugxbse.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zvvczejl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cwwdxcqt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lbbijukn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yfzpgdro.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ysgjohbc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jtejastf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dzjglvjg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xeauxoeu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2onmbsxkq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xsufyhgc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdqhyviv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gpgmeuts.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qcoeysag.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nebwjnma.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yvtqjhjd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yfslefyg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jguymexc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qympefjy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fnztvari.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2grwonnxs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ozxgesmf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rehrlvrv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mwhycykk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nfbiogif.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2giqaputj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gzegwkif.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bpiigbay.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulaeuafk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cculckdt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ksuvwqwq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lbryuikl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jeupzdgb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ghtdzcik.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rlwtpqqp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kcokflsw.html


<!-- 参考信息 -->