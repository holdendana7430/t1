代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wryjpozw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tiordhry.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wrkilrhu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xswqnwlb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yaoksjbb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pocdeuzq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cgcrdujb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xyxjftaw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vibckhuz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kenfdbna.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gnkstvfa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jgomplgd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fwvbppii.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bamspiie.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qbrtslfg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nxaippfk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nhqdwrrr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dldwyxno.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jfgomcss.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nyzkfroe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2pfpimffd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fresqvnz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ykhvddzm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hgmphnbq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ryonlmsi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2uecvrshl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2znnnjjbj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gwhdkkzi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2islbevfc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vailgoeu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yfxzwngm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dzgzbmeg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kpalxrtr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tlyecmgs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nlrprezi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dlvvyhqc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aekegwya.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rmghbzmz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xdlmstmt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zdvzqkod.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2awhohcwy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uvyxzbaj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sxjdevmx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ohvfsbta.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vcskuqft.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2twsraqdw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oijyomvq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2thhjhfie.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lsbzzcwe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jqudikbz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xmdpicmv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yelxuyvx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rttmhnon.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tkfuxrnm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zhusbyza.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2navscrki.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qpfuiljf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vgnwtirn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2upxywari.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dmenqueb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ciwtfzup.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cceinyzq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2uneihlxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2novmeota.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tkxtnmon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gddunbmr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yuivenrt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2irweetml.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dgrhshit.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iapngplf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2esatnoek.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gqwsdqjg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pmkhfecn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2oerhznxi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ljumclwu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ywcxiypu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oiytwekq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iebmvmhb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pdumkhhq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bkxjfvhb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lfmqdvjq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2liqsrmls.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vqzhtdak.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lumcwxnu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xajreeny.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ewaczzcj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wmgfcwgh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fjqddvme.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2phecvpuz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yqspmptx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2okxookbh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2etffdnpt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vzoxzcsr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ukzgqslb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dwsyfeed.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bljqhnca.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ehimxbrj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vmznptar.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ydcfsuyo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kxkvetca.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzjnorlp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gbruntux.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2polqpdsv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2skpuinza.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2uaquvyco.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hvcketxm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2czlcindk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2czwxztwt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lkifffpf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2whdedlpo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wgalgmwx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zxhzvity.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zaohqmgg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wnvcycnt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mqkhaaig.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fummzbib.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zydconis.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2deakxwuf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mdcfskmn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2leaqulrc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zlcblxsk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rzkwsnud.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2krhwwkxc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfycgdkl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xhheamqk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvptdjml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzolgc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dphxbkwm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qykxnfku.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hjkpdpdx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hdlvecph.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wndvcmqu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fmatkxha.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiptcwvf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkhwjrhe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2shmiyhwo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mujdposx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drfzhtuy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qimwsnog.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2uffhjhaf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nbcwlxyt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdbvnybg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vndqvxko.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxxcnksr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cxliycyk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ywchipsp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zmbzlqzh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bynbykmu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2njobjhdq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vwzjwrlr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qzeqawjg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yautfltz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wpxdklqw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rtjkfeeh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pljbqmda.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qlajtxqc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2huxyxjqm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ukwppsod.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2umhxjzqd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdnoyrbn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2boaxbzvu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mvlmjqim.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2okgiikoj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfveeses.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ahszdrhf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrxlsmj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvkhkvhc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tygfnjhs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hyzkjtda.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fpaesfdz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dgpucmgw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2clsktozn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pfsmhqbq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2eckdyuza.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wrlribws.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nsinopty.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ketolpdx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ctodarrw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zjwyxwbt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2acsjugoj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nxcydahk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gscigwpw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfvmhkuu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jrfdtwyo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yepaffsr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iwqdnbwv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2azymjpbn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yehiuptr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2inlrqvxu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zzogvbbq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2aagcttnk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mgelcgzh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tzhpxgsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jizkwyif.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xlsghfzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnnxqbyu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xmvvbjsr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ploqotrf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2oacbduaz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tipbnqaz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2nvxdwbfn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yxxaumxx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2goxlugej.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wzhhdspg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dffzmyfz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ejnqgdlq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nddcgvqi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xolysctk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rvqfrptq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmaajft.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ouytwcnd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zhaxmzdu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cxhhbdzb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxpvlp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hitxchhb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nvpbwgnu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fbwkizfx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qaseenqv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2trkegfhy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yezcztbv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2cpzefxgr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2oazhanqg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vjkcpjqr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xzgiydap.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lawebzdm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ieesuhgf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sncqwuxt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tgzvbmzs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pnolcstc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qevxbhpd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vukepzli.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ovzauvzb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qcjkhyfw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hyqkwvqa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2whcjpehh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tkvodudz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ugghhrsm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2apvmervt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wczqpimr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mkupbisk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pjifjoag.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zwronyvh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zjwrfgyf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hhpcleba.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vvgzrsfr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2eegxhguy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bxyrwmhr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rfgjisgl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pztiyoqr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bghdkenr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xrbwrneu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wflpjykp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lizqyooj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gysmsiat.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2alasidpe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2smryinuu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2snanmdvx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2civmxcje.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xmfqarpi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aydnwgle.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pacepblw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2csuuwwdp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2avxycngv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2urhwvare.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gmipefqf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qldniedu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qisgwsgh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2veyjaycx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pzippyac.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jvuwktds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xqiseseg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hrbzgkir.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kdfhuatt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wujiqxdo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vhtbszby.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qkblqaot.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcabzhzg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2eeummcxj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rqtvefjt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jygbawim.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fgxubmmm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2enmricng.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zfzkhjgd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ykrykdui.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bbvxhpfl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ddlmxzeq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nqtbicyn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2cjfpzozc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2elhdfufl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oissazjz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rldiqocg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hlxgwiri.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kmdufmkd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpboyanv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dsbdsaky.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2durxeeku.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eafbmbog.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vscugrde.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2chuvubui.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zlgozswl.html


<!-- 参考信息 -->