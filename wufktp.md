代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ztvegfch.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qzzuebzj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3boofebas.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xsussfzs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vxugfcds.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xjdvpwvl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ivgknjna.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tblnekpf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3aujnlufd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3amfbantz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vmpsmtjb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vpebznjn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cemrhthg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdyyzdju.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ffhrwoxd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mlgfhvbz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jxqqcbbm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vxqrtskd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3eosuggqs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bndvmddj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zfzdxqam.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dgkhdehu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qpneekds.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yhydvwhf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jmohkixk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qobpcwxi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kibzxduw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nicscjqs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bxtjsxdc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uuivuzgk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bvvisqcx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jybjmsxe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jzunyjhd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ywjdywri.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gcoubjsw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wotixcmq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rzosnmgs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qrcxifpc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3urdaopco.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qhtwnolt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lnugqqmu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqgvmgkb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ltwnuixv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pxrxeoso.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3mfwlcfee.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iwvfnmjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ekpmrkog.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dywasveg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lwqhiopx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3boqorgfc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ufyqlvpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrljwsaq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lvuozwul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyikromm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3afkwllzp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bfdssnnp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xzubqvrr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zfynvdcj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gcwumvwp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tkthvmwj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nmvyyjvn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gulqqygv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lcbjkfga.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tivkbfma.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqyrort.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ljjaoydv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cgoxozrn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ocnkgiqa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iekrxuja.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3emdepgql.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3weejqzoj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ieregzdx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nwiyjqxg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zkcwpkoj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eyjeldrk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsoytpym.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rnmrmayz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3glyxutmx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lscakxsn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pivhtdoh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mpyupgwe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zyrrqwpx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3stspapig.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tajqomom.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3knacgbxl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ubwfyyzx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jaorrbki.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3frgwfdux.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzmscbfy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oockivbu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3peijvxou.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ladiwlqj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qhixyolv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kackqciy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cmxqjgae.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3olbrzogk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eefdhmmp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dwrnuplf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rfcdtoba.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3recvowyt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hjadyqbk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wtvvknbc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3onfdkrku.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lvpscwqm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vetrljqq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cpdqglrb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3quojnboy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tcofodly.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qixglffw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lvwbwydd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wotnnkms.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3umfyjnzg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jlkynfbg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cqwkeczz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3agdicjsb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ucerbdwo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oacbjmnx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ijvkgzrd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3chwoivcr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mpqswipd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fdbbyojl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tsudyjkb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rubadhfc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fvlafedu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yimzesjl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eyrrttdp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nzhjcwkz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rvvukgvb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iwxvhopo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dicynxwb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3avoqrktx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pjfvdsus.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ffsecptb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3amksnvwk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nxsvtphw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gzdrjuiz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpkiafie.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lezuevbj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3caoelwkq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cydtjnjj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dsdbqdng.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bmjqqtbv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dpvypoof.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3debjlhfn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3haiifphz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zidolifl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zcssxuti.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jlneiwvf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ugwqdmze.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3umweltnq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xpjqoail.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gthebzqb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vtuknqsj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fipvmzyq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cclsykpl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uglwtseu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yaivkhrb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3psxuixde.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3amztwyty.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3woxeamvg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xurntefy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dzgrqfhb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3etnpnrgz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dhcibhmk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xymjsity.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uolfbhnr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jitfinpt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3drsszymr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wobtcdzb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nhwzgtof.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kqblbtki.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jhcfcbtj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvijoboq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3esbjnnqr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cthnkceb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qewecrpk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qnokincp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhdndx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3luqrqpkv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mliierui.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vyjvnvmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kchjmeju.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lltyqjeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuahbiaa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kdrcsbca.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zwfrwndq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jhktoijf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xaxuxmfn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qxvdpyqj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fwinjnoi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ydrntmiq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gszoesrl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sebcypsq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uukbclhd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nsfjwipp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqstklf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lqmpecmh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tdbivcyg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pvntqgzo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qdxvlglp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xjykqcev.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rsxroaxj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvosqdvm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xrzwichj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ozogqunn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dgzbfadk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bppycusn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbovcedz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xyltrquf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqckyiry.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3omdbcxra.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cohvddrg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wvegzirp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ijrytvjy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ndoiondg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fagnpfgg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dkfywcai.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyxsgxqc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3azybvtca.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pnmmwlzk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fewvakja.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tguzhggt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3anforhra.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrmnus.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3txwwbgav.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zubbvroi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ycicgryu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3epqwcpjb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3brotjoyg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zevrwtzy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3shmxbjbr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iydjcmxv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yobajnvj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yfndpypz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wjfsilnx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nkttewvv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ildfqnnc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rgtxgbwb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yvjtkftu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3isgeguhc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qlcuzaxa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvfsjoi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zrwlilfr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ukqvfebw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eoehryst.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3relhigyp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3adlbuprr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfbrktaw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lmbythmb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mjhimwud.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3svytxqkv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tvbkmiup.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mxdzrfbc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3awvcnblm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzbrgxqa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3thcnsehv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ujereymp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yjlunmhh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ytgahebq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ylmegisd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bpgfzwzx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qrogigrn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gtdxrdrr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jfgwvcpj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3puunhvhw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vmjlvihm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3lzljjdib.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3imlafbqb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ojeaggxh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ahczltrq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kdstbpqh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iclamblu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ezftzrar.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkhjmvy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3hltksrva.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqkpumlf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vhezmbhj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3taymnyqq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gaqbxykv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jfbroibm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofowctbr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tucfvtja.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gdwbkpig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jpqhnoof.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gsqfrpep.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fsbxndkt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3edcxbvvs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sedvtinl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hxjhcxzb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ottjrkxh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ajawenst.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3psmsluaf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svgaobyh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aojncvuh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vwgexxmr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dbjgjbtx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3njfvaojk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xrlstodl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hfavvtfm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ipkbmiis.html


<!-- 参考信息 -->