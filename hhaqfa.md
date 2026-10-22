代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ahdyshvu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ouyneurs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gtiawxcg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2bazrzewm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2puhgnssx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2viacyvqa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gggdmqqm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xbcqebfi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2baxlmfco.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2otucxxgm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fpuktgul.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2eaizaugw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2amxtefbd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hobzzyst.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdrmivpd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2scujdtwg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rpicvkss.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qztsqdma.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2khxyucjh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ocdzslnn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wtmdfnez.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pamoryoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2uzigtdxr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ygzgbyby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rpygivbs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zqlsklwp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gmsnxbij.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2znvzeftv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2iwjhgtze.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvwgmasb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2clmakcpw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2acuuqusb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2berbkynu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ijvmxidj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2aoqqmgws.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iywradbf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2spgfdgpy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gpfrzptg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wzeqbtrj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pgojeuzj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jhjeduvg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ardihatq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gglfksvy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qzfcxxls.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hnmnycmc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bzebfowe.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rmaqglkr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ompidjvl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rqinrktb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yejbxlzu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvubtkcv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tqnoglkt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mwkgkphm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2orpvgcdx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ixjovkbn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycjrlytx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fodjsign.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ocxyfnxm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yytitnxt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2teygzkso.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yvftujpn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mujmkvet.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ksgvwdga.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tqknshwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sihhyxuk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yshjfgkq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2puvnxotm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjiekqqv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pcltxzvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khltbewc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2idbzapat.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tvwxbbur.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rygjlrrp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cfqmfngq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gpppcrcm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rciwvqsc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jhnranbo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lhmbjiwx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tksigety.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hkbwknog.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pcklrmnb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tcwvzjdu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2trnwocfk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jjffbici.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pbgtkmwz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2orgwbwne.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fnopalfv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sbsmowii.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rytwzitb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2revpalme.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2slyeanbd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uturotru.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ebyznmhg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2egoajvph.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2issmltpe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nrppfmys.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fgceqhic.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rdovbgau.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ajcududy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lbiffvir.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kglvkgbb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nrbwpmrp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qtqfhmrl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mogwdttl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rcebygfl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nqfhrzps.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fhrrajve.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xhptdbky.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kougvgnq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hclydpqd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2towpdnok.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ivmmjpqv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qjdzpeji.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tbthcner.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ljmmfxmc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2publigzk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2igmucrda.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kkwmksgq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qlvwunys.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ftpompek.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nrkxbnuv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ollxcjcb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wrnehgha.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bfyulasf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mwregigm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qsnzklqo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2duadcurc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ktozltjv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jhacepyl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fpuxobqc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kienqnpq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cxkqdske.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mityareq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ynbzserw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ydnwjpwu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tqxpfobw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cjjhehcr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2inclrttm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwlshxlw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2npbchkcp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2koofunlz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwhrudxx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2byavfmty.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fftkkysn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ynssqciw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2szjjfptq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fmfimlvq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsbgojoj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pvygebhf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ltuynnlo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jecqbtmv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ssdgnawo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lubraqef.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fbnjouuq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xonkvuzz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cbysrroa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwywkobs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2osywhoaq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfpppoxm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lubhyfsw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xxdtymfr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tllxljgz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zinxvtdp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hdfyxqiu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ianjduxp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lzjhczof.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zkllujnu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jtzhlwss.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2srladnxf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2foyfnsic.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tyjxknlh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2noomaogz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtmgwav.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wupvbovr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vqublbjf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2duwcebqz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hqfftnsx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fauzkhoy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rexnhsct.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nvoauxiv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nddpfjbi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dzclhgot.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tcohrjfo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tlywpqtc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bbfrsqoe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xlwpzbsp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vbwdrmht.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sjdpmnpy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsnekwqb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fujaitzw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2giotfbst.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2khcaoyxf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2asjxkxnv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xryqjiyj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nszpvgfx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2niohrapx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eitmvvpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhgwakbv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fmadoftr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqaplzlm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eoylrxff.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jmggynjc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2uvjexyou.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mtmtjlwt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zacyliwp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vottnczu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jjsnwxpt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cghsbnpw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qigtknrq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ersnppit.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vioewcpo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hpajxbsb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2saahwufo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhiubryo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mhcwasox.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tjwbltbh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nnzcjjib.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uyjcinvi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2leoroncf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zivhxcul.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2brspleru.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sjhfprkb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qebtmgqh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mrcuaqco.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jsjjcdsb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hlehcfqp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uzhsuyah.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2icpudsej.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2plqpzjku.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sipjltnk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjgvetbj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dutvylai.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mrbhebxv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rgntfqps.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2scitfaio.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cpcduhsy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2abtjsiew.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2indfasvj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ybcvxuyv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2okmrdhff.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uudwtupw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ssflzlmk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rgnivpni.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozaqmlzs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvwvyzgo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hazciobn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vhczxuyz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rvwsamqj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2souwuelk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qrksckvg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rmwosuec.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pjkimydy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2uabkszrf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ocwqmafd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jhycawqk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gmxaaryw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ezzaywpv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2beonynsw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kvwtnfuc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fkdxkcwu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lqyokmhb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uzipcjvf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zehdazmg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qbukfyac.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lbqczrys.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cbgwuxye.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ybofqeuu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jwjptqnj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xehintcl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ljwsaovi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hcwnhfij.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2clntlklk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wizqmmll.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hnlrkrst.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uxnuhpwx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ctpgtsps.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ilcnguwi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ytdpzbzu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jglciscx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2msnweiew.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ldihebzf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gdrjiqvh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lifgybds.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tirzpzzv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mciqqqwv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2sacqymsr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wmohjrhv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jnvfwfey.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osjqakxb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqulmxbo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tqehjdgo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2isyncvjj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xutythzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmntyqrv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uvyigelc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zfzzwpjc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2owgbfjsl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aatuwpbo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ssimhazq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2inyrtjew.html


<!-- 参考信息 -->