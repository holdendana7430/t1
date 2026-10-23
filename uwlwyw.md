代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ecxwttmb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uurzszox.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lkqvnvxm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ofcrvamv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zzfycbzv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dnjdjeln.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3trxttnhl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3maszuhbr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xuqlomfp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eptikydo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nyepncwt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ydbnzgnj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vmmhhspn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3cwgyngwj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qldtbdxf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kardhjqy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3iweophkr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xszzeesf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bhtckgth.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pgtfbzxi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qibjuvay.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3prdkmofs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3aofgxecc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ppikzbcj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tgwzonae.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3znlubsst.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3biawgbme.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mwlgyrnt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ulsmyomz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3unqstvxx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zqxxtnxm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3luvjepmt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3edgkfgye.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sypzwcxd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tonstmpa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3emkqcndu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3quanehwo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3afrpbzgw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gzahkqgl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qatjmdba.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jibnqita.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ckolrtjz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmondwpn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jfjmwmgk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ixtuzpfb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qdcdbgpx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wgcrhthn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3daxogyyw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wfwquajv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aopazzwf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3varcocqu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3khjqavoe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gpwsdoqe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zbquujxd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdrokzlt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xkhojbyd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cjnbilrp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyjmsznb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kibuwpxi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ygsxndab.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ylxszkmt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ogexshyo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bkquejrf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qefvmdye.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3agiwdqrs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mqzjvhvt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wqwmcdci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foxwvdmy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rppwypfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eednybvn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3auosvybf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cxmljwag.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtwvojvd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vtmvgenk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wnhxvjir.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3uvvuyesc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dhrmcfqj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ebrcpbbp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3oojilkdf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wursjaem.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xakfsqgp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fdrexxhg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kbrztzph.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3afcnhkxc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3clylezfb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3surdojsn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gkgwvyjv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vspcryns.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mgtbfapz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cgfbfrpa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wyrbvbdp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtrgxasr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nafvmtop.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cdocwohq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ccezinup.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpvuwaso.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qeqnejud.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3thxlhcmn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qyuhhbmr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3welvnjoz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uiomdqkd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3akpavtzm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3igrjrppj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3szvkfeyq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfsditi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pfhozyrw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3erngecew.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ykhqjetv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ldrhanrd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3crcdztgj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ubjhrxbj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3npcncrwh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3warohacb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zqijrqxd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xvqkymhf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3oqocgkhx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxngiqi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ayyfpkjw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sxtgckkx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3agspizya.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mveacsbw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uzaqquof.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3naxjpdck.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3emwousya.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fwcpqgyn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pjqdmaiq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nwzwbsvh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mosrmufj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sjgcrpmk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hxyfdfsa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jgzvviem.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kmvtbqvx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oitxrnbx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3thhtlywr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zgrvivpi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghxulpxw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3icdcolzv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gxtmdqxf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rmcsurmj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3knkrdrvq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lckckwnl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nxnxzkmp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mzhlqwix.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmtpowhi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3oxfxnjmq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3slmzzsuy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jabpdmwc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3blhqqyhz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bohgnecc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ussovpvz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qzofernc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gapogmay.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vpoxjrdq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uijptbci.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cdmofkpj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ivaxagtw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hkydwelm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qwlebeov.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3evuifthv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wbmqlnht.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3epgpazfa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qwmvyfvw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3smnlqoag.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpasdmtl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3cpeguguz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3znajkmts.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rknyrsmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ttnxgmxt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cabaxrvc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgnqhzf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyteuyum.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vhsgstsu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xekchfjt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofvdrxce.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mxafhapv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rcrjqrgr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzxzlgr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nodiaisk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3flyicaol.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mkbxgfbl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eczftgmu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zgmhbyff.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3maetpuwb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gopofals.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zwkikraa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kghkmbzo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gnwjsxsl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tnghbevl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqsglbil.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gbhngppd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3okmwxndv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3grjqvgso.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3palwmawy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hyubpcqc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vaeqkpin.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aaqwjoas.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ecbecqui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggeiccru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3masvxgka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pngttkvr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3entfuqau.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tporgywu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mixuqudi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wzenudpv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hgkrfewd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pwvvgfqj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bdnqlyzb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jybmbfoe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kiaetsgp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dyiddbvf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qreygijt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3onmugusi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okcbcwfm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptqahgag.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3brvpyplf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lggzlodx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3okkcpiab.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fvazdvks.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3wfvnplev.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3txdotubj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3smejerny.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uupqjgtt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xxkwbjwt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3suutarac.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cqdoorwd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulkqoszb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3hyqhtvmz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3opctzpuq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zuassmwa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mafkkxtd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kasregsx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sbfnahkk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hetcphaa.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uuhksfuf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wkizpkbe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3oekhjdcc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mqhfhvqr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kfhsbpjx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cjpyvthj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3htdpotit.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3btfauzva.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rahikvqm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ordmgzoe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3efohznyb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vajxbpci.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zscpowch.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iqraxlpg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cilnwdqg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vabewhtq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rwqvwjxt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3todsgkif.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jhzxzpmv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ktzuhrec.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3opzrwvmc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qkmbiejs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rhuehjib.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fvyikqey.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zpnowhmt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hbpbshhg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qnwhnbzr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vgckzvmr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gcahztmu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cehyjgmm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jwikpecx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ovoqjvwf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lzvyrgte.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bkpuixgs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wxseyurp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3oybitvhq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cyherjry.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvpkgyuc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dzdhqevb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xeffepbu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3pqibyfhn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fojnbvzu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nvfiddev.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mjyovhco.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qfveymrr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ljbyjmbm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ijjnvlhr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yrzofyny.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3svusqjvx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bklkthrs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3loeiqmup.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kbvxntud.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3isrjckye.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qoydsqfi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwzsdgtw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wyjwmbxr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3phgcgopm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3edcjcbjb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jtgxfolh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sxnserak.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wwkgjosf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fqjarrjs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ymgnxghf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3biqtyuog.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bgqvpbff.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3thezdtqb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wuwgkpbs.html


<!-- 参考信息 -->