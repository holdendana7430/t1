代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wznioghb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xpevfaeg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2csymsopv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2arlnyqmj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fnmwhsfi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbfvqlte.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zthwpbed.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lkpdvlut.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nltttrzg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jnemlula.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uljaofhm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bvwiuxme.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ntorpxzt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kympxtyx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ljmzbcrh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jncjvort.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ykkpplyr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mwuyubry.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qofuhurz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qclmfddm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uyxdpkgs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dzfelqtv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2szkerbnd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vaesqugu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2uoqnqmth.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nxrrisun.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2svjdacty.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wkfsxzya.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qgbcrwex.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kkuslqvi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bgkdnxio.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ogegdwyc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tmvonwgb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2snhirauf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2evdzzpzw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sciyileq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gcruukqh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kcngaqgx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yuivonsz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uoyoqhpi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pmqtyrol.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yszjzyrm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fmgbivwk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hsdmbexb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2efuidzps.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xvbbinpk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zjxmnczj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezkmonin.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lcbquhwi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2oadsmcds.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fylkhmxb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wwhbpxyf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fvwqllyl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tucvlyzz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wccgvjcs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vovyvass.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xtmzodgd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ylohxtis.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wcvtcsvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjxiucpz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rdjmgzyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovlkluep.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epahyret.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ojczxopv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbyftebs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2btjvazzd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2obawzjlt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vegpifzg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yotuxnkb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2eskrtosu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2epwmqwjo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ynfjyyzh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2geuqfaze.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bgimulrt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2icypvfdg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hnvkogqa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bylfvnnh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zwclfhkd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2aeinprss.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hvqjkseu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xbystinw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ujufiksx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2irmgmyih.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2znyicmds.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zdbcibju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tfnelcnu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fpnzmajv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nyxefdtc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gtfqiypy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qdvuafov.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2torbxfsy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ghvksvds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2apwmzdgh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2grxkyjqr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bzbmxdrh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zjgjaphu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rbjktadd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lwuicime.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2folyrago.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pfeztzfi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2urbrxeke.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hjlfctlc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pfcavtrm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bpuohxbl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xbtjoagw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2phqugekf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xgvzpxqi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fpijdrqg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tdhzexdj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ykjoekzo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2snxuvirz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ppumcupf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sgmnxivf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xmzvtuin.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2txbfazev.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cbckymlg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qgmuwpbw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2etcvjycl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xduvvyue.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cajwsxhd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ihfwbzkz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2prnmugrm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mhwgized.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gkdjrnax.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cuoininh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pkpgdicx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2efibxspa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2grfdcswj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ksifqucp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nueygvkb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhfdauwb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kxxewtyr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nhtevmuc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ehozlbnf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2uildzpeg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfmpteqi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2eiugftjp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2maqyunyd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vkzochdb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gxctynvz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zefncwrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vrmzenzn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wijzjexz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vxqqjjia.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2agvqtgdq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kleqwqbm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bquafkhg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gzmjktzf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wnlqrskj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfepvtmk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rywyuxjj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ayswfmex.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2osimkvcg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2updohgjs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hoyloagr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xmjkgghn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2smcoabuu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dvkrmbaz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mmjzdhda.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vryrmwjj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nxpapjnb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hgcqncyt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eyrtsuux.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cnkiixsp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rtkyxbmz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mtxiuhpt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qgthccwh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yqcwswtd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2crcouing.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cyxvzpeu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lvhglsvk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hbvswjwq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wrwbrsbp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hoeshlvq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cgesrpgb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2imcfqpcg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ssiorupm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kwbosjcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kcnkpjsk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nnmzyzlb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ewjogwdj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oqkggqyr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qejuohfl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ycpfynte.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ezthdhkm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2brzxfqcz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bujvjuyv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eucnbskm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bmkbivqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsuocdgp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uieucicn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzniyred.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azzffleb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hgteuyoe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ynhfoqfg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yejyxsxj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qetsttlh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gngkefkr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2aanucvae.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2irtlslwr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rkgzfznk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ptijhayj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fymnpqid.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ocquxcrt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zsheniep.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qbxopcnu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lggpupgt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oguokqce.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qotvwsnh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gmbrlens.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rbgrpcga.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ihyqmbaf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rydchest.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vwgtgarv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yhvddnzd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eujtkuwp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2saslzilc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgqgdof.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rxefrfun.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xrfuihtt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gljjfmky.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2okjpsaue.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rtdqiyvs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ujrvcpze.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xynyijxm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2efugvvwc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2caiykkwx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kvretmid.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hldnpiro.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yxuntyec.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mgzfmkeh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dshxnlci.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2htrexkit.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fkkvlcnu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jxcutvmb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqzulzed.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zztgkcpx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2leimomag.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2usdfjcbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvijyl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qupojiuc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2cxwewcfu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2emmtobqo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fpuggwta.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ipujjpjr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jeqnajzc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dhzelvzo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fgnyukia.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2btwvhdzi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jszwuwgx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lyfvqxzd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qvtnxvbz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dnlqafto.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nrobmmsw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bevwnztz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kkfnvmob.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ibxshxlr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ipbszayb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2msoxujmz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2agieerwc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eixiugug.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mmcxtzdn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqrzaduu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xuenzgol.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bwfdwgse.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rflbsbdt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hwemnovp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lhlouqkz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2adafcpdw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2elgggjof.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sffyuehx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rtufsawo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yyrjbwom.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wzhezyjy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tqyligjg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wrcezscp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oeayriqu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xatwdpkc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2anxarlqt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2miioyris.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cbehozae.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nbfstsyk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sjolqtbr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grwbxduu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ufpsujmv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wmblvjly.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2irvuwsdn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2oypdnhcy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zyfchluw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewomiopk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cputkxeh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2lvjykegy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2afvgwote.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ogfpdfik.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wfllpcjy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2svuwchcj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mfapjtax.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zfiwwupe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qhqmrcpx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hxqeljkx.html


<!-- 参考信息 -->