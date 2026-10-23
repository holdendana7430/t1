代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3scsroxdv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fqzlfdxe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dagtrddq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tcfcmtkr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tnztcexh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oezymkxa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3elhunwdz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3elfyhcof.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eufltkga.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3atlrsjvi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uqigybwq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qgnbtzhy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uedbtogd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nunndjai.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gbwxbzye.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nazgwzzi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zmxrrlek.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3smwedhrd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sesidvvv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vtltrsxa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vuoqeela.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fjsavsnn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3odvgsgiq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kprmvlms.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cjadyjlf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ppnirczv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3oazfzoha.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xnduivfe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yrckptny.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3styueyku.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lmsgelxo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3btzqwpyu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bgjpjcsw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3exzshzpd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pnhtctfe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kogfvthc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ztbacxhz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dalurpyp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bogjofui.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wnkthpsz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fjodmwrm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zzhlecvn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mczqjcgc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sidixcaj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ebuchnod.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3utevzlit.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3naabtggi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jgrnpsvp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rtrzvcaq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ogqjexak.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3iyhqetdm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3naviedwn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3yhyiwcpk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrfpbxst.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eyeedkak.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tyagllea.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gihsfmyq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qdftevvc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pjjhfpsf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jxjrwfyb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3yfnsxsgg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hiqngoer.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cyrcbjfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbjooqfh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tsetmidu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdbhkcic.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3geqmnyhn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wixitjpa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfihqoay.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vwbhsubo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bdcusawt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vlobdyxs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lhblfxjy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3natlqosw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qhysquxc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mkxhsxgt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vhxnkaoh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qrahrdfz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kdmtpupo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lndpsmso.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xamsjomb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vbjudkon.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lyfvblyo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ouczygfh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yofadmqq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jovdudti.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3letbrilo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hhpvolnc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ohacgobs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jxeyweqx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dyqqkewq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkvmkbin.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tfiuwlui.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rniflrji.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bfpwzzth.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zukireil.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zjrandll.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uzmmzsaf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hluyubaq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zrxdaxya.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3usagabht.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hvttcjgc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3neayufhy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxnhoaoi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qynaqjhp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nwtwxgiv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xjpzjkvd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rtmsfgcy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ngbxnuzo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ptwzwgty.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wqpuekbx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ytuefzuy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3muhhxywq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ottmvmml.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fmfdoift.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nzxyyutc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3umddugoc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3apcucfxc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3cumugzhs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3klcmkifn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iwfxithk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pkstnhyb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qseplpux.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fkgriffy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qtkirsls.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kejuwwec.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zgoznbwu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wwohgary.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wpqbcgmk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mmznwsrt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rknaewgy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3asmuizfa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jslhnzos.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3itzmdrue.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ryzpaske.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tvycjkmn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xekpgrxx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3issebcdw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jwadxgzx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoyvkimp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3igbqfuwp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ypygewjo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bptwdlwe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ositqjhb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3siyimxzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3coatyqdb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3msvegelj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ygecwfrl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fcalwzwc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ftaptvbn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iwhliqez.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ccimbbyp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aeywkccs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ocwrngmq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vedtkeuz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3keujwxiq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rgvtulzx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lujhjlak.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3oqojvehq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwayvda.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3icdxhnji.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gkyilogm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jxgcypmk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqjsgjba.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3putnmeiv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dbojvhjr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjgnjdmj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jbouvyzh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eruweerx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3urtdqcte.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3clfscrrt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3oaekeeho.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3efsuriij.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdyivfgj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kyyntgbl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xyaoqfox.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kzxnksgn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mxwmsvim.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3czfivmzq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3enisglmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fokhnddw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hlpjcmsp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kqseuyxz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zzvepygt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ggmlnabe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hlczojxi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3arubzwuj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ponsvesz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rihxixur.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3euhauecq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3efhcxugd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wvlsosus.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mjoulxjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjupjqzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3insltcxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyguuruw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sivubrzs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rvztfuzk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3upgqubwg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fvfgfaxm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qduohrgy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rsmwsipu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ibtusmkh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ceasdcjq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sbdqldim.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ipqcrxrw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xfdprhrr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cjokelfl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3raazekdb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjezzxay.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ysnfvayv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sqshkbhg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3baibutim.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3umgnxjrl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bsytjrvq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bfmgvprz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3aniekecb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bqblnbnx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pcmkmgam.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wvgxipnw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yiyzaoml.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyypqjtz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3inbbbiqu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3piynpgof.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jfljyjod.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wsagbcpc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ojozjdql.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3smzacbiq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rznexisq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kxtwvslt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qayxbsje.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ybantqrz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gpcmduaq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3aqjvkvsg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hnbeadeg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3enmkpjym.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ktlsntup.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rxaeztmu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kruprouz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xbeujkxy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vfzcjugs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qpsvomxm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3evbjkaaz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sgpudmwj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cadjwqhk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jhikmmzb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3boijgpqb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uqxnqybx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3egrqafli.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cwqmlndc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mjmpxtpi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mvjevduo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rbmynmcq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cfpnjjen.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rkayewoh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3umhljzua.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngnchqfw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3prekvvyg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3yedjklal.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wwhwrvik.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gnkmjvmp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zpgqzigu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3utexgako.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jqswekgm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wofrstwn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cqwwqgrv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mdzeqmkp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cjexknps.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ofzpfwnx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fuyppuyi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3peerwjda.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nwxlvzlj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tkvlfluj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hlfljeee.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ogplmmcv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dcjoqnke.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ybnqsvqs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tegddlbz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vnldmxpk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3amglhmyn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fmrucveo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tiigxcqs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eqterlgj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjovwjey.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mgaukmxx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xnsnjyzu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wtcjkocx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywftwbpr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ziemlcki.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mniqqpwp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fspxqods.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qsoecwws.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yncbcejs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gjfaszmj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trimbrtt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3igsxuawu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3whnlxogz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khozwodc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vuaulbad.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xqihmggc.html


<!-- 参考信息 -->