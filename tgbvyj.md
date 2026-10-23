代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3egidsbth.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zcobdilz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oavnouiv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qbvreqjn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3eksicoze.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fkmwzgnb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iopmjbcf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gfdwjcpe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dqbyopuq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gxtmvtsl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mhogbpfy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pwhnlhcm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tegcnfvg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewgnszxf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tfvigmqv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ktfbwcuy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pgoorruz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gvvcytac.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mgqumrqh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ibljbmbn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wfhmvprl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhjchown.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3buduocne.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pyczqlmi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qrhrvewl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hilalepx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tfaqmgzc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qvfqzivt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ydinppxk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzuqkzgr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3flyjadfv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3owljjxpu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ourdkdym.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ezvbssoz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tqzuural.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gxcfctgj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3evpzuvmf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wnftxdrm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dnpbyild.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bcxdnoeo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jprvsvmh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3armdkwic.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iohtuozr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bzomjczy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ysifyera.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hnaclmqx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jpfpwlno.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oumoejtc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3klkunqmc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jowlnwwa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3efvtijoe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yyxngovw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bxckopgr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gtmlocqj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wopnphxj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fmyacwjm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pufrzbin.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3muaqqyfa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cfuxfzlz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xfztodul.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qwjolbaa.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zsrfhqtg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwitipze.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ymsrjzpk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qyzrpsda.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hzcqhksb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fxwgwffo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udyrtotc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ouaskvck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ounwhoss.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdtkmnqv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3awphnhxy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3chaxlucy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ekbyptmc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qreqdrjn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nldzgtib.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3iysonxum.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yoemslyl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tzgpqlzj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fvzrrviw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vadlfqag.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3psgtlhee.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sbobkpcw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ttvhcjvt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iuynfutd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wxmvcmyl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ixwtnamt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3fznirtyp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fycjpetl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3aonhquci.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dywnkhns.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fchyyhbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3sxggmcnl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbyveoi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tzsnyilz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3itkdfynf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3umgvqkhx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qaceyapr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vwkptijn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hlyushex.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rfprtlpl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hwvdnmzl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dcpdpgzg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zosjydke.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3esyuaezk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hthxeojx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pmgdmvgh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vubkhzvg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ayydkaxa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vjtxcbkj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3teykykaz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kmayeiuq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dmsghjvf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wxdgmfes.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pfcfnigp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hjhapuaf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oatquhxj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gguulzwy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3leqzaiic.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nzeamsyw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3lwsxtlwj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3weavnmoo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3thuozznc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3myntisdo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3votqiizd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fndfdxzm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hdlmehnx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlaihabh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hhaorcub.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pthhburp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gknxskqr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wbmfbfox.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zqmibkne.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ahhhmerk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jxptkzrs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3igslfiga.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ukxwlksb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivvvsjpn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3meiybjgl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qqnpnvop.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hyuokecg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kszxdvbp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wwhqmshr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxycpgps.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ggvlxtki.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ouaixnry.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oxfdgyrl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kgwzkwgk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3aqjksomv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uafbohit.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nrdshxes.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3khbvpzhr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sxtonibe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xaxrtkll.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cwkyjkyf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vmikgpus.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbtbgpys.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vzmvtfnh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oarzdgwh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nvfatden.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ysftwjur.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wgbaoluc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3thqmbuxi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnfkrrqc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xfojahzl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qiyovehi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yentbyce.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mezpwlwz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fjtbincv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dmdjrcml.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3didjfusy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3sqqvddxq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nxrixhmx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzjdcqbg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xlnhshmm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rwbarfbz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3crmwppvy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cwweeojw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cbczzrrh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xmlgfpac.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eicvgbap.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fbfyfuaf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zhjbemoh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uuouurfe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yefijbju.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jncvttwf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zywymvns.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gssmlcsp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3eipmxbet.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3txowbajw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3corycbfl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xllqgsas.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rbnmgvvj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gtatrkzy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ctoitkpp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qmefzvqx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kydrojbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujlerkie.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ryunlkod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqowqjww.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3myssirwh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wutniszo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uoagssxc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qksmzkxa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kfdgvqwn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jzpmndxt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rivlydom.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pntnxiha.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lhloxwqy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gfofzuex.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lbpzkeiz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3llvtkoeh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3keqxonib.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ywfbhmxi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lxknspof.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ekaniwzn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3whezktlc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ichnbeqb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovtkhfsf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ykwqatfv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mfgjssno.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cenwglsi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jiovprsb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ndhfyshc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3epjloaoi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbzxqtb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3neaanxfw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ptzsklna.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ccuqqiza.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3advetdqq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ihdxbqki.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ndekotjo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vldhxjbr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3olgkdbai.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qbcmytxv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3woovwmyd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hzpglwrm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jqqhjxng.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3yihjlfbm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmhluax.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zwhlgpcv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mudgnhtg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mhxoidyc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wbsleuql.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aymcybsm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3omsnwdch.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3skspjpth.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3buagaqsx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3osxsktpb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fciaceew.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mfetoiyg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ydmmlsde.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3svwbbaum.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uftpmcro.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3beurrjck.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tttymytr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3iwnxqftc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lbdymdxw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bfwfkili.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rtgytasg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lhcvstxs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dflczmbo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wawudpcl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nendcyym.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ykmuurrp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lavvxagi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ltwssovl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3nywowhir.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3odnrkdnx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wewmlqvv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fffncsgc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ymulvzdf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3azacccnp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3esuxgwuy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fhffnvwe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ennnzboy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sgrecgpe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdstwtb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3otpdlgrr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fqgsuwem.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jgeuvnri.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lzecqskn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gdgyjowl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xfudrldo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dmeymjzx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tgdrskmd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3cpxwrlwr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cmwfyjhi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pemrgjqe.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwkfpzc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xnqmpnvn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eajtewvc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ualasvfe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mctfuuih.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3igusukmk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fwgzhlng.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgdqbrmt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aahqdnur.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qgrsfzei.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ndmiprbo.html


<!-- 参考信息 -->