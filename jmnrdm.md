代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvhxagvu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lvujeuvj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yhjnzkvt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zrixiilx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2agqcssrj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dxxahvhm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jlvxierp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hivstfoo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yhjbpykx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tjsoigbu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dbqgsetz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rhwojbqv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ovaendws.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtfolnmz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tlqqaxjx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vrmsgjjr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zdobhlxq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cmlqcnwo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2orqyhncb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gejdaohj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sloxcfov.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gdpajelm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zbtxflgn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fzdzblqi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2coubpuju.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mwalgefz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ldzbjbxi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iyqcqjod.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2chqtaoxx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nbgxzhrd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mrxztwwy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2finfjykg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nzogiang.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bnbutatz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlryprz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oatqmyqw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2krhduzqx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xjofcthl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2czmwijxg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hqyzlvot.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mwdxychn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xgncopzr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkzfupan.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ntcxegny.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2roviyllh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kwurdphm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ipijmpfe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dksvirfk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cwznkalt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sntjaanw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vlffcrqp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2enwjjhsk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2efcktute.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2scwvmsvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oubvline.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2odxvqxvc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jnkfuypc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmaajyws.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dlgrbzyz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2whpiwvlc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rsbqolyy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2teaevpkh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vmpftyna.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2eovxdpgp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dlrmtpui.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qnyshvpb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kfabkzsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuojcera.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pnclxboa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqxkcezn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhaytnar.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2eijdizzk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zafyattm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dabllgni.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hzwdtlvo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sqdqfjme.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bepjxkvz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hxcsiegy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uvpoegkb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iwxaulsm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2miswwgbc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gglcdpmg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bknmlgjb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vjfbwbch.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2idowuekw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ktfhjpez.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ibwpxmij.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xrpietbh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qjyqwtms.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jukjqkje.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pqbhpudd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2phkxzrhw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kqrgxrfx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rdsndhad.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uzsvnpmw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqxvhaes.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mjrwtsgu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yslncesy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2togrammo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yvmohrhe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2flgegjas.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ncbsopyo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vjcauose.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2aouojcxf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dzyqfots.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2roilfttx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ndewypxn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xnnnomyg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wjmsnlah.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2duhkahbx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ymlsvvma.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ouhuwfwf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ucpqipux.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2prepsivn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vlazlvrh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tudlvfsr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbncuwb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2siedegxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zodepgsv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mdibkgjw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pnvqlunq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2clbtwssw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tzpckeor.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xdzookgs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2visilblr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vporvlbh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qgpiuxxk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tuuxtdyz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hkbhgfnh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kwqhceic.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wjstomfd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ozkodpqp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dskkfhmu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zbovltbd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pzxzzflh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fagkviyt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dkhgdflo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjaoddb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2euvqittp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dogcbihi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nbpybojm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bkbbckve.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vjjmrjjf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pjhghofx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2atfcpbzs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sbeqfzsv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rqokrgya.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cjgdqxti.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2oxoclbla.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2guvotjoj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2geqmpwbi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kszntdry.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2avinxhsa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yusldwgp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xozpqkmr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jeljxhvm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wdnmwczh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ixkfzrsb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzxhyqno.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gucbyaqs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fmawiqgl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bzyulfsp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ptnzcons.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2cgyhaljm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zsyqiqfc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mvrjqkgx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qamyehsx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhpbrqh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2epodevyi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ikzvjnih.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nvyacstv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nlpnkmwp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dotjolfi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2iglzirlj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ocbthquc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cjnlmzbu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fcioized.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwbozash.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2irpodhdt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wxctpkoo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uufirrjz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qjkisxxj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gmlxirre.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dzolvrss.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2msptwbxh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wvcipvji.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rcrpdsbf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xpuhlmjq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gagdktrc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2amnomenr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2oodimkjz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lipdihed.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yemmllrl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rhmpwmuv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ymifqfhs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ylrucenk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gwjhfbot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olnlrhzz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hmzerfqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohswxtsp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfehhflh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2loqfojjk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfhbbmkc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2enyrzext.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mrhnhaux.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nkefeplp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dcidxljg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzaatsti.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fuhmhjgc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dguhnavc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qvymefzb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2shgucqfr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qsuritlg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uxtsrjea.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qnbdjguh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgzicdr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kudaqrer.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yjmpmumm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hrqljjnx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kbdkucsi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yeorxeor.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2oyyfybeg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hprmssvz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tbwbqbmb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hbabyzza.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zgtlxxjk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhotkxjh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cegrsbwl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ntgtqrme.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kranviog.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2acmelafs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lwemagcc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yxwxsfcp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ircqibbh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hnzbmapr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zzumopsh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xkrfyqbq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gwhybsmt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2srmzszhd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2isiosrdm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yrzbddxy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2givmuhwt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yvabgpst.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bshybvew.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ufocipkc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2oibsyfcl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jokliamc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbtqeso.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pvkcivnd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fmsgerww.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mtjigcxv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2smdrduhg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lecyndex.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgkyuord.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bjeubqkf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qjjaccik.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lrhpwerc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eqaclccu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jqhcdntf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qdgylvdz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oxmpvnyb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mqjecmeq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nolsyuzm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gnybvygl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tgfbcerz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wadbprlv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ooldaabf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ceqiqumq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qbzawpfx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yttgabnk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iphunbbt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oheyqlzv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2btteuvqx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2aghttuio.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hlnjpati.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vrlkfcwz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tzvgkved.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2updpzbep.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lyooastw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cwvucxpm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2stgrzojb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hjfbbxxv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ojilfzdu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2inrpyypb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vmgxuyzc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zocjchqn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cylegxsk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hnzdzcom.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kraegfjr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxheqxi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qthyvbjh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2omdqytwd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2csvqkcev.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2osadfjvt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uupmvxrm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ywcmhstp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qshoblyy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iligvdrm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mnnebarr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jbdecrdw.html


<!-- 参考信息 -->