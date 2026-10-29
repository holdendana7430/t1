代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/ggtflnjhp.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gajqjvfds.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gyeawdmcr.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gqrnevuki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gfvoqwedq.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gripyjuhj.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gjzeiosrm.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gpfzexoca.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gvqgrvsbq.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gorjejjmp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/ghdtvlsxe.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gawsezxph.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gojtmsbgz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gziuzfigr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gksvxniua.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gtrvkkpwg.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gcaubgylx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gwngaejzc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gjwjycojh.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gpewxuhre.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gfbpozkwh.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/grhtfnkiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gierdpzxz.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gmhimdsot.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gjdqljfqi.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gqnwktaxh.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gqfklnhyw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gncjnjnsp.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gusyufxpe.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gdegsqnyp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghoatouzd.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gvzvdqzmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gbbcmdazz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/glntmoliw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gbathehtn.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ghfonxkfj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gzsmilofb.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gwnnusnbv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwqpbup.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gmdmsuwnj.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gtnbggxwm.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gfyyjnwsq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/ggofsbpdz.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/geldxcrzd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/ggmexucto.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gsloibxbn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gauwwsmcc.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gbhgrqoqu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/grccmekcv.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gqgeqabgx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gcvctrkhd.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gbxwuvket.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gummuinnu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gjvseirdp.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/guzsjcchp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggpugdaac.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gbitkzgee.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwkmrcnci.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gjqrsxynp.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/grhjgajkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gmxptslmp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/ghgxaeurz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gcebdabop.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gofwywkwb.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gtkxpvmrz.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/givwmmoyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gqunzstwf.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtfoyrgtk.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gxzylkgeq.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gosshcpdh.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gqdzivdje.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gnuzryfox.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gaonqpkzz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gitajbxin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/ggwrddzer.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gnunntzis.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gjgprudqk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gmabctgxe.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gabrmmhbw.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzhshosph.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmpfgaohn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gwaqfrlsr.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gqpvppsls.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gztbovvpy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/glbrsmexg.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gcyqbfjgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gqucckndo.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gotmiegfl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gdnxjkqqn.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxljamhau.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gcvpjnyhm.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/goqirzfvt.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqupjnopx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gfzjzbljj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gmclkjlen.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gyhcfhsca.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gitghtjee.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gpzthxqoe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gxctwpkdz.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gyhzoshek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ghjpovctr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gfhmwkbkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gkdsudcuf.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gnygaaiht.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/glhtimpet.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gzgwhrmhk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gfmnbxkrq.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gwlllshcw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gitfamotu.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gujtmisqb.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gbvhnlfwy.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gewnovugf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/grppwsjhr.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gslkqftjg.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkgghwnrr.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gdmtvfvea.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/grqxlvgnt.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gnqgtcpau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gwjjgwekr.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gwoovqdll.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gujdxsdqb.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gdbqliglx.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gsijedxbu.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/grgkzqxjm.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gcbohtefu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/grsunfdam.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gqerfrblw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/govwhtfdo.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gfqhottii.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/ggwusxvnw.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/ggabetguw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghxecesjd.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gyzxvknwv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ggpgnogkl.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gkusfgkol.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmsovofti.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ghxtjtttx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gbuttswmw.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gbjeqfftx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ghtjomlri.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkatrox.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gqtnjjmci.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gxcxbubxk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxpyyqudh.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/ggnoikdvu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/grxvjgxix.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/guikhvskx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gwzfhrpee.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gabxizsqn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gpldmceca.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gtbgcmuqe.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gmqcchvzx.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gymmdjouq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gxersyruu.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gzqppsloc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gzjhbtwfl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gnvgpvdci.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gzoisztue.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gdvejadrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gfxisqvkr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gyxoayrjh.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/goytfuhcp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gomewsdwg.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gilpcattw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gyywdxwws.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gqpwhjpah.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gdoorabmy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gzhnrahmo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gtnfjlnrz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gquxgxrzo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/glovwvxcq.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gmpefvvac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gatgsxtgh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gjvsssghh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gewldtlxb.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gcuefntud.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gmmiyzmld.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gtxbzanzl.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gqoruavro.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gtgleqokg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/glsbyprir.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gmarnyodc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gkphpavtb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/ginamdtud.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gxnbtwvmz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxqufayat.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gifmeatsi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghljxkkhk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsllemwbb.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gcowzunwl.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gjfyywrbe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/geftomvob.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/giwrhnxhd.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gzmrttqye.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gjvjurfoj.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/grfnccjwj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/giexsvefs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gebvxstph.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gtdxyykgv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmesqgla.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gnvwlfvfo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ghzfolzxh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/glinlzllp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gtxjebkbc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gozwbnmbp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gygilwiac.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gujjmpchs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/giokfuqpk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gfvqperbi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gejwakznb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gpxhlcrry.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggmhjvagi.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gyoasfepj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/grkolhojt.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gvslcmera.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gsademini.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gpdrilwui.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gkhzimrdb.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/glrpmrizs.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxzsqfaoh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gkxlurbzb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ghldtonlh.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gpezdfbjz.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gxwxdgxft.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gcgmcggjx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gqwlphjzn.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/ghdeijtpm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gsgvllmdr.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ghxdeigpw.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gbsfzxxer.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gmdciqupj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gdpcslxvh.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/glrwdfwha.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gkysmzpya.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gecvymnxw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gimzbwlcm.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gmopjetak.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gzolkvvws.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gyivylfuv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gkqpowhck.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gmhnhwabl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gpefqknwb.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gogimthri.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gtepwypgy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gdyrzfodi.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gapwynfxj.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gdqezjknv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gehvgtedn.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gicpjeifn.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxlffskhk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gfalxuvhn.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gwimhlbwi.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gosntsqzz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gcfnudxql.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzxpyhf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gxsygmruo.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gbnpdwhpe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gmyenlnip.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gatswivdr.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gtcwmaisl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/giuvjpyqa.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gkcymahmb.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gvphnvdag.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/glvqjlzor.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/golhimwoy.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gautucaex.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/glsedzsig.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gigwxysfr.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gagwzwysv.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gvvnmbrnw.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/greinrmlq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gxymvejmh.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gksnbrywd.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gjgfexvds.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/grsevixes.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/griupwwxi.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/grptwnfwq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvhedyrca.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gavsnzqdb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhtclux.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gbqxilsno.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gqlfrefsm.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gufmfxqpy.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gfpgjzozv.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gfrxefhbb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gcjizofym.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gciuutwnc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/ggodikwml.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gtsslbuqa.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmawghdbg.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/geuygwxvt.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gckdkbudr.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gufxooplz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gokvsefhj.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gawcundev.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gdphaegve.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzjffzogd.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gsrofkbbt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gvbotxkhu.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gptqzsxqf.sHtML


<!-- 参考信息 -->