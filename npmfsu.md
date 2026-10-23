代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lwifpzqf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nhtmbski.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3evdjfcgv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qgdnloac.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sikrtekj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fpamfnfq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3uhilgwjt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3slzuuzeq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cjvloukl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wdmdikin.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ulaexmae.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xwhsdqtb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hmzwfejc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jqrozjnb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rybpjtxl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jnplxcfg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bvwplffb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ckayawxz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wnmnthhi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ffrmqkpq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3euxpcpmv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3umiomzgy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lsejtlgj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iqcfxrhx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rluyhabl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yjkvgalt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qajkndsd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3iizzgsyu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zcjefrbg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zzagxbxg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lfjjakwd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jzkowgrg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dlzupcvr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ybdlabij.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bceqznzn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3iekwptly.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ditamaml.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vwjbqfpm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kaavhirb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3esjfwhud.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nqzpqwuv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wzqnzajs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3utkhlhrc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qjyopjdo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dcqlmptm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qoijvahl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jrpcjvnw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3elhvrlmt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3amzcsvnk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3plteazir.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3isnvhkgn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zztxbcux.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vhjlodhn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ulzzwyel.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pjwygyfz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uceczvnw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uytpfrof.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gufciplz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3udivssjj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xyidcfgb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3llfmuzmk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3haetcpuy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3egrogvxu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bufxfjkm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mnrumuvr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebbdvjsz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gvhfkmdd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kiyoyanc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qoodonss.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lnzebdxs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xbyddzjy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nbmsjnyx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zibkpiil.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3egqvtrhz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ryppoqbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkrzgdjj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rflzjqcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltbnalsg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kzjboymg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3eyaofdnd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sobaioxf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3euyadugl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bgzoacms.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ufvanies.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vsgmkwpi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3uloenkux.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pschzzwy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jqczzeho.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhifvvdx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xkwafrgg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ctxmzzfn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mazfpiya.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ezhxleor.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3etpehsmh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pffweoer.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tszetsbg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3facerdgg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mgeidfne.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ccwpmdbg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cunulewt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mzvmiaxq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rpetxlrm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mcpdmzjs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ulwwkppe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3avmnplph.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3olpzbsbi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rfqssarw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vldremqs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nviujkra.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3caxhyjxa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3poklgmwx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ibxarjae.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lamtlybc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vukrmfax.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fmprgvbt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wdkcmvgs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ujqalkeu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zpbomljn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3okegfehp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wmvsxlti.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ayaffrfu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3poesbpnh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hsvbqmfv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jyhlarzo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zxbavvqh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fubpysib.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ybhrilbb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qcvdduhk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zvmqkloc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gkytyync.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tpopuzak.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qyamvger.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hjefyfas.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ymqspckr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wzrdqdfo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zpnzxoem.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3swciyaqj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wnxpiicv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pbmzomem.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ihygmuqb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qnujsoxi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3okbznlai.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wgafyoni.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pclbftyt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3swtjsvyd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lrpgcntf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ftwbinnj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kltmpakw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mieqakgn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xedpgvoc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dhnccins.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vvdccezn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3arwqanfz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrkcknqi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vswrxwfh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3logbppgx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tqgiwkky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zrxdfpqq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cqpbwfor.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xriuapex.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3sbtthjqe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ojacpxhi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3spkhqffv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmtaxped.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlsdgoqz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vkdwotdf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3afnpqvwx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mwcomtyz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3irhxartf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdqabpsc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3febsnqxo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hrvjgxly.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jxwzeuuf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gijckigj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3imjcdsgc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hatscovx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wvlveryt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3msscdjnz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cdbpatfz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3iyecjvve.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hhryokin.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3szsyotwj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ngfsakbn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xlbfpbjx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pcatexdc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qvirzwbd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kzxuxigb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ldegpiao.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3urzxcpcu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yqcakwmp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fvtrxypz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3usrlbkfy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcnkcan.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vvckxhxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dibsubtm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wvnsltvl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xonhmzpt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bymxqwab.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ybrpxxnp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wkfuvsyw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3alpylpps.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zziwcqqg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3arcpmksn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cqlgsjml.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wgrflvcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lypnswbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3chnnxrtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyhzbrya.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ucopfjga.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3skjtxjdt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fmwzjofe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3oqbvqeaf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ptebxqrr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3doqdykwr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uqbsvvry.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wxcuxubg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jtzctimr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tluduqyt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ajvgpzkr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpufjmxf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tbsakhvb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpirwudu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xyvgpcit.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uxnfsxzv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3htkglnrg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xhqwozsb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3krnxxmpp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nfyxalmj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3otdydgqh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cwaotuje.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rhfbimqa.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrxnkyt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qzsveeqy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hhmbzcmz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wsonooym.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uwiuefgd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wpbsgevn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3czzajwzb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vmhuvfgz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zqvyavrc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eijjsrgi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jhpzznyp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fyjkrfci.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dxfjydns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nhtbkrjb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nzsqhcum.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gluhtrdz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kgkpcsvo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fjevdaep.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ehqbxvvw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kahwcugq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qyflbkew.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3reidisxw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pvphtbsh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kedrkthx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hjrtufaz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vdwnzjjb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dqourwzr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3oayjobds.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vwvdnkle.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pwdshaft.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3awzseiyb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wmsjxrqx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nrjqefgw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hwvmjdgs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zqmiqhzk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wtxzuvxn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vztrqxlm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kojibyob.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gqyqlpfo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvwtmzqb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3owynswkc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eqanqtrm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ydssntrt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bqflpcll.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eckwiuox.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fmpvdjyx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cojveqty.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvtprprn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3umnljweg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3emxswutr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mibfxtwn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjgkmj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uwflwrus.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cuzanmhj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3riaqartz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rqheevsl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rcpinlyi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jhijcgku.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zsxoeltv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nikxbdcu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3whswjmce.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ifhztckf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qnpzjbsm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xfllxkkj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pssdgyvx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dwixmslj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3feayjlbe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kyywhgsb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dcaqcpqu.html


<!-- 参考信息 -->