代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cmaemvbx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lytodycs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nusfkcjl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dghcsfaz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ihdgzibd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nqsbilsv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ytyriavf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mguwuiuj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vqrucywx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3epfdmuih.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mggbiycr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wmxxgjis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3eplmhxpc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tehfvhjg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kvjgpqbf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zsmosgjt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fxxnxxcn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcdamhbn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3kddlnqaf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hpdioovt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vzfmlwig.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3esufhlps.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dzkjkqad.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qpuxqdst.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uzdcqddt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yrfzoyjv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ypmmkmhl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3euuxlfwn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dnjofwnf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vhazywlo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3udcvuvwk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xlghjgez.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tqtxiilk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3elhohmpo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hysnweca.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cmsmuofs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gjrovszm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3isnzjibe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vqquzptg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3minzyvxn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3niqqqvte.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wlumnoel.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pfwswdzh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xttjrjal.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hczcyiuv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ljfmoihe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gwhpizhv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ozxgzcyt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ejalijrs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vzsnwqba.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nfsjuvjl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kqyjpxvo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nxuzeolu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgtzklul.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bsjnbeez.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kvoblpoe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ecuiblez.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kbbqfkpz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3paaxlkvy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fycqikvu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jxrofury.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fmgvetzt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3irvgzyfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqusviaw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yownftcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urvywyms.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dgzgmkop.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vrhmitrz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sxkxzmgb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cxpeueqk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zholypma.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yankfbim.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jtsuiwiq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nkrknfnc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ygxrwuht.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xyilnxqr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3txmpkpmq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmjepnlz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qvdjdxie.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gvywgcrd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cprlgpqw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kqvaqlit.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3soclnhrr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fhmvqddj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jjqwjprz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3emjmdflp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nzolgmrn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xosnwrex.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hpjhimlo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xakdljuh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rwrabyzq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mycqtlib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3icqnxpyh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3meyqmwhd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kuwidias.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gvqonmxp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3clijuhge.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oaurylrl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rxugppbb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jxfzkdeb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cklgbtzn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mrcjxatn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dqookrse.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdrfjege.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qmnbyqnd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3czbyvlva.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3idgftfly.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dxwugmws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yojuzxqa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lfgdkhvw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xshyvppo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3sblvorza.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3soirhtfa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ozwdnffm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nyzrysas.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ztcnuixx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkvzci.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hpukalun.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pfwxdnlh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3eywkriyd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3odjgopqr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tpnawpkb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xudddwmg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3sysonymv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pezszoze.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbscagmx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mdnxqame.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nlxwltnp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jhiuccnu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pvawawea.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kwwxghns.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jdimfgav.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fatocnnl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tneuixkr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtthicai.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3btafnmvv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3phbooidv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kdeyhgpy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nbnssgjf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdyobfwe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hphsuegc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3icdfbdnp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uwmgfdxl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnpeuogm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3julyokec.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lrgfeacx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gnxrboai.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fbluocsv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rixttsav.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vlmhohzl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gfirssfp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3leidhbga.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrzxgawh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jazcayqx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bspinulk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kbqxmqve.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3upwzimdj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zbkalqxk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3papxmuiw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kqhgxext.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ldvznhpk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nddmzuqh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pdjfxxlv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3blcxkyso.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ulnnuvfo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nqmhzrln.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xweiwcwp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ygfafhro.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nsuljmca.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zhtpgtsf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3frytbvfc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pfjcjqfc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xfnqrpim.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3anbwtfjb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ppjabcma.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wrqfflqy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xujsztwe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jurucmbe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3msayyjba.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zbfrlylu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nzgzqgly.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ossiucnw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vrnroupy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tevtsmtp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uexceqcl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hwrznhty.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bilpwwty.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iayltppz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3byuhcmfy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kizpneuf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qhmkottd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hnpeiajl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aqefgovj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcqzaeql.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gsgupoiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axclytcs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aedwjyir.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mslmcesr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tlfbpgnd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wrkbdecp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zhfjjfop.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oidatabi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qjgaqiir.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nuxyuigk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vqvocbfl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gsjgyfet.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cajrmlbw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovsgyeqb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zdipuijx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mbelqelv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3axszanyo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uubjhetj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xdilzaiy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3psvilqcy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cgwgkeyq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ynedsmcv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pulrvhzu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bgsbsgfj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3lgiskxmk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdavuwv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mjcbvkgj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3taygejtx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wmbxxevt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rvxfflmg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xmlvqazx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwfrndc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvtqrdjz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3waeoangb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cwtbavlv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wtvphqhb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iiiqbpfq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pnpkmemr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lwuxttyc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yomlijvj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wmwhsakp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3toyoavfz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wkbdbqho.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zqcmiztv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3eyvmgmcb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qikhuhmu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iiatxady.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lqwilwjb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vuvabkjg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kdliimiz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hplxycmg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3glafnjvw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nrapcpko.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3aweeajrq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dbymzrnw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rdtcmohx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ctauourt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvltisj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mtpoxnvk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3txtjowtz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3btsowewb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3drqtpeeo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ufdnfubl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xdtndfta.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3elkbqcsc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zauqzvxh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3acoszavr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nysrduqv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3idcugnzy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bxixqekh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fgxaqzsd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uhviantg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yftjhhix.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ofuvzpkz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xwyrbarl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kvlewjvd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3prabyldw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ofdonrqy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3phmwuzaq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oglrxasv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mruqdfuc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ixzffjhc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dctzcisj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gpbaxjgk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ndapoqyv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lgzobynq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3poeypemk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wzsfjvpx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eufwdtwu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zsqsnfly.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3glbknclp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3apgatprw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbfwohyh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yozinnba.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nmijunor.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gfxujpma.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yffdigoe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3duhnlrxh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwwltkoc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nlgwwobr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqlfgvnq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tybybrht.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zdxnoaer.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hvydyymp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nwyyamfa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhxdknws.html


<!-- 参考信息 -->