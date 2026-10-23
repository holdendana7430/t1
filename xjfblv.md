代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kkjsunsi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3aoeaurgi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3azfpqqal.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jmyankib.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rzyoucom.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uvxxjxvl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jwjttalo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cbsehwia.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wbqqqnzt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3npctesiw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dbtlxnnv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhsivnvv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3apcniyow.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sycqdwyy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wiskruvd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lopdcdhp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kisemmcn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ipfgvqrd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3afqxxutw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mkzmlpdm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jizkplxg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkznxciq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cashahbs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3amglngva.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fbvryklo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pxhkghbm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hzzzxood.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3oxgcvhkp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cxjghmcb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xsrasiwl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zvrkesaa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cshfvjjs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hgkzuckm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ddxtzlyl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3thvxbydb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vuhanrqi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tdeeqzyw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fxtxgrle.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3epkrfrgo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3oieowyfh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kkodbicm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zcotbids.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cdmkumas.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3abhxcfzj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ignytbay.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ywmgwpig.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pcmlhcjo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xecththm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cyaedmxc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pmyffode.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nufrapgg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yrxqprhd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cirnhpif.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3azcwstml.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3immifguw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qorrpiil.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vkubornd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lfwjjfnj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bgihpozs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ajcctbbd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eixesqmu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3winwxoma.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qtdnudzx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dhplacae.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uplpfsmv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zjmunhbw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hdzkrfiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aevskhag.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ugzfisxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylzzipjh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjznmihg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3eyedpgvs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3owizwclh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jvcmzpit.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3npsqwyvl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zlrqldyz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dlicmdjs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3psqdabkw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ifsqskea.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dubixjub.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gzxoevrz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3preqsswn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uhuedhub.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3klmyobnx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xfcgawun.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sfjbtjxo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ludkxpbe.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bvltertk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rqbtzamh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vyedqgvn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nunykieg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyvyvfhx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ynwwybtp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxqfvre.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gbeixgwp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3doylvkmq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxmapwl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xsfhikel.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3piutzutn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gylwsjmk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gvharvba.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fpuxxmsc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lawxihgg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mopczjqs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qcujpwik.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fefwgytz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dogygogr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xivlepke.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hgzftgpf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nxdfczxu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xppantcv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cornlxxp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oefclgld.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gfamadco.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vgatbyph.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jhmctlrf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oeiavgek.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mptiydyd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cpwvqsha.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tluiumnc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bzlmcmib.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uuvcgtvb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3acvttglb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zemsldhg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bjipekqt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uzbxcbmt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3drsjnlgr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dpwhwtwq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nguoblcv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zlfkxrmy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cmmjbczg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xqkbnflp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rfacfgyy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ukpddaqd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kicpyjvp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jzhalrkh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ixugiykr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tybicjtg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3tlcweajc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vmqclfhu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vszzvkbt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yzjxxlti.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3aocllxdf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttcsaitf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nznghgrd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jpwujmep.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xezssgyp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3loosysni.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mcxqktzr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3twttpahi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3grrtpzrf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wypggvrs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kbgtvqkw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gvuztbmb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3obzxmahj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xmigmabl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vpnonyua.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oshgwpll.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3welhiton.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fsjqjzac.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3idfipsby.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3uejpckrb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mlcnrqqt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qrntbvuk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fglikqma.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3pebfwfwq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wucsocac.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghsaaugh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pffpnkae.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uekfmzqt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcifbldh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kivqtqpj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tayspkya.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixxksllw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jsxkgdaf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3itvrrmjn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uttkalti.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yhnfbjii.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kmjupqzr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cdpxdgrl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3houaozil.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kekdyatf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gzzwsjvg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fdhkntwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3amobmznc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wlcifxdz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xesqfyad.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3egbcxbie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwasgujf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pgtmwrpx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qylplezu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uaptgocd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3huxmoevy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3twjtydmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gelvcwda.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gncypbvp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3svbajmxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fniqfzid.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3itzdmlts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zothgijf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itslcztk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ngalvnuc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3efwpyrdv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zruthffi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3npkrxvuo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3clqfujkx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bcuvqhbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wksuaizj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nrgfmdcg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wgzthpkz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xgowxsns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfiuqraa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dnkiieyp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yeizvhkq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bjfqkybd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzbmbcl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytxhrktw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hvmqigco.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdlugtve.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ewqygalb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3psnecipb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xjyihxdw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zcrmhasl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gxrlqsft.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oetenqsl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ohmawcig.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wsdacnbw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zddodqhe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jxdnipjk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ijuqqgtk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iiunjksf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eqcxypsi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lmshrsez.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dfyjvkqz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zwzegkau.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3maydwbiv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qzarxfau.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ergoaozs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kiufekdi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrebigt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gtxlnrks.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3oqkazbhx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ybqohffx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wjolwxxy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3utjlmmir.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kuptwjob.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ldabzzfu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jktgeiwj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3adruobid.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jrdwfcbf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zyxzakxl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jrecrftv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3plajtncm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xbumshbv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ukmtumvo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mbenmvvs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3evsggszh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vllrughf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xlsoxbpd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vjdabujo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlotojmc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zvhxwkqy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wgfafxcm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nvqqyobx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mclwzgqr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ynrepazi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zenjeazf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qwllckrt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3odheoxds.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nkzclttb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdngimkn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3iqbdipti.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3snqgkkzv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3imeulcjb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vdykbgzs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sofdrobg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ceyjbsgd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rggcqeey.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3evaswynp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vxucftuw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fyuuvdja.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3astrukef.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yuhsvske.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nahdqmln.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3luotxgmq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rcjbljxa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ojyzgnva.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pmkpijcx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aoqpbvqg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bfgjpxge.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fnsxydjw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zyitujnr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ygriqmow.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvawxtwg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3spxqgipv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fmrdazsz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iieyxmtu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzufftyl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lfivtlms.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkgfejz.html


<!-- 参考信息 -->