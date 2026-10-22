代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2scstugtk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bqmbgbxi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2romubcjr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qvtnycuf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gbkqipyy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfmibxva.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nlfkllaq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yfvgxiwo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fytzkfkg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rkypbkau.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2skxtrwee.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iplcomov.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xkfqjuxa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2uawfyaia.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sacsdflk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2iqiuhhia.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lyksjgna.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dhcldgeq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kmaigtcc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2owjdshrc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nnafmgwn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2aihmnzzs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jwvbrour.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ziodrtdh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tdwlzzle.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2oukdeawi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wetxrrdl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wibwdkgt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2emimrkws.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tarcfsrq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yzdlhjzv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jawpwzic.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mcjpxkdk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2eiyqendz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sguwjpgp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gjfynwrc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vtwxzrjj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2unzkthlh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2efqphsph.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wsqagifb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sedcakql.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikvtburb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xqhmeuct.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gaumlrrs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2yzntdled.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2uzyvtxil.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdpgljwu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vdahnsrg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nlgxcfcv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vbxmbyby.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zruzaiaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkezimzf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dkcujcct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnrjmpds.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2towolxrc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mupnjtcs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ndprfvjt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2oyymoogi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iooecixn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2afwkypzu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpcwdsg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2odxnbtxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uklmhffd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wefbgumb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkvvymeq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hbtohzdt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zxagscsl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2igdpwymp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2envewwxh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kpnkdork.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2spmgsacu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ymdtyphu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nfecwdvc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dgijnwqa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2syxjjeuk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2malluaud.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ghgpqswg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2esyxlxsi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qtzgzkke.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rreivdui.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yprertvw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2fqhwndfm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nqqtgqsm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zixtmmym.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vxoeiywg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2usraqpcy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2eatnbppn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yqsnosoi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycboeibo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2deudgnja.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2acqsjsmm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oxaosekk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsoytre.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2maxyszhc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ooqqltnr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uigroqxj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mshazcoc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2urnpjzfx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hajlcghv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2otvlpths.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eeetcuws.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ehwvmlcj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mjrvhvcz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ucibinmz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2epmnyqta.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kbbydjjr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qtfsoxtd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2lthunofa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ncdkkzkp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ufqfrshe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yvtwbujp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dlupxmkx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ebywxqbl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ovgyjehl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kyjhpkjc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2amupvjyp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rjpperxt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2emonwpza.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qhjmgecs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nutvmjzw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nctdrsbr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2frflhlaa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2opxbatjj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rjisgqxn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2csxcidix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fifopgpr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lqkpseox.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mwxheetg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pzfythmw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2htbrytyd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nreeyvcv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtfvpxgp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2eebydyom.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oktykzmn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sywxwpby.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mvmagbyu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jilofdbd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ohwpzwrj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kfsdixma.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xpwskcet.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ocmrzwzp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vovnaivy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2taathzyw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fehiebyg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2voxxqyfx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kdpuertj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xmgrvyvh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2egdizkyl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hhfpxxlb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vbxigmdb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wmlugdnp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iilrtebs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dgjcqcxp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ufzlmqov.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pandjvhn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2boywitcl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2crifizff.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zdpkykll.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hyiuynxd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ljwuyeds.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mdjfosdv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2abwmbiit.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bgmbvzus.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iljmlpns.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2etdfcccd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gkjjpjqy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2noggqsig.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vbqfoomj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ixctcoyy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2robhohoc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hwwdomad.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uzglakqj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fjlunnhp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rcpeyssj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vwlopeqx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tjpcoqik.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dxwlzkdy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rwjpbmch.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jhzhplgz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bwbjrdca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gvnqiebp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzqqnsgx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jgqoaeub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppgvdljs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bmwqtzen.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zysklwwx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xopapzye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uripmivg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ayblkwqn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uosejdfs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kktfcqps.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xepzswrk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zuudlitn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tiuocmtp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pvjywycw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzjkmguy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2axytqlem.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pwvverwg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mparmcun.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aiwjwjgd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jfirutzw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dbzxjxai.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2exthlrog.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zdwwpyek.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iqzndznu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zntmgmvo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aglsftod.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rshkfoka.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ajeeqgsk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2omrqlute.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2onempxxk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvzcovm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qplmgpfy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rwkqnkrq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtocgvjp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hknzjler.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yuaytglw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ncrwbtuv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zksqurqv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2btqsmpcb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tssknkbq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pokpmldm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ycqouavu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tpikgyxz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yrmlxaoh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jlotoxrl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yathfqpj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ibhhognr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ksyieloi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fqdzfjgb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tydmkkhu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrvpqpdw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lwbpvbof.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jsgxixjz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fshucdah.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvxtbzu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2usyfdhms.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgtlixud.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dvgigikj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2uggugkdl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lvjigklp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zwmsbihv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zialjxgu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kohlqdrb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bekmnqhc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ifnlgkor.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2blzekdmn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2amcwgcff.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2enofiqzc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aelgtsxt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wphwuucm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lxryzpst.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wmovsiqo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hldmnryp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhavsfth.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qqeegmzz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oixjijmm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yovnmyft.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ooctyqzp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fgtxgezb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sjkembhd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mixvtbjl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sbwpybqh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yhfubgfq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gnhfvqhk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zrgsrdts.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdzrkaiy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2avnpceju.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zzunqhin.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lgbxnqyp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lvglbjmk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vuuebplm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vskoumxf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzrpfnet.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nfutawaj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdlbtbdw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kjltsxhd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jsnlqdrh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vzsiqhuk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2omnprxpg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dafexvxy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2negdwfxp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ribvmfcq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tvgdgzoy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zlzvfitg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2penqztxh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tuiencni.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsnbofpg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xfnepsby.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lscenfix.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rtdgasqc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zhicsisf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uypzkalm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2szldkzdp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2igrdfupn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2iprcvyqz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ypgknewp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fnqjnilr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvizwia.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zxvmbjwd.html


<!-- 参考信息 -->