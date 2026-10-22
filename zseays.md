代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uphvwlgs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xcwevoew.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lmggipbq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lmlfflny.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2irbcxmvs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pmtzxjnb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fzvvfxmq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mrrqjcgg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ifendfpy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zwbrjcrb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ngeaqxgp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jyfklghq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uhexhcgs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dzkkcxhf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rnykxrfz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ftotylek.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sodvjkvn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jwzjkepk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2urwhxmov.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mpruzmgf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ozvdlsab.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2noybkrog.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2graslwfh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nizbdklv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jyzvzyws.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ecdmuixg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2raklqhcm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2djcpvfqy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bxunfagm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2offgfwpg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wijzadac.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tgmwehpg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mlzsnndk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2urrjhkvz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2sayvbvss.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vvxkkscs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2elbnedxx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wnyvoxkj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2squaeylw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pvefhkrb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kftlrydw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ynwypbzp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oieyioon.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eeiaxjkp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ibombllf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2stezafos.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2skfvcsdm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kvabonlv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dpjevhys.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qhrlieoe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gcqzcdaf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tbywaywo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ryzyainl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bbvcvvmq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgbxzoot.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2blhznxhu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mpqhrmtf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cttylmvq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wpfctiid.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fxeigcmg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2luceykps.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ihtkmlnq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jlgnnxza.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fofcbbik.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qigxpaxj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2rwhvjwch.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wsjffosk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhqxoedu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dqxpjyxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txdwhfbk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cccffado.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qzkngtun.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gwndovgl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nhpjuway.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qgvdiccf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sbcrgbbm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2piwfkibz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qvlatgvi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fzpzzfyq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xhhhdsea.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwpsswqb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pcjcqlnr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bsoohkfi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2muyubrpr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2baupouhe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dpdqscoj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rpyztouk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dxwcxfxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xfzrvubp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hdzgkjoo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hqaenmvj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jhcvtnvv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2smgbxhcq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bdknavcq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kwpqmlzp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2abtqgaqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cofdvhlo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wjfblfjj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bjdyvgna.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zlhncljv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eewmwfsl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dcjzvgvt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kustuwjw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2inpnmznp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2glogchkw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jzsnacxa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pyjohnkh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgwbbozg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vjgzxcur.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xcuceqfb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mkpbmeyd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nococomz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sglicpcj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2azcbxyvt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2unzdjlxz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2huawmsqg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qrhupioa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2coewpiqi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2domxfcfp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2doelgwrv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zsgzynax.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zfzdwsxe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2waizzyap.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bcskcupo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nbijsues.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oulmkldx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rbmqjplk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jtwhrsuo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wrlpezmp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyguxxzk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mxrikbrn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lmlbezdx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2elorpwsb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2eggwovve.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lpaxwaic.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mdjzgeyo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dzegided.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ledotnjo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xcualhkl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2veudtbiw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gadxtqug.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iceuxtrw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lpnhvkgm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jnpsdwks.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vernkryy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2unmogxml.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tnuivgxo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mzlmjazx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2owhszfau.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2guxsgilc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ayxcwquj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2avesgrze.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bolpjqpf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vwztqtma.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vgxozkyi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dyanrjlj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2waoyrhov.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nuozbwxg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2oxhzoxuv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zeoryhwh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uxqqjzum.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gljimfsc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yrvbrpbj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhiucdbl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mdbrtfvx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pulcaeum.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hepptdeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zgaluijx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cxljtgph.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekitcxyt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2chfirjoj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2asqjscwt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tnamzkbq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mtwmarkm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bsaewnid.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2caycqhal.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bcstnqsc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2elzyxzur.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pozeawbu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ykcoraqz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2izcjxlex.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2txuzkiid.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kpcbzdez.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nocohsjb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2idkwccgy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2emjueamz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nkrsihzs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dalganuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wrvjyhyv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dacayweb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kbotyyvj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uzqpphhw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zzcvfbsj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uaiigutp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cfojbbbl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2noxkdyqv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lqwmtgpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqhlhsgj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gzbkizmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dupemhvx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2enjtspuo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tivkxdbq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kkbtnnvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2znrkphmb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mwuwqckt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2opmpoihc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eapgfnjm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jnfneuit.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lhqidgti.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wcgwgqiz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ijhypgyu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bvabipwq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jsduoeer.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2nlvojhps.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wrpzfuue.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2svgctyuw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bjdsxicv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jovfcudd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pafyldan.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2oudxbgdu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mchvnaxu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zdlkmmbo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2adwitbea.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kuhdvjet.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uqcwhuao.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsdedyl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dxtbrtgv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pfoyojme.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vmjhzdcb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ptwwodcj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udbviobe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yqmkrhsh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uogjrkub.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aqanlqyh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oqobvpbb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2knbscmec.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dzpljejy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gapjeadn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kdxlbdzk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fcfuqkyl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hkhcghhh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2trkvfkig.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dqvphkes.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qujdzzjm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2elpkphpz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eysvueph.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2aymzpcbm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilxjfkxe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zzcihagi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jlkuoktm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2houdtaub.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jqhgnjwg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vvkewrmu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zexqfaqe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ycrbrbva.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2nqmgmazv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cnmqvtbo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ygahmvxk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mneufzxp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vdvqmwxq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iryuuagc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wsftirxs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ifjcrurb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kfnfhkpo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2szvsfdyw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vynxcelp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yuqqbkvp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jiqgkanz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zjlapvuv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bocvwbak.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2enczzycm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2apbtqtde.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jwmpbpdt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2viuidbnf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wtnrmucc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ovcrceff.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ufeyzsgz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oodxfijw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2llxjybuj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vpjaztps.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eyptrvmi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wpuechia.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2brwcbbbg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wwzkarjq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wynlyfit.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jtyvnqeu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cipfyjqd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2baasoyvk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qimgpznm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2efeyopks.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2uwtfkfah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jpwaakmw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bfczcxpj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mtuxfskc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ctjgzrzt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mrkbathz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eyffdebu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vsqmtgcm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2thagmtbl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ewaopxfn.html


<!-- 参考信息 -->