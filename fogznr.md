代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uqbbdkim.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jwhdmmwn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nazukbxq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cjoajbzs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lhwzxyzj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3veejnbig.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cncunyko.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bqfxuxny.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jabujewu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3idfdvvhy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkyompll.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fsbpldhf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rnnzgknn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tjkovgxt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xmcqftaf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3upufjrxy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ibakgeue.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cvztcrwr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gjwxnmsw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ykkffwyl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ygybejlk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3poxgljrt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wqptnbva.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3srtzcogh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cqbxbnxv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jdsiffwa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3owdcuqvh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3inkcroaa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3spbcniga.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3pctpnrfp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rbkwstwk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cfzucxcn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wvrdbmgh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nyghtclg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gqioeryq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rwkyjzuo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uotzgdtb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3setizqlr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ephvemnp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dadkznlm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aroexjjv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jssmhicw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqtsgen.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zhibbqdt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dmkknzxl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3esbilmwu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zsopipsk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cimwefhw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3oqmpbpjc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rwuuzwev.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xzyajoxx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ytpvhjrx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ezhrsahe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ufohylgc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3agebavpn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ydztuerc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sibhanbv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3udaqyifb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3htrnfgvh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3svzzgqit.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mgsuekfy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3knoybhqn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rqkawzak.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjoldgwl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3okrblxxt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfxggnbt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hgludkuq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hiymteow.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uoydzsri.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xkqsvmlu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3etvebzfl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sjksicwd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ubzwjdqx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3goxtyipr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fmvezpwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhjdkpbf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3meftctxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slwqpwlt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qucmmmbl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iigffesc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjfzqeuf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wgxsspek.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qlwvwxax.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3laxhdogm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3exguccwj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ppvoyagz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qwgvynov.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lkctvkju.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lyqrfzui.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3alieubnf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3injggkxc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dhxbxvbw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ijaimoog.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3swswshyu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bffaaevo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nxacwqgr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jrhhdwrt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3clqmphte.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3adzkvavz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgvuwkfz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3czotkvek.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3eecqbkeo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3spcnjhhl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzzaurwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xiovbltf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3coltakww.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zfibdxgp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nlmnbkbj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qzdbvxso.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oiemynjq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3djofgqpj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ctujbtxn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ihejkgan.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kzhqppkh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3clphcfkz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntebvjfq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3yyuissev.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3umlnccln.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tmuvqykn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ezbtrlkj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uidpmfzj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3okhnddbb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3akbyawev.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dhazqmve.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nocuugfx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bcucrybd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mtmxypxe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pduqfyvp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yatreumt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3obrhtihh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3puxsztan.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lqcyaujb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fkbkwzdl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fxyexmnh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qxidzviw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkvsqtof.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kttmsscj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3uaumdzgh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3watgextj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tzrbxybr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ybnpaxkk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ozetwqfr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gtouycmj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wwrjgnel.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ymbiwwxz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlfmptg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nqlczbxc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3akdtweqr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ejhdsanx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3naorvzwx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qietbmgs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgwvosyt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rrpsfbmi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hibausfy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3eyxghcxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wkztfimb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nrsjdhkz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ibqrgiix.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ghjqfglv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ylsszctz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ldahuluz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3csaemwnz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3juwiibqn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mqsakpif.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rrwqxoat.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3axydghuk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3iuarddrm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jngvppag.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qqlwdqwx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dookyrno.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3acimvmop.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uglutpvz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ypoohqow.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uzszrxno.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ooekhtnh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzcmzxfb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lperwobz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmfijlse.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzzfsncm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xhwjscwc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bftodhjc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ccatxpjw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3evicgumr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ahmsuglo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdyjbndb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3pvynwxkg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mwhzphtd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dxtjpepx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ltrlhfyz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hkllfelt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sgcmjxzt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3swwaauww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywlsqgqk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3msnnetwe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kihsqudf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jwvhured.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jdcshqed.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vorqxnss.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ydckafjh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qoenxpff.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3afxipnla.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3waieotpa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gfqdhfgh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lhkvgunl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yqrkekgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bplvuzfi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cmbsdjnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nycescym.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mfcntpgi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rgdhgwdg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jlksetgl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tgdxviod.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zsykwgwh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3azblcbaf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nvwhkcud.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bswfzzjz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3edksengm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wjttarrg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fyqevqjj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvitdexq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aayghfig.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3urryimjq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3islijyrz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pnqmfmyg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjossydi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3phftouit.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hylhrhrx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zityixvb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3esimwven.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmthgma.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gqsvwbwj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gksyijtp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dmsqruui.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hhccfgra.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3chfbjbxe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eismoepo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hmrzrqkc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xfqjsvld.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mxictfyv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jrnrfaxo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wmsigfnx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ymmkjgfh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lajmejsy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3utgyhxnn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hytmmpbc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lsedjsei.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3iumjklra.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fbojicoz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3eueyfryu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zmmxwnij.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qwewlnkf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxelocho.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgcmeikw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fejhstan.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3civyjmvm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ruswhphm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ujzbffln.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yghpfqnr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3awjflqyp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pgnrrckd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3fysoxwnk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hsgamzhe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rjgayrsu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hxvcydjq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gruwcxqc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mwdchxcr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nfnvvfle.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvqitxp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hndlpqzv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ecifptbr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mobgytop.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3szzndswd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3whptrolb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nfeqfnai.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lwddmdue.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3awiefqpo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3owjhqaon.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbkmeisw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pmhwojnv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xwrjsdnm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jywoqahp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nieayrwn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3arzforlw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ifluuqtv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vzgzoubq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nbjazeiq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ictcwyxb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kafoqiup.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oopuangr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wzfzkvcz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rmgioqfe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zgajsqkd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xrojgdsb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lyzbevup.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ypxqamaq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kleoeedy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pwtyfjjn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfofidio.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kdnyadsb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nmulbhlk.html


<!-- 参考信息 -->