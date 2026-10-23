代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3oculzydn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nzxhqspd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evbiqczx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cpplimjp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ftcpqfnf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cccbzzfr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvpkebaa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ulbtojsu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kcbriqay.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xlgnyfaf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3plaiuqpb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fnaxhmkv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jaqwciam.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3brkjwaao.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vsuznjzu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eiedgzca.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3txplplxt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jurhpyha.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rufiomto.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wtqxpmma.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3snauyezb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoyvaihd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ovykrszj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dvmitshs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3usqyzfuc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vjoekiod.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nysdzdvv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jzjctmlr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jixbbnyr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qomaztpa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nirrozby.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wolfkgoz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3smjoturo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3guinuxii.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3juvqduay.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xtpzgmct.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ajcbamah.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zjsnjguz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3roaohwwp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fqxydfii.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xhckopsh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ljyflpcn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3amfjhflb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zwdlafzy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3suiocfjm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fohtqqpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vdmtcczb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3inysgbtx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hpbvqqpv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vnhuiekt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3avaucphy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3binbigti.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3glusixat.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3psxomcaf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xewysoow.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sluipuhg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfzhvbyl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bhybyyit.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vlnvkgwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oakeqnbb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ugvyznsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkaecewo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3figgiesk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3akbaeghg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3taseivvo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3iamlzotz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hwczdxqy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xrdkydkf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ziogzkfh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3umsjmhov.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wbodtpnq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hbxxxbvk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kwyryctm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cuamkaxr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fywxwxqv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ymgpdiaq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mslmnwgr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cmskyqlw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lvursnru.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lffgzymy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eojoxadj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ijjfwsaa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jbbovhuq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yswvjlxc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lkegltfi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vsxncsmq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lnytrvpt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcaaufdr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mtrilydu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3aayxnbtp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mtykmwpw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jdnawoyi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vwwaqmme.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zelxxvud.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dialiykr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bqyvhkiq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ezvudrzg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wmheamdz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qkiuvurm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjhbxrhh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hfehuiyw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cpdsfhwo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pgtvufjo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gmbynrux.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yrfwqtfb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ltgbufas.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nniypgdu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3twlhtbbw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3eqhdshat.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hsbpbxcr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lpxvzstx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ukcsuajl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gfqgkzpe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vyhzarju.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hmuporiu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nfnmgyud.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rlmaozam.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nnnwkzof.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iuthgacq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojptrmll.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bavuppfl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqcrwoxe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kkvybwba.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qzpqzsqg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bozxlovp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pvqrtctd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wuxqwtyj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fypeltud.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nqgdayhz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sggcuraq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvscpbba.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zmtxpsgn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3znwxaiyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zdgkqets.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xuzeuglq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hsfkngcm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iuyxyxmp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rlixozxw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kkkerwei.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ofaoowtb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dxkpknbv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dikpbpcz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3iiekbeuu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yokumoiq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vfrswrzl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3itwfsvbx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qazgetwn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3quncrfqy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mwrnuhoo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cxioyrsx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kqhbzcoa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mzltmuwj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jzvykrlw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xdbfeqjw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qukatewm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhdvwotz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qeqlyvqi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kajsbobh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ohdqbscs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zijaxzzz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kyrrziss.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qkkuuuth.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkkitzgk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gurjsgyd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3kvzbkfra.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fveiknnp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3iexvdtnc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rzkarlnc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ibkvrzwc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zojuefxy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sjqbhora.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3eyuamckk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjpglafw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dtqxjosy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wrkwzzcw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cauyhfgj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kxmdydxw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pdapggcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3owfonuzb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3sqlfvwos.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3qesbsiss.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zxyvdwsv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eeoitttl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qyasknvu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sajshvqm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rzoimjfm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3nbmzphjb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ebwlgbab.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3byoevjik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btwdwodt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3stcnzoah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqvzuxdx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dmmrpeza.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xjacurmm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkberqgy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bwfwzprz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3labuifan.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tdzjelxj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ysofgeyq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vdxzznth.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pcrojqyk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3aktghwsg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ayxbsquz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xarrnpfs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3shveksqv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3triadvbd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wwhtjxku.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xuewhlmc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vywnhnak.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3txumcwpj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rgllmgih.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wiorxogh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3llkmneco.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cjrujyse.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ckmyyzjs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qyepnkqw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bittafvq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbtfiah.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vwkqkjmc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gypvvowy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3virdscqh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tuqekuer.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nwgarynz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lrqgxodx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uxvgprup.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gigskqpa.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3itmjgcur.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wofhxjwd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rzuazprb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fmklqkvk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mymuekqu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3couwauwu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jlwnruit.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jnshhefu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fqaeygbe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jhtrthps.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykskhabw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrciymi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dfrfaciz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptqfppwx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lkkowckw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uumdensn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3havavocu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hvypuqnk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wlfpaffu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3evofvssy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tyzrazwd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kmpethyo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3seuylcnt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vwqcrsph.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ctktnlaa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ziqyuhum.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3osdtrusj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gbnqcvnb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ijbjqwhw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vepzetnw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3auupvzhf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3odewoort.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hljlwbbf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ngnfysho.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ftkrjwbc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qrcngqfw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eggiyneo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bvcoowxc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fftnorkj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ohhpdwix.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3orvitajb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ygiobkfn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xlycprvu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wvkfxghn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mklwaozm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wgukoabk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hiwljyum.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zaokukbt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3btewubze.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ylhfzapt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3blnjzbsv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cogfpqod.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zhltsbll.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etyppxjg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3krtqzfzs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cshzmzae.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3eslooifb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngpzquiv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hzavwker.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3njdljize.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yaktohdy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lcxpllxv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jhiedypy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uqamnkgk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmrnlyhj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xgqrdsgb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvuiwspy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nrpuugrd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3svkjkbca.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3emyhmmcy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3glkefggx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uvisuoeq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mmrpeqhm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3omnowxxw.html


<!-- 参考信息 -->