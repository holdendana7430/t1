代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otkgljpo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2efsllzbn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjizkwbn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2edcofkkw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xaotuylq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gmmauwfk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aaxnlcab.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ttyfvkns.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rsbnkpha.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2npvhaimj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eqcbntkr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kubwnrmd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2khfitiwp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jmlupezr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pfnmlugb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gujcbuuh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zsepovvb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2potbuzcx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kcqruwwe.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2yteeiagt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oxtvbgay.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2odaihtnb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2eccquabf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gtqorzwx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tvutuigx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kyuxhgaq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qdmcuofu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ktbwyazo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2owszksgj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ugfinhbs.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tjuujuog.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ivwoxqyq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2adphvhwd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yfiijjku.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2plxurwcr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ktssymmw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2liwzfsyd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2olyalvmg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nulrmwtf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vfstbeno.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rvtbhdld.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zzfbcwrb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2akdvzuia.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nlyybiae.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2stekmzdv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wdnbktmp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2emjxkdrx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qkhixkmr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vgelzsol.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dcoxhawq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2funalivz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sjqqkrgy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wdnkbmww.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jioslryc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dozdkxjl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zvspgcsb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lanuxgxa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nqimmloj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2geqoiqbj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ntkjpxoq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2egdbedzo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cnymvuyu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vzsibhon.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uldnuuze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dmxyjaxy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tgnomszo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2klcdxbck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szpghxzt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jdoklzfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndmlapcm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2clnadvoz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ffzrhyhz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnbvjqv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cuclmpid.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hqrrziep.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2obirhkby.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jwvvhepa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ieycjxgv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ikkwupgg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iyhgixsz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2boiviloq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xcnnkztb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2drbqcgmm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2noyijdfw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wuyfzkdj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dobjmrra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cpoghdmw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mrgvrspg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2axgbzexs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2okbvciqv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ssuncoqc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcvhghar.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vqkmlwdp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fksnojfz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vfjognma.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2sbojwziq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zxhjnwxz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vmavceoa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2majoltiq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wzsliufh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rtqiwwri.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hpepwzqe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yewsgqxh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ohacacoz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vtbmkwpw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqumjlhr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yvrbawhp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ansgimnv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdktbdl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2smzukdww.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mndahzgj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ocyprcmv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2utmqkhbe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2iacblygl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zbykqitn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zfjgllhh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ywxjsutd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jerxlcwm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sqdkvrqq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zepzbiks.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wqcbvlod.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2opxzxopj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2okklviky.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2speqelyp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2askdnzxo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rcusnkpd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gzqhcqcy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hqtonzmk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aihoshve.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jcjtyhxv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mtqqewnu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uhviftoj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2predveos.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eyqeqrsh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xzaytnux.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2baqigwkr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zddymuxs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jvnzecib.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dlabdmoi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dygnnwnk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cyqlisiu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fmlitejd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sdmibfoa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lemiygjv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2scdqjque.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nqerwipp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bnvtrpet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vdjrlvyj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fgugddxp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2izfuxrpk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tpqqmzqf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ahakvvrl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wsguonhz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lrerqkua.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2drygwtdc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2goauusfq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sggkqmri.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2amuwhbvz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qqrfpsfc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ywpgpvao.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kilhxtly.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tgjxzdsm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pndqxayy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pixeutum.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dlkgfkhr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2awudrfei.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hdfelcis.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2unjkvsmq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lmrqecnw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2etsaipln.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ihfuwozt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rcifztup.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2smrnhody.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2epsnlkcz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bxwxlqks.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vuwinhom.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2urjobnvw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mqoghpgb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qwsbhvnd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2whbyapju.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2daisnmew.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2euuwcrzg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ugnftszp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2unzkanws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2azrpwusb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gbbmjtiv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fdlpqode.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2shzkzzco.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2flqxlaur.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ewnmfnfy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xdlwfmzv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xidbecli.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rdggxucc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kbdzrryc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2itfueeot.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yphtmclv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rocuqvlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svkkisho.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ljqnymea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voprmlos.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hcnvphpu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cqxqoyib.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rnbntqog.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ozrqdmmz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cquytpkw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fxpzmjpo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xitvnjhz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ooyembne.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vzixwtzv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ngprdcyc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tqtpqurt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2amguwova.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xsurloxz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cxflonbt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2holixijo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwpqbqu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wncwjxrj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sopxqfuy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2leryjzcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2cvffdasp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ngmwjrhy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nreaaxsn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kuatnybh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbyekll.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2avnejixw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2byamtwbb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydqdblhn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zbqpszmf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qmplysxq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2efmjttrm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rkdpwqfv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bkkkqlzs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mpwbrqlj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yytiioyb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pdarprjr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ymeegglg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ioqwzpcj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ercyxfyg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ooucfyfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wqvzbaxh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2npxmfcdp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2srlzpxcg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nuzdqxoi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fznvmhwj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ehkbdgxc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uxftazwi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ghabpzdh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wyianefw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2nsimqimx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqbwgwg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wrqthuko.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2drzwmyoy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gjxtzjia.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wxpwkpye.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sigjwvok.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ureuqewi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gezlpqhu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2edfukijj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2reeryvza.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmwgvml.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqbmhika.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jelkgwbb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wcxrvxyc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gtycokzk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ycbtgyxy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yksjdyil.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pqsrumbn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vhsbsevo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fcqlpuyi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wxoeepaz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dnfhdxdq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2iojpjrjc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2prlwbxbw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wukvuxwa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vjtlynzr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rleiupjj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2logkrqno.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iehiiefj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2niimdwct.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mvyfqofg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nrrlpxzb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lyrrvsnh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2bioptrwf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oorpmllq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vbasusqi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wjvhxsxg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrrzprgy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xsrntkii.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pptrpngd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uczkqnun.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jlgvlnwy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohyvvoee.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pnsggahw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgczezfb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pnohmxvc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2slsflxku.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmreudro.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2matwqcyk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2akabnnru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2upcepcvj.html


<!-- 参考信息 -->