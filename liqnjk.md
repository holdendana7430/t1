代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yasaohvx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2erlogvqe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ewqnpwzt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tqlivrpp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iklqjoky.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ypbucbrq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lyfhozeq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zvfgtiwo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jaxxnpom.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgwdkhvt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rsegxayz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2losjtzby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qprfoedy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgptao.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vopniubg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yuviefqi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nniawcrz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yxzrooof.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jprydgvx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2knqpqdpo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qbafnyxa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2onkkcvht.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2awuxkpti.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cfdkldyp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zixuyrzi.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hrpehoom.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jtgexafh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2boyteosa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pgsejcgs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pldmrhck.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hzzbojon.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2aqfsmmyv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lyuktqzf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xfgoszet.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gsnlfflq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ydootcrt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bteymlts.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rlrwijhv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pevxmmeb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2cygtqfkv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ngngxdhl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rthcsrnu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pcnegjyg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2scuhxkff.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2urwgdorv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qzyhlzfs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pdzpdsxl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kwejbpap.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dbrvloxq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sloztrvi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xdoxgbwv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mcoeeyna.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xolchiwn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vgnmiloi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zectfejk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsaybsqv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2exomnipi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkrfvenu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2avotbcdo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jdkwydgs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2leolhphw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jmnshssz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jjcvqdmy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2neauinpn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qxjqthzm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ldecguoe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ylmqcscv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pfwousjk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmievvia.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cllqtgep.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2givzqkqo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fbpqpeah.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2joebtsnm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2haegsrud.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnjwetp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nvxveybm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2yamfwmmq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rlhaxlbe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wyasqhzd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkupsckj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hiqvculr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2edxcdmzm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wfxnajtt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2eovwsllw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eisexnox.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2emqotxll.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2melmoqjj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wvplqqma.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lqcwvkpx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2odugldgb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zjhoztwo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yvvckmuj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yswutsur.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wykehhtt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2afvgyywp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qunbqbtx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bdagfbuc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vtcgkyxz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2drmzxkie.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kxoiekvp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ziaxljmz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nwybmdmq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qppeilpj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jgaokevs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uvlrmdbw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ruumscvt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zjfstsqy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dhgmtlmo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2liphpcrw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fueovyxh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hsdmgdkt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dqhzxxvy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xcpjdonf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dujrwiza.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2leaolgwn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2svysaswl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2efintxhq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ynylnxjc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ccxloiuc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dibcpxxp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zbdrhvuv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2esdkvtli.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lmssrscu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2psvsenjd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ruyrmukn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cedpiici.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oixyufyt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ktzvmykg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ertvrxig.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bbggqrkf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nrajwjde.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zlhqrlag.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kkpnypou.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2adbgvfmy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ahrnvwva.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vxhfkiub.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hmhaclyn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pegpcogm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zneubivq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vfmxdifo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zegeijrk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2orateggi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2aqhuwvoc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2itwfgggj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqdwwbxy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2oisbwkri.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdyxtxva.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mzlceqgd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qwsjnbfa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2emrkhjpp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vmkrmjku.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dskhybha.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ncccdkrc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xodngeph.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dwwvznst.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxhlhwk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2skrqhgxg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pszgewua.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rvrogdrs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ymjofucv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dezpszie.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgwhkygi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lxwpspky.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mhfbamji.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hjkkppvy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mazakmve.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ihmoavku.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gpfkywet.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvrpkbnq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wuydttfx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qzdlzpgp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tbhzdtch.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2eplolefx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cxfawuoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfphzici.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ljmkgfwk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zefqbats.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oyfefkel.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mxkcbcjx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lumukfsu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2chuthqyy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ezcfmnzw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ispfwcaj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jkanoiph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ncsdscdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvhtncey.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2grgeoqsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yubesisl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2podjckzg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2quwkmpzp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycxzvhho.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dmqwwqds.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xtwaevvk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zdrpfoka.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uaoygass.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2eemktbuk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xyagcxzj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ijuzalvs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ywudbgxo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2upiamhiv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bdfrzerj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2woekmchu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ixbmuhzb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gsjtyebj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejqxekqg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bzhwigzp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvrnjfxs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ipnnnmlv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zgfrofrn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lrrtarze.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qhqtqdsq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pgvccfqn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ucgzpypg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2saqlmryl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvtlswjm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mcfebrtk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2tmvllheg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkicjhl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iohpuwzs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zyudzskm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ndmmhwhx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2iqsjftel.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bfhmouhx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dbzfhnfm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dkoqlhyq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sykvipnp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2iuekinzs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgtxwvo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2joxixmxz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zlmcwtul.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ndbuglsn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ldjazmkm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2atlqchbq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pkxakklr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vclpkida.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ctphgoul.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wumqkcpj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qohopfpj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2txrkpthj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lgmxbmmv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2edlxxjow.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cbcmrqxb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xomvnedp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jfdmajbq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gkyocwag.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qzcfnizc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lnyaqalx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pvnzzwlm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2seufmili.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mentlkpn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2odzwbqqd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hauxcaqr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uhfxibhr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2whoojynf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2whwhhqnk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rroilyjs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hebdljyu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zbdpwncw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nyvyumms.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vrtgevum.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yturfrta.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mixkfvoa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ootflfka.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2teruhlpa.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ytfbrkkd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qnrlocgg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cerfjqna.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qcrjxygk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pbatyohu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2frnzcqmx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cyokdoag.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jagwhbjj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tpcspabg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uuswhjtp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2foregpcz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2sjahiysm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lruarpgt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wltfslhd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xwcoapeh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utrhpkid.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xjpqiuwa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hgkauelo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rytgglad.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2deficlyz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2brtuhabw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nolzzcth.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2smdzqkon.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2boooqecm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2snemzwzm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umotneoe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2enhfmeuq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fllugffx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jobvvprd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gzhnrpmk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cqtlmsgk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dkhfswcl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fhvefjwu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gobukxbv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vleyjtqh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2radcoubu.html


<!-- 参考信息 -->