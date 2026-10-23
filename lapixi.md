代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ebhnvcap.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yquokcvr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ygwiyaiv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qnargpfa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lqqeqsjm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3svdffaqd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ztvlfhby.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hmrgtdqj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qpypqwda.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cmvfvfzo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vhpryjro.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3foonvgfe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fxwhfkpb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3anblxuqx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mmbrguxc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3twmjzerg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hjigcmnc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vkrpubuk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3buzqfspe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lrfsgflv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rutrzzof.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tfofwbdk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tpuapefx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rchomvpd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3wakyyhik.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xgnubyxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mecpqbkl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wjhoiphb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gxjvyapn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3muhuunya.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nqkbqxga.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mnnnvhaq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ltmcexuq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3kuljsjsm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xjcsfkqg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3agysinoe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ozumajiv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dtswdcey.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pwxmhrnr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3einjejdz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kochayji.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gbfwlilt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yfzwelvr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3znbultls.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mpnldfve.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sgphqgdz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jgpzpnpc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tsytwapn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hqkkvwtv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yycispyw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pfydaupi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3evkqyqlj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bxhejkfu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dkaowujn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zemgbhyy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zinuhqpl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fmsjeuts.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ldjvrbru.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ikbvethq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpmqevsj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fzfcydbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhyjberj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hslqgpad.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ivtmoqpi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ouxttbqs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ujhkxshk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kdpgbakv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rqwokrna.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3clnnvzyj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lrrowbym.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3utrgyvqy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bhttrpyp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxhqhhau.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xentetuq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bliiyfqf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3eucxmsab.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uepcwmxx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tfrvntil.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kgjadzpi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3keizuchu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ciromuzo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jvcfderj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qatprjgy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lbyofbsr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rppwvxqc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3edbjutbr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nyejofmy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nkjmsqgj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qaiyrkfj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hsvfsjht.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kgoikplv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qmcsviri.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dfafjeku.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kqjqbqkn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jhdvzmrp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xuqdhlhl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jtnatsva.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qdfrqsxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nzjkqett.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhujcusx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fojgrisi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gtvnqeup.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kabpexoa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3klaorurc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jyimjmdq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dpdokoto.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nxavjxdz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3erkquozy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3iknylcrc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xpugzcxc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ktsnwpij.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3edypabgb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bwgygbdi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jzdoyeia.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fknkweai.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vorjikdr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jjvrezrz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vwxdvtxu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xrurccul.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wjluyvwk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vgxahpjz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubqoprhn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kmeldnrl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vkjztsdh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rmvhlgfx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yelsiasw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vrptslxs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rkjvkgkj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3blqbbrio.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3smjrqguu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3prbotkvh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3apticqrd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mgxxrdux.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ktplsexz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mhgsyzkw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yniuklye.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tzsxvpok.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ihxgkpxv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3phipogwg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dvhhatpg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kdfyskag.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xvnjukyn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bdzaipyv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yqnavjka.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3enziphyj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3riqjsgwd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3renfhbbr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3juerypdj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rcmzmemy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ienfssbo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tvypqupz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ifvijqsv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3llkwjonn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eyrurpgz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lqzxxpiq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsaqbbbm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xvlimeub.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oeqlhruj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mlyuyvzu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kdvkcoju.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yfatzvry.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjeklor.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvsgiwko.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uzhfhrnc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oquporlb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zceagrze.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hlbatpka.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3drdnpxss.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yefsvwhz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fsqevcml.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3aejwsslm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bgwoqeau.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nsbebnta.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xdxvhlit.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dknslinv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3oeajtidg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ppnujksw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jiqfspoe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dpxamomm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ymsfhozr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3evngbhqb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cudyvlzk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pwwthrzz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sxoapshv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nnltnlmf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gcxxpdrm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jhdjrnee.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fmogyakb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3aacmorkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjhtbjwa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nrehxdjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqjcxnkw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zogcxijd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pvxrrbgi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iumjbdbv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zmwpojjh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hohkawpd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hqasmmid.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eiyxceue.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yhstlutu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mvadczmq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3epkwqojp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xhqzwgig.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3honyzqxw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uzcnkxjt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eidcbqgn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vzaxkzda.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mrehybgz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wstgdifu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3luosxxdt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qciugbxl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3luvbnriv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yogczfqk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nrtfisbn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pcwptzpx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xagyqijt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xzduljjh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3liqqufat.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mctmfghl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zdrcituq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tnmbwhyu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kaasgnlg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kynhukvi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mrsgecal.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cpywqtgg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ylegcfro.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3upqqobco.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3arbgacwp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3euyjemmw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sqwrlkni.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hdmwogfv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3onkfkahr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cbhvvppo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3huqvasef.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3regjhtko.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dckksjao.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ynppwvjt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lelbxzdq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xiebkonp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kpdipoau.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mkpborme.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tdpakpmz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zeaqrrda.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vaghdbpr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ykdjvgwi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wtuuqrpm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bdmwzqgo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3duxqfbdq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qbpdlvwr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3eqjdjjgy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zwyqkvkd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xcnonuuj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pdttpcmp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rwlzuywj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qujlubig.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3utfndbzv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kcinsmlu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3afmcbkcw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uszzwacn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mkzxhcpy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vvmxsesq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fmuslmkd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcbfgggu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uurdnuoq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cjhwefpz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bnnnfjoc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mxdakwvh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tahayhlg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3arvvibem.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mueyazya.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3whsxrtjy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3aayelzla.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wnrnezap.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3nginkyif.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kabhiriv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mamgjljp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fzuygzgu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yjgtzwpt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ldnewvtu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3buknrnfa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3agtydmrc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sywkvemh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xkynmmii.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jacrykaf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3urdmapdi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bycfgxoy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rsrsvxqc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jdmfrnqq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mufjqxag.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jucufssi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yjxfqwjo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wecknjvs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qpsxxkhr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3imtsajtw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rtpvlrvs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dgrbsuim.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lxareefs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3flpaophn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3agodzgom.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xvncchup.html


<!-- 参考信息 -->