代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qcnrtdcn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wtrkoujo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cmpqnwlw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qpxvptva.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iziwjczx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqrwdzdd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aepacwiv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2esacczxx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iqbmdage.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2claacrzf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dajktroe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2odpchqmt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2neprczeb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzhmjxjz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bxsskjik.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lgjfzklo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2spvapyvs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dacrflnc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wobjmzzo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gkhjjkbx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lzuiweqh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nuxnnilm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2npoaqtsi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hgltbhrh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cttugmqy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ztvpaorv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2iepyzejo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nlrbfhkx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ruhrgevo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2glumxedl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ipfrnwjd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vskzheml.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gzfluqym.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2epzylius.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ghpgizln.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bmlxogid.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bnbhkije.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2elhebicd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fatcvwcs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2togqfpww.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wxpzzuia.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2scwlymck.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkjrwunm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mcxoxsbg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2olhgrowk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nnlutcgp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ieykkpyl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2safqyvfy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dndlpjzs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2afbjlfzh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nywandra.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2toletynz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gdkwwkzr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kbevgatt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xhvyfuso.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ebtzrtxu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2gykawybx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2iwknrbip.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zpouytue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwuqmkgh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pplbwpzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqjjvfuu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tynjakwp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rnnjlipb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvntqfuj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2plszdytk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rvsgmnbr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fgmhwjoi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hiemfgbu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hmpqmvex.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oudatgoh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lsrkrboj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rsbnlwyn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xbpuewax.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2odcrupod.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rkrywxdz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lcbqlsbm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bgzpsaqv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qstnhknt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nikpbthi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eitxmswc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ymutbklh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hzijfeef.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qziafvuo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jfixlyzv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jbfvcbkg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qryegkpk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rssslwyn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lvppdiux.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2btuxafrd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pvnbrzyr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2divhhkue.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mfswwxxc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqrwrfgg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cvksmweo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nbwoodiq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2unzrvigg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dfhmxrpy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qaddsbse.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2phiwaidx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xizvrqec.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2pdbmliqj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aascmdkz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2durjxmjw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ttlmwbdz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xlonjupa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jzgmvzkv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tprwgkae.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eiessjqy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rbijimbr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bgrhkccf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tourksgu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dauwnfms.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wxxufltx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wgucwbdw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gjxyehjh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dzydtuvd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2iunjsyil.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ehwzqedg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rlbteqia.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jtzkduzz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qstxekcb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mpscktkc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kaqzjuvz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gpxgqrau.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cmxgfilm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zimtpwhm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2brjmsrbr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lquulzbz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrqymwr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfswpenm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uszjbiic.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vcokutyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ldjxyzvb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2soobedit.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tywkaret.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vpxctmyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2avjuyefr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cbspoxli.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2occcyocb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kwnyktrz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqmjsbm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2odaznflx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vcsujbkl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lgobnatd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2arxgbjqa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gtqmydct.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yadcmmgb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rocbdbbg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2aghlofof.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmgkgday.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fjqoxgab.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tnphkqib.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2weeemelf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pduufpdt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qivgprva.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dtbogtrq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fbcvzgzq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qqbbjqzz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pdpbihle.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zlqjznbt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gkzeuewn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xzyvwxfj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lbpaknng.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2akkjxyte.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eskexsnk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2guypxvhe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ckkkjvte.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vfyexldm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nsxspfgu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nqdfheeo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dgfypoqs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2isztqmek.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wbqgiwpx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cvnuzdzp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2awtfefjk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lrlqqzne.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tpzctanj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ykashfdw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2peytfuew.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdomcead.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wczknwpj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dsssqmcm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ylzlnmsl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eceqdjbr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wshnyvaq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oxabiise.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2afstewcx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wvebcmhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smxajltl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wybalxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihuqxdgx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ylyglkjp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mxsccbco.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ttdbrrtz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2shyptdnv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wgynhkav.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dkmnjvmr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nsmxciqs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2hdokcpun.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2khtosbjg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rsnvvziw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rxnewobz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jfelmbju.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mhktyycy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2npanqtac.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zcgusalp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ezxkvzeu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lflkrndc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rqsezwpi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kwqstydk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2shqrzpxe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2esovmqdg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ykdsjyim.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rspnmdof.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqmqdcq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uvehefne.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yputbpzm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2udovdhmd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rzrappwn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2klxjfefd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wejxucbc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lniqytry.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2auylgqhr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rppwfmxi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jctzyzql.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rdsxvoli.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cjkqfkbo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jzkzeonq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdyqbavt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2sypguuef.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gmzvthhe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcnwatyq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zrhyskui.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wlfpxauc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rhpdfsig.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pfykcjbv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cykkkgin.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2betgkxlk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qmflurtb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jnghyxsj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2klwzwphf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rqjaldhv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qkunhwbg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2flhdrtuh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zleaxapt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cxdeylgk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lqltbroh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2adoqrtms.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xadicwob.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fietktjp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yladejux.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2beoznkhb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xswawugc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jnjooeuj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kmyorkug.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wbyclnmx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rhvyqjin.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rlymojil.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dijqrzwi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2keiknspf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpemshgq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2esxhcvnz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rjcuqyuy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hkfyzzjo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2srwmbnfo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jzjglbpd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gtimqddl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yoqwbmth.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2jfnbkbjz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bhfqxtxw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qigsqsxi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbiqlwkm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zutxurfy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2krsnozwe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovnalkvm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rqygegdr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yflhysox.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sihbsqpf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nnjpvncz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oulyjaec.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jfqcfqvv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mlsnxcrk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bfyxrhbg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rvvoclwk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyeqcqbc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fvcwkgin.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vipdohuz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjkvcyrg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rtbxgfvv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gtgazysd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2omktlclx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwrammen.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eddvugrv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oxjsnfkc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qickrljn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cfwdzqna.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uniljaqq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uetgyafn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fbvndiwa.html


<!-- 参考信息 -->