代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bnzfevwi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rtzmxwum.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qtbvjzui.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ilbsohas.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ckuheukm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2oaialqkd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2puwukfdy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2naqtauqm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2weusrruk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ehxjvyrr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hlaqpyek.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2idtrqmll.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2crwilcdc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2thvzzilv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2inbntuqz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dnwkohha.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kkjpukro.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2njaagjrp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dzmatqzx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uwddjveo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ezxawpmc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xqphzntj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2atigcdoe.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gcqhpqzq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fldwkgap.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zbhunled.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2khjtqman.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ekzekiml.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2covztnmm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipdsxznh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2djfehuri.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nukjsqox.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2efhjmyte.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ozkxfbkv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2osthkviz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ollmctxl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vgnavpvk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hiuakgcg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jazgiudi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2okhepagh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nwpluaqj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2akkyczhc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jthrihwb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sxuemoge.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2behcemym.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tpsuugec.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hynjkhrt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jhktshow.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2maoxyiwb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xpqqnmrh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2magscbez.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2cnkxrqun.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oauujygc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zgvhuqlu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zyvxzehn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gfhvmeen.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mabkexin.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mmfnvcdm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pnpecccx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pfacmmew.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2otveofjc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2erarjnxq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nnaiphek.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nijuzhti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2upkpcdkv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vtwumedi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xqjaoskb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slbihcbu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yycfuzll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rryhuzev.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vfckpsyd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zrperzqn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmpmckyw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2iwpjtxum.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cncatqpm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oqdckvsh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ksmyfetv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wkzsgtzq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xgrmzklo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nbohppbt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2teifekza.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uqamdspm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hmygljgi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pryiaayn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cnqacyhf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ygxtlcfg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lhrozlwu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2utqzvkhd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ldkegeig.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kggaeukn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vwosaais.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2espgqiyb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ohyhpztw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cdxvadxy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pybmxvkr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gjcdawyp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lxxoiqcu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wzouppjn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gwqyjhue.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hsekqcbd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zxnrjzxp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wipbqbyg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fnuxrwvs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mbjpakjw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2akcblbae.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tyecgltq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2moqutebu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cpnsqoqi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xuhmbnpz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2luzyadgz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jplphzvy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ebxpvdrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2spnlktdy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2oeciphma.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yohndxlp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lpbqndwq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2npljtxlj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tkqrexko.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kbgcvcgt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kokhosew.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kimbsdkx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kxdertzb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vomtndza.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ffmtnjuw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xwantnis.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yvdpmtnq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yrnhjhhh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vikfbfqa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qwtheynn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mfgpbnsh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fvffxmee.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hesjbvuy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fkmfrmje.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tewkkjxe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2estwdtmg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ubxoibpe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gpphypyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohvrwapz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flxlindd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2awkhimsb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jsmusojd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pdxcazbk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fimyzbsx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssexezfd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nwghpmsj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2otrncbsv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2iheahkgk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnattkgl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dfnoumik.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iidxaglm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zokusqwb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ldxwpmwf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xbovkiuf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qoclwjot.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cxetkbuw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iesyrlmv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhdywjdn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2glabbewh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2btdnnnwk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2unossnjc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2yqwmyxgm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gpfpollf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2aexlaxcg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2juysalge.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2uhlhlpvq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2epzkpmgq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nhjumaub.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fniwqluf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ydkdfexh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gofqfhmj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hqaryzys.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lbbdmctl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfobqns.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkrakluw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xqhvxqxw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2awpmncjp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2obzobzpb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2toqpbljd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2khwejiny.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wykcfftb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfiwuegl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rnopteef.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wwualygy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xloiamuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2eknfftdx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2udsejuez.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wiuocsqo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tycdjecu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhurhmgi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rljzytmo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wdiwljql.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wngmmagi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tzkbrfhm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hmdxmogx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lxzefmgg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2muyiifft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kmvxuztn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbfpybmb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sewuaukp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bczpfrmx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yhkshxzf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pgozopyl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ehmjgnga.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nftzagzd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ilgqvysa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cwduxkoc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vvogefze.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptsrzasb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kmxwuzdu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zszfuckf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ujuhxhbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fewkksra.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fcnpmxmx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ipfncdrj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nziwxpip.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qroykzwj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wociucgu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ergupdfj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvnzbtso.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ugnslrpn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nkcgbzwf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2muhcqqid.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wtkfgdgp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykfkkhdf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zqvmmonk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzaxfsnm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2scuvdmdb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nokcnley.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2iammpwki.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tkeufxsk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpbuasph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wcmgptgc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wsnijtvw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lojojnwu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vzkihteh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2edbxnmok.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qpdlrvri.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qnymsmcf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fbtugyln.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zphiwvzi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2olbdaivf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jicveyvj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xhmopkdy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdeiwwpw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kgknxwsv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2efrgyazh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zpzskequ.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdexerxm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kvogvgoe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmudlfz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gjogickx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2byvathrk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lfglzaqj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mfufimrv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dqdjeqhl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2icxdjszu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2uumyefup.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nvipmonn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nsumefcd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qdtfajcf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fzyibfvy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kuvuzwtz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ifsqqobi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vsbhyadg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2chulqhky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wbvtbbri.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yirnkoid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wnjykksk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2sqdmfzeh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rlojhaxn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2awxdqucu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ombaomvp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oxrwflub.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2arqbvdid.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kkfsudml.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fjjfvpjg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2llsuvyee.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rznwafpt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ljnsymix.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2efyirewu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvieav.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lfgdqped.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2drnpfpjn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wgsmkfhz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wqbashfu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2axnvhqxi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qcdqdmge.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yinyursr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntdgoowy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvmbuacu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wbesyynw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2elfzbufa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nykfcvbg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wzpmvduq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lftsdktv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pqyhylae.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdtuktsd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dofzlqvs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lghmdaqe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uugneevy.html


<!-- 参考信息 -->