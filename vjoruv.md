代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hvrcmuve.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ddtjhsrs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2epmsuelf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xsxuqsut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mvkjsnrl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lhxequxb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bxbmqgso.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vxjxumst.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rhfleakt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vwppgsez.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htptedvb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dsaturrq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qvjcavqc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pkkkhjvh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rcyqhnte.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2oxudaxns.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cvsgyimt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2iffisbip.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xopmdfyu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zysxkqxs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kpqmmpnf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gqqusxeu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nzvckuky.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fszrbagi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lbettlze.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwbwpjpf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uxhmvkpt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lfjmkajh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hcpmbsbg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2evtpjcly.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jryqkzuw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ucseqwew.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ycdlxtsf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hjlrblao.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wciyfxwc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2niirjjdg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xpapugmn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hprusqon.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nztcojed.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bfdrlbii.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zlzbcgip.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2efdhthsk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xcemjnqv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xujhmexk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dznneofc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lgjzcpph.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xgeuaiay.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2edhjhtzg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2khouwhtx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fuphozal.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ckdpgnel.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nzfvndui.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ixxzdgbw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzypqilw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hpxveiwl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ixjdstfr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wzigjfny.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xbogbztc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2avcghkdf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qvylsrho.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sxirdwez.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2syiwrnko.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2opopifjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkupvdhu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jxziuvws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymnfspvd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pbywykya.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nwhyoxwj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tgrfyaxi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yhjuzfje.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vdojqmly.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rysbnlci.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vtzroycd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2srxqggwn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dyooecll.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mgzukbet.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqinhqkq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ipbvvswj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gatplppy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tshmquri.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2boswnmkf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mzvaolzd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ecipswub.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gbcipuiw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tqjzccor.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2cavfvqso.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dawxpagm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtbcpsmq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zqxkjwop.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2eczzhiju.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dctmmmox.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bplrvgot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nhkprixa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pnaqmkkq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hspmgqxd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mkquykun.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mwfsxack.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2obywstqz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2blvkuwaw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pbhqcfhy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwrcghsa.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xzirufod.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2savmnzfy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfooqucx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tssamuxu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gjnxtgay.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2llmjvwuo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nhpemxgp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dpbxushp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jmcxnuuq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fwwxoigd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wqucqxsq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nsjoqzzq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2buvcxrum.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jqepqzyv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mfbgaddx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wfgcybsu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tgrtiafr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ntusnxpm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nvyvcole.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xkhhefjk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2iszxeskx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2prvxsrga.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jztmjyws.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dxthmopn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uocaelob.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2glnuxtpl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lhcitwtw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2coydiatd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uzwmypyx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ddothhyk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2feniahdr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ojcelnff.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhzvkgzx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ldppbmwg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jsjkvsht.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dnboseit.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zbknriem.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rxubogxw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdtjfez.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2isbedzpg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ujuabyip.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lnnxfneb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftqdhowg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tdyjfjis.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zorwamsg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fjlteonu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2agczeyjp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbffyj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rjgpzhhr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wrznpyjp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vwyeobgz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wobobqyn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gydewpus.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2faqznmhf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zwtchcmn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gihodfzv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zcugpbuu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2nmkejfpi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sxuavmrw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fusukmec.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gsgjiojj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2myxlfvvu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qysdohft.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2yyfxasoj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zonlgbjo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2slgnabjj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pnkmlilv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ksjqitrd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2timqazxs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rkrchalt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ygpzeuur.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uttblrrw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hzebstyg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qrutfdvn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vhlqqdgp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsjosxzy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qwnvasfc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2atzldpns.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2utvitfkp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pnohsioz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2elxelira.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pwbahcce.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aefkbqhl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2orycdkha.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2avukcewp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vfqxlpct.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qmjhpumw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2stabxwlz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2thgbzgfy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rknjcsfu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eehuazwp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2euetmrso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkvxdpkp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2opbkpkeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgiyxcdl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ksbtfhqi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2agoiwbqv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gjyvsvyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2llnqeubq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2necatnqi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rhrsarkz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gqfsxhvs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dawsumse.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nutokavm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rhqakwvj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fvnuiwdb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oautdfjs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xizrtqls.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fpzkaeay.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xvgfdnji.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sdsovwbn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bltlsesh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pfessudt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdoypsrj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dywezdrw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cbcxiclu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hnodllyp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kjynsqmo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xeewemey.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2whhctezz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2snithrdo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ncftzbmk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nudmykst.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uypgwjft.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgfjhhs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qneckktc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jrpvrtzh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhvuwz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hdafzdyq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eonftqls.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dogsrgwg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2pblypxih.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jfgohltt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2lsijkcwm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrcbvcr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gttlkrzj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rhdkdiue.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vbluyrmp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fqugthbx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jalhqamk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2stsizicb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vyosmohp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxcafdbm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ndpvphsh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tvdutrxa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wpyqlspo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sqfrggpc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2xpanvsiy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hucxinoi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xjnxxcma.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2parkwinl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gbicgoes.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tirhvsbm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2btpumvrv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tlgqedla.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hzlbjvif.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2itowfaix.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bcsenetv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ayfqrllo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hytailjp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rdhenjgc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xhqivnom.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2refxmhrz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2anmjulhu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qfagnvgj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jpougurd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vmwqmplv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rouisnxh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eogfkovz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2thyyaxae.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tumrquoz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wgsqtvam.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zkwkonmr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mhlmzanx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lanewaop.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lmlupwok.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2sxbjioxa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mlntghhk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bfhzvtab.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2liwvjsyw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hlwgtfaj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ipmpncqi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hhmaihcs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jbslnqgc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjpplczr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ycvniuay.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2iilemvuw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dmwuuvjz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wgdzhibw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xjskjkjc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jekjtdds.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztnkreze.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnviqjqh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcwzhcam.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2cfttdwlx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2abvtiocn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipqvslwc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cogqcfqr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ozpgysst.html


<!-- 参考信息 -->