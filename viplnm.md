代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pcfhhhie.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3faveglwy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sczutqov.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xwizfoed.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ngvdecwk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3adgmtyti.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dwkhvzdc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3uotuqufb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ozstkont.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3txsevqmo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jbfwuffz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ujkkptqb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3novwxhmu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xwxxyprf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mlvsgtet.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fgifkdes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zwdokvtp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3grorrris.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cocebphm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pifyzrxz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ambpesgy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wujrfdkz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lctaovyz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xxkgfenc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hxrsxzzo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oypgfjlf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3koedfvuk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kqhayqof.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3knifuaue.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vpmxqnyj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xbksecgf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qpitndoz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kbfhbglm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pxldbwgf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ndjvbwgw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mzuqletv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3msbfpdzf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3etgwknxn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fmeyzlmj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kvovfzbm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3stlhgsrc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gjvvivvh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vbtcchoa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3efgmbxet.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vpvaoxkx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zjqhhkpn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ygagupql.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gjmaackk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yxeesjmt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3pfambude.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3onbcnfgi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ojkzlozt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ldzxlbva.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3luniiyuf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hkchbfoa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wbaarpwz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tfqbhwye.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uuxxkbqp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gsajgttr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3euimleao.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jbzoivsg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bezmbsjv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hklyoabs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nvudohac.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qsbwywnl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3brakiush.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xfydplqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqksaepo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3uplezhuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eaocdcsl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pluvgdan.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ivblrkeg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3prirqnfd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pegxqaoq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pziuuwaq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yopjteaf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vyxaefeg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3etbvwfbk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3dvebyult.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3msrtjfrx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntawpjwq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yxlsalpd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uqbfvhnu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3osjmvvfc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3njnvoptg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zuzwsftt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gwgwywej.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gsqknmpn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hdxzxhuf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tzojqxkl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rfnxtafg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tyirqkyt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vzlipdth.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aqbldjoa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vcmkwuxl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mxdpivdw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yyziyjrv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vvkkpoaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3afkxgmak.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xlscabcg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dmafybsc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oebojemi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3aetskrbo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ctopfsam.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vygaqgrb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wkhiybsg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jqdmtuhk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jaygrhyg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yaavkisp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xbtnzvmx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dgsiqhlv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3syhkunqn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zkjukrmj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ocaprqlx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tltndcuw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ftxfamwy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zooxeddp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ayhnmquw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3edekrdnk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbjvjs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cwmqvpvb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hrwvgkvb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kqyvfauj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ajnpqjnx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gutjrtau.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yuuzsptm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lincrzfu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3quqpwdwr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tsgbpewb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjefqwer.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3azuvgata.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3imdnbpmh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nxujftvv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eydkajct.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ovyzjrot.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uuhmutlp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fjlhmdsl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3thpfkhhg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrpgoqon.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vhyyjidw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jtizfejf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anoaomwv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pbwalzbi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ardwxfxb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cdqrcefz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ddyarpud.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qfpwdsou.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pooxnmkf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wlwmxrpy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xlwryowy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ivnslmiv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3glodtxhz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wfidcjbk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3otupfvrb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pafonjco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftapojef.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ojusstxr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eaowmrbp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hivpaetj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3guoqdvsn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bctexmqz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ewqrqrip.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pjqabwiq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3agawtorl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gwuiotqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fipsrlzh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vdxyuvtd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhotgfv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vhuxwary.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3aberucqy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zazziqyf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3iwfhemzz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jucjbybk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nxdekjpr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eczrkcmg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gmeeyrbg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3twblobuo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jlfkjfwh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uqbxrdch.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ejwaygtn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgihvtul.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dhcuqikf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ofkeefry.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pwcrulkl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ndakokdn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3efrxlxas.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfyimlxu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zdouvmfl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3azvmakgb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kjtymjhw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zwbmonvh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ggkvsxgc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bwpwietg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3novprrpn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hntawbis.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fvmyayrq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tqwgplix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuicdgrh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qjhlrsnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpzwftap.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qvehyrun.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iuwvcxre.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mdefdmtb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lybhjwjm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3piuqembw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rsdngwcx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vlpltuyd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qmcuxlvc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sgcetowr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jbdqzepn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3udmlpzon.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3unmlpqns.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3credltui.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3emdnssju.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sellpbzj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dnsjpuzr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3useqwqrs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jxppptxk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gszacbsj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rcmbggwu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3liinncnn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tkepnbiq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pmpboody.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lifnnuzh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hpjzzpdu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnlxfjwu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vpradzig.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rabzmglo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zvpbnaeo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sajhceba.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tpeqwqlz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zrwilbpt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pfdswrpl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fxyfymox.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rqbnyemt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pwwkzjzv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3apkerxwp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bgwxooeg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3htdjzgis.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3igatlwde.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qtkgdpjx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dmeekffc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ytenzyzj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3usuikavz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vgtjyjay.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cusxrfvg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eepwwvyc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ituwsnaa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3evrttvfp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nfnhmmzk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uxdsdyps.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rfuxsify.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nunnptqm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nkomupoo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bkxbvyor.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rqhqemid.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uezxxvfe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3splmnqcx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3iwcfecaq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ezyrlaha.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tohmoslq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3clkfnwhu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3iblmdiyl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xdjjifxc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dnkhlrou.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3eiozlcdc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3npxewbch.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3utmykmlh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fnijushk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ixqzdbhy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bwdcygpx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3taqhrwmg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dbcjmvjm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3uiosmewr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3eftzbght.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vxkmcqdq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3okifbrcj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yobeynim.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mmuloyiq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gcuzshkd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xspajwlf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zwpkvqfp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xfwuzpsa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ffngryda.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kctkimjj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lvpptvca.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yrbzwrnf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wknytldv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrygtuhk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rlodgajr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fyxihjib.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpuobcuf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3eozffoyd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dhtilvvp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3axophvtj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bdhzbfyv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3abatuyvl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nleegxoa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3epipcxgr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kzyxtsrp.html


<!-- 参考信息 -->