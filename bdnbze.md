代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2swvbwcdf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vtyowhdr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hqorickq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2esziflkl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uhzdtngo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wswmdlao.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yhbpfqjn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wfmuewuw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zavtgxfu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oltwtzoc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ktkvfwxn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wceeznmi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qvdjatoc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmxkqbkg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uhqzflyi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2aggyorlj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nmuxmkre.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ebkxpmnj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vdqimtaa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tzadvibo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ipgqusvp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wropxfcr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jbmmaspm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pksnnuhb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bhecpqeq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fihgrdui.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lepocvsm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bxzwvrrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dwhuwltq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ifzaufac.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fmjylmtn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qmdvsxtc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2egzkylgh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xuepeeih.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzdarfal.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ftthabdj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wrsonzhq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2owmynbtw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ifuzscba.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2owbztdri.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mfmuzerr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nhmjbwlz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdpzjsgr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ydcsctdp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ykwqcroe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tcxgtpsy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fipjtsti.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fhrpkolf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jajdmuqh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ffdljavw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zlhhfkyp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pchlglcr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fimmuaws.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gpvhyztw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuyulkje.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jkcejrxo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdmkdggt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nkwsvjbb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gzpvjszj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxyoyrww.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ryxrfkmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtnzlwfx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cnqhokhq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wxetphre.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxaevola.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bmibwobd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nppjekck.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qdbodqrk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2tgxcqafn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ocnnvqnx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fmihedxf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vtabehgb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mykxtxra.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ffiknawe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kdqyztwe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wlrsstpp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2unpkxxed.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gpejtrby.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pueidglm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ovinajdy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rpsvfcvj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gtxwexvz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cxnbgpgw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkicyyih.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lsokhdzo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iyxwhvkq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uqowxtny.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yxyavsja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ufvrfsyh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qcuasjgo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xvyykdia.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kfqpztme.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gtbktbqd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wxywqoyn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2adrwjxct.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zuyxbdsm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jkpijlrz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2koqlqmyx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yhitefga.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oxfyhscb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xztixtyv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2remgywqm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdcqya.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mnfwujef.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bcdslboq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sfzkznpz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qilqcsvg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2eoltyyal.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eslfsijd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yiahjrwe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bwstzmuh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ajzvnjba.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lciuggwc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kekvulzo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2htvygzcw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kfhcxrma.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uupprodr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cigyrbdx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kzuegwvj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cxqyhnsx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vkmxqiri.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivklcobo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lpjfkzza.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2eskxnsmm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2iherfxyh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fhscbpvq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ogjfrmay.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2phrusyqw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ybmagdow.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vciuetwt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sjahvdrk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hyzerybz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rfwdlyrc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qzsevfby.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sqagwosr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2koivzlag.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wvrwiutu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2atyeooub.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2skzppgja.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tzavzapb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mupvuoqf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uvzfrilf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bzvudsob.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2guyyqbfx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2amktyjiy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xqlnsbgn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2byecfwxf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2raexbcvn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhkfxzzt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yqmlocpl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2essarxqs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bdhdnsrd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hwkndpnx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lvijyyvp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2edgbawki.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yqeegagz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tlmcucot.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wqyfxtap.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gqcxyygs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oitltnqq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fzmcjgtq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmzrzrza.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2etftfwtp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qdvqxyey.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2udgblorx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fbautywf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ysijpgtj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tftnshfe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2llkwhcaf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zvahxsbu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bxjkyqym.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tfhhkqvk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffhwpafi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ywpgzaah.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yjwkkfwh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2iregiruf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mfexzsut.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ccofxppk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xbeizfwy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aodykser.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2foaavdqi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sqwcjpsq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2akkuvfqm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2peybuwel.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oyzsgdzr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2prqeekmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ycvjudpd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mqicsgmg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ivovavas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwewxpvx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ldokibys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyensfzc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2alsttjtk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kxzujgmh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jmsazkse.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mdhtaarw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vdkdiyqc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zjauxjoz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gglqpirz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gwtuytjs.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nhiajumq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fabiibhv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pjcuickm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mrnywikz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eqnbqksp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2anhirloz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wvfpestc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zfpvxktj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ghckjdbt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gmjbtmuj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2okyeptmk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ajgfsacv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jlahbbgf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hxvdmdea.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mwzmguwj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsdyzhj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2arupbasu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2luoqcjqi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2patqvjik.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zckfnyjr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qhefnvmn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rpewmwrs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkdalkbh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2opaykwmj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ihnkcanw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oppvenoc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2akzvnptj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ihtaxvfe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fmmlnnjz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gobsmetw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pwnanbpd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2syuxobnm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2meojallg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rxarauul.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2srhegfkv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bwcccani.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2netgvpyy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnhianp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dkuiehly.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pzzobjei.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lxectblr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sgtnrdjp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ychpyuzs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mljbrdqh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dlutyimp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2plgfaewj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nptklept.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vldzieno.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pvvzluvx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2goviuphc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xtlxxnqj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bamogyos.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pbohidpm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nygkhqli.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ugidvfzs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bszdsrrb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lzcfjutn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mqkfzhnt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2aucmocwp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xqcowscv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vyzsakbh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2avhefapk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qkbfxlrr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bxktnrso.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2auoaksyv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nxjgqhdt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qmcyxtxm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2kclunjjj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2czydbrym.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zjbwaczt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mhewlldf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xolemgkx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kgaryntq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pkmxmble.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2elbvjmyi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mdewtnvq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oujshxup.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ljklbtbf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rmwkcqxs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfbkrttp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lrbrwtux.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ianvhupf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2cdbdicvm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ygwkumay.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fehnxrts.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwljhpij.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2avtzjpiv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rzqnrcow.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jtequdpb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qedfpogn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jdmesmnj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gcpsokxd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vaxpsbgk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uebxbwzn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fwafovfx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jjrfqmhu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rureowih.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eewxyqnl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kfpmdgvb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2owtjieuw.html


<!-- 参考信息 -->