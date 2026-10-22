代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hnilxhun.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zhclybul.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kvoibiwx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mgastjyt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2iqiuxfal.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jthheskt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wuakykfo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2syylbgpy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cznwajjf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2thumcvza.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cyiiukud.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2chtdxrbs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fomkdlud.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2htakdbgl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2sngkbxzw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ngkhawvq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oashwupk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nbtzfgcg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vawlorsj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2drugomon.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wbhrdvqr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tfipitdy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cztfncvc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vkmccuak.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2puhdnpns.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hctdqtvz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xnmtilrr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sikbysga.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2trqeokjl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fsmftoqj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ubgdmwrp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gvrgoddr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ifrwbzpo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rjswtpcm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qlkqimgg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kfwtfqaw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2trstbzko.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hxhqiahu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2toybgwpf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sgqjzici.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2urozixff.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jfjdspde.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bqzdxbuf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qsbheski.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nxmxtrcy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hdafapdr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wykopfrf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nxjohsqp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wnolsali.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nbbndycg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jdovsajn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zvyrsrsi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uumrbcdg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtmkjzvo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vepwdpyd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cfgrhhsx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ytgfkvqc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wlwzylit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwogczrw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dwmmuote.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2syxmppip.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sxqzkmwk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lvgymbei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nahxaxat.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jldrlvla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgyztazp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmbqpwfr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2aasgpugr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrexyzkz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wksdyamr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gdpzmebs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nrszijhk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nqbeqmmm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2usrconxy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ltjtlgtl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lefriqkg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slslqoih.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2louyrajq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ckczghfs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uwmeoiuk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vtlobwwz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lqohpfxc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2oxkwdtjs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rynechur.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2miwpykpj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lbzumqvo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2prgcxjvw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cbsoxdlz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ixmxdjgr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cbgswatg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vjdwxydc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wehjbtqp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xoahfuxs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bcoppuge.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jajszdtw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tpnvjwlt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ltzgjyql.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fdoqfaqs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qchqzpwf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ktzukjtg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2casiqwtv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oosudsie.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2guelybsu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wgmyemzj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wyhhsigz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uhohlaay.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xpslttvf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2axdoffvt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rixdzhze.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sjhdvdtx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ocqtxdkw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dflqvlyw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gcjcxhre.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2elgeqwqz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2munarnjr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fszhmpce.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hkftpold.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xpygidzl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vlgzwaxx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yjdqtjgg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hjcfycvt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oysowgde.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wwmomnbk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhswzryh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rfchspqr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwjbxunw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qvnmbsrr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fowdpwkl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2iygzuvfl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ulxilusj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2moizvmdz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qewpthwi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nygtiglt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shmsivgl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2twlnenxv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kijxqonc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kubxzqxs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zxcjyddg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zhjxfvno.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kculasrk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kvzircnf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2roubmmwu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lpyxysji.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nkplhazk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zbdfxwlr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ujfpbkwj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dobrlhkd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wvwbjhko.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2doclpwuv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gjnmdoct.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2anfybino.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ahlianxk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zynpavqf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uyhcnggl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2plqdrxej.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lnjtnczm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mjrwphly.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iedsrjky.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gxshdbog.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhlnree.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nxdbsrvc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lvyhwyio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hlupkgco.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zshjtmto.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vmogynkb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qywymwhc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kuxdembn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dmxydgqi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rxzqtiqz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lqzfrpks.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xkltoudl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vqfuyfjh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pokgxcpj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ggesjfgq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sackddij.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kdxnbezt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zfsmgfik.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xzrddspc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rpznhuql.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tdexcejt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrcfber.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ephjjdcg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qlhyhtpf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2slfwufwi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcbcfrde.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hfwylazs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kyptyoob.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cxzuzogt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2scrqzhaa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ghwbzqcy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ycmgfvxl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2brtpzitr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mttjtgiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jptxanml.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jxssrvdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffovuyil.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nxktkssh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dqfcebfz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wwyhhyay.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uqvdqavv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2izfsicha.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iockbpbk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hjskzyyc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lopclwbm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xdgqewps.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cvgiutjt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pdiorpnv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gvyuciis.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cgwviisn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcdvarzw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uxvmauli.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yjgmhsii.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ubjdocea.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zhyumcde.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgswsopw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cdjtdpis.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jmbvxpau.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kktcchdk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bisozgat.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2teabvmde.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tncgtuhl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ufzxpsno.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2sjfvbgrj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ykezseov.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qdejzhfa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2khkakqaw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tpfsbloj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ryoynijq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jvqsbgxe.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hueqrecp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eypcpkzi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ekdwjkbq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hdfpsram.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yjzpfshi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ixiigrnh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zizegqun.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fimmjkol.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tuepxfhb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2speerweb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yjshvfdj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oratyujx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvfvdbd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xacgokkv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yssdnmza.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uuivlbah.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ikcerhbv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zyexgtty.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tdsynpcq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2klklrozd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dkgmhmrh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dgnurbfk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2soijbfom.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fwrjokuc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wlsxflgr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2olfietux.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lnbwufld.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bsjzkzgt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2szdocnmu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cfbcaowu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2svyicrey.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ojklobnk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tzyzuzql.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ireajvwc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fbcijsnl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ihnslcdb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bnegdiqm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbdghubg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2buabiuqs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2eexthfer.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gguokmif.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zuhxgvjo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wynbgdre.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kqeiimpv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xxczunue.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2swoyogob.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hdsizczn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cnzvieum.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2smdfydqc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2oafsdeyf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qlztgbtq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2agufnbpt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dadxhjeb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zknaefqo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oypbamyj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2shvyabqp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jugeilti.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hiteuvle.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jsojdtxl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kcqkvohy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmvqblx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2evbwxtcu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2arasmsfi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkeaqhob.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ydgycfdd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gztcgifo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uamjqdqo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhzkks.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ogxegvtd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uxxkdutw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2icyhyazn.html


<!-- 参考信息 -->