代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qhtgffcq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3enesabvg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uklitafz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vgkvvfii.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3azgqpyzk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mtttpakx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uducwezq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dqqzjhkh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bjattidl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ayqwjzvh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiqorrnh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3igjyerol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qgeqpaub.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3coboxgwz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yaneyygm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pwkktfin.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bsnlmlpl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3alkmbhyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3azxijtyc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kiitlrpk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lgjafkow.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wzmzsjcq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ycqkmhjg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pkvmljlj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3omdkddkn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pghiuhsi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wwjiiqrw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3prewriiy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ibgedieg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fbwpottd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zbampetb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ifzzzevq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3feovafsa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xjjarhjk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3couxzlcc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ajqcuuiy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ctajcgos.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xkmcrcre.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ssbmqdgy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ysyvbbse.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3awwzgxpf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lhliozbq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3whzpxogo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lunvapsg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3cjxnjofv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hrfwfvyc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hucbxsun.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oqvzkzle.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dysgjuzn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hzsuzicc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxcbzoha.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dpcrvyzc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ufirjlsg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wpoiyysx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vmkfwbwl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3csogxjkh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hmtsocyd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zboqoxpw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dazkhbst.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uxensnwc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hdarxcor.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cbvqcgcm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3urmzvkzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpwjmhcx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cmsixnuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqzadfgc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wtttkueh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vpqyymtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptmvvmah.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3luebhocb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bqkcnzti.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3sdbeidnl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wragltgd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rfasgabr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bpmdswaz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kgurmtzu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jyovmwbm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bkzongha.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zmknhvjv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ligrwuxo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dfimfinn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mwlmvfta.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kjcakzus.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xpxfmdbq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3viwgkppg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3sqwdubvn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3axpmatas.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiigzarg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uwknxoyk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cnysdhss.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3grivchhc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwcqzvwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mhmvmiow.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kcentcsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3utgraxpu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lbampodu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xcuhhpse.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jvgpkbfn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dgtkyqlb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3izbkmryv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ttbfxlzl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xvcxoaxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yyoboqlq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yxyvbxcz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nlmumkat.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xewtvtoy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3myztoqik.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mzuwpnyy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mdvtodpd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3aarzvmdp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3whaevdkd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wbjofmao.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ejemooix.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bskipwqt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjueue.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rueqxbql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hblzerzd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3haubajsq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xswtcmxr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iknoctaw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3henybfff.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3juwkrnky.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ewqxyval.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cmjaxfve.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dfkecnlb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dzzphyio.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qwmmjxss.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nxeqgrcr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vzlhmlkg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3efkwxied.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qrithrmc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qjxonmxt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ymfrhubj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ouqjgrhp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xmwmshly.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fsgjzfwn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vckzmgix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxuzyqk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kctkdyhs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yizupcwn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yxhdtnua.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qhcfflsu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ljgmyowd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkjaieah.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3liqzewec.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ncrypept.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ruxsnasq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ckbsytyj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ksgyfvxi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3iswexkvr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yfnuwuel.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cnilyqsp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoahxzdw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ldiwjtoy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcgxuvey.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jdijytrx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rrmwrkzg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3egfuzigw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tvxxjerb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbjggqb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fxujvrgi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xueoffgp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ibcneych.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3alznbhnv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gsutlllf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3whybuqcm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwuqvcwz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nxugzegf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3eflmbnqb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zlvufjdi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lbswgvdm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ncszgyla.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vsylbici.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jtqysuhj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lghennbx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vamurpri.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3awfzhymh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dlqafmjg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pgdflzfx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zxfgugpz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3djigijot.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vqgkobjl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rtdotmhe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mehkapij.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmvirrrp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fnfgbvhh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fiwsxagb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3duksydrg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fmxpcakw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3opmxfrwo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wbuszhlp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pytgzita.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3luwubnrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pceagiyl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ronrxjir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkoppjpo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zbmbboij.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xuvfnxws.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrnwfgmr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nrcrtjcy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kttqpqbs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3noqivcma.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kjauhfgf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3elbrnukx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xtnxjxpd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3oowzxdhw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bzwxrtec.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ryjsfurv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3foznlqen.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3iwnigvyo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xblgnrdj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3temuherf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3agfzulqv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qpajwnbq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ekzdiqih.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dyxqktfw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fweptvtb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vctexqgg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfgjmoct.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcvqkyai.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ygfclmdp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3sxsrxjuy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbvscxol.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3geuzdish.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gjvkdsgf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ybatmftz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lfqvmmqs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnwmwhbl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mdzoqmni.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xfpcgujn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vofcmuqi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cyjwrtly.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cheizonl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lialbpja.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ecztnmrt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nnyhaour.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yxpcpeni.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mzirwnqo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mwpjctxn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ynjwrfor.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fostlmig.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3moijlxoc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3svoabpnm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbhxvqn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qvztarpz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3iakmyzme.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3glstagzu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3detcbjqp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mygispwt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3feqlfmwc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fryhxebx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3lqvrnkme.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vnnqubwh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dhatbfvm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vqegqdnj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3uzhirwgx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3durvijyd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kfizppmu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3scsflnaq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3efooryze.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qlrepnzu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ifpsarex.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ufkojiou.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vgywkbkh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zyzvloic.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ayncpsdw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3dywoynni.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3goggtxrg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3grivavzj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3susnijdj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3iijpkhco.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lbypyfcv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nosmygwk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vomkgnyq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dnenezpk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3frcgance.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gymhahhx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ejmtbhmq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uerxpthw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mnqczkeb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rgvywild.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pzbzggmm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxbwjnhj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zxwswatt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nxjzlsex.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zbmrzsgu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fwrgipqr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxribkn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nukmthkv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eayjuwcn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3auurvldo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rqwbnipu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xojryqxm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aruahujk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptlwegvb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3icxkqmfy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3czjvskqp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lbrmbnio.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qeyjywnq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3afzdlixi.html


<!-- 参考信息 -->