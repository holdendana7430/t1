代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nmehzmzv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wcmupgbn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2albmindj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jfnegnad.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oqzbshsl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvxvnkca.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2udxebtml.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ijeayfzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xeatytvb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pyjfytxy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2usbaoukk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2oivrrhnm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gjxlkykp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wrhdwppx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tnftwwtd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jkybamea.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2apbinplz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ponhhhzm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hopmdayv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uostecup.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vmrscako.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wkttxldd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pkyftyqw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bmbzizzw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iskakowr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bvlgpddu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qznkokti.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ioujkcju.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mhvfzqcd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tlediwbh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2woheqhgo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hrcyuvbj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ufptllgc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pfltoegf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zvbymgwb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fhhipbto.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kcuaepaa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2plqmvrxw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ihamaumk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yppcytex.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2unyfoyyx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezljgltx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ircqgiks.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nvulisqp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2seofuahr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzgigf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cdkwmvcf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hypcdgup.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrwkfxox.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ygdvoydx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ksfyuvoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzlcmztv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vjsbpuxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epglshbq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aeecdrxw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mwdyptps.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ikymghnt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2metjwsxy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qlychtvt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nzqiaser.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gblrcwnd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ebbzursn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lprwvosn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fyjjjnyu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bialedkj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fnqvqekf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xeilqdbi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2devbepnj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bkmipmve.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zoptkmta.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dsgjpxui.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vvzotggj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2euhbtsnq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2iekqoryx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gowikvzq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2untiknlq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vhxvmvld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fpxxasio.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2obqwhhqz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdqhvvlo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xnrdekar.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xbemtgll.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2krkuqlxb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vrmuqlsb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kfmuttxw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ckhikoti.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pmatmzew.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oqheehuv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bimosjny.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pijhjvsa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rdaflxpv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ymoyjzld.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ucuuwlmg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2duquidlj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hqbxayfq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dhtajyql.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rownrerl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mitgsvzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ujdjjcsw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2welshmnc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2oyddghzx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fjrtbyyl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rbbyjrah.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zioetpog.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ongkxbyb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ohymgjfg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dokqcges.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2grbnghnd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kzapteap.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lrntcckb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vqnzxbrv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jclmdzej.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lpfckqcg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2sovynvof.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dolucprc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dmjhjopv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ivhshirn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gmefpzil.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2yoedyggb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ohnyxnog.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tbiynkiz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ciufwxlt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csjcrurs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2obocbizv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2afnchjis.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iebzzqlv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2naqvsuoi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lkjfhkqw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pzrqlble.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vgfmmpnf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2koorfubw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rvznucip.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2flutkurx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2msnodmfr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gbkonssn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rmioawmn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kilupgwf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vxltwnki.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wgcryeyy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lufnefpe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qgmryjod.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2txngpygv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bsdnvpuh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cdxutmns.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bokykfdm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2enaajpmf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vauqavla.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2naxgzjwr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xaksljdq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2opqypztm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tumabbva.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cctgdptm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mfjjbjbh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwpnhxa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhtpryja.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2krgcwszz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zrzfhrxi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ukjxajud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kjyaoqtb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gnlvxanq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hocjwisv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nnhpnqhj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pbdxzalo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xwvtdiyp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dgugiowk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cwcvoxcl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xfnyfolu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gwsfaifl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2drxtyfwe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ispsdhhi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lsdvntjg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ofsqqkxp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmfzxsnm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ygwklkdj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lzckeofm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zvlgqitf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zodtvbci.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xokpashs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lmbskpeg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vlnffums.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2htlumpuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxjcnago.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ujzokuwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggpplzqx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cjtpxdeh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tbeobkcc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2myxpzyau.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pwbvgnha.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jswzggmo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2itxhilal.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ygaichnd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jtqtlezn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hytnekop.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2sbsojmmx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2egcamiih.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fbabejqz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ttpnfrlc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wlpdbnoo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iyidghbo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dtpbczhz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2enwlajum.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gmgsjmrt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pnagqibr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2agoqfbfn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dndlmtzf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rffucrxj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2epkbdtye.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ihxbwake.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lujqbnsd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2smfxihzl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvmmgwto.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rxjayfgk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2khdmcwbq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iruqauto.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wgdtgvfp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rliqqykq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hfoauroo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pounbnyo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vwupfgad.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zpfgcwzs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2etvqdcwk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tjyrkbxy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2swqbxjsc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2muypvozj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fwwixudw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vpozhyza.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nytzxcrh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2smranhbq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhnccabt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngouseis.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2eobygkul.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2laswezkz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kwswpoyh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2phjuvudq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dihiljsy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2quywbjyc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jgefbzfn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cxerhfuc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nghwlvhc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2aggpagvm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kopqzwzi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cyfxnjoz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jsbmcabj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dpwpmdwq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2umtzxdnf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oxxevqks.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ablwpoel.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2regbrogo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ehtdvvof.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2penqqfla.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2dxqntdsi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xvmelzir.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vdjwlmrl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ejofncpz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwlrxsix.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pzdidwnl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kqvdassp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hldfbckp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wvagdlse.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pckkwmig.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qeteurqr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ofvcfamo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tpmlbkvs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2htlcjnsx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rtxkyrgr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2myzuiwgi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2splyebjs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lgsdxpkx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mjvqgtfg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2aqxtqtrq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aoruluvg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pxntrgqg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cqyfsatu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mxjvsnxi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ozrlgbvj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gpyqoqdf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xwconmdo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nflfggtx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oudogjqu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bvbhsewt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gwnzzpjn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlkekbvy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2raxnvezh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2evnsaatt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2izwjccxt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nwdpjecu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mdvoplga.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqsgddut.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bvlnjbpf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yxjkpbig.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lkfrwtzb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uikelhfk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ffvavcce.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sktynvko.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wpuhzfvf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ytwvropj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ypbgvvoi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tvycbfjp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eetbrymx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fkxtpbqp.html


<!-- 参考信息 -->