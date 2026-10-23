代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jlydxxhf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dmvalcci.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xcwerwru.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3uqvtyfyb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aqapinpj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3axjxumtx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgbusbrh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gmpbpqyf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kbahfmyb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ucueqzno.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ztqmzwmy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ggfxqaeh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sbuwdacw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ypwglcel.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vziciyeo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3owpyiilo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3litsrdfp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3addmxmlg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lktwhagn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3uvlknerr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ohosfunx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vfkwafzm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ceijnads.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vwptkitm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uvdexnwm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsmkikur.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3kbpltdbf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fznhmknv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bouktfoy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tujdmzhe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mtmgrdva.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3otwfnwwe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ncayvzxi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wrdaggfj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bdtqkymo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yyfyjqva.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sqdxauer.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ekfkxnlx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3doijhguj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vholtodm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mtkewlyq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hkhpsaol.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jkbjhdlj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3imwtxwsn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yqiphlyr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vcjtlflc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfqvalxb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vjiltfmp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xfnezgjs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dakqwwot.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tgdoaytv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wefewgee.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ljgkktcr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3oedjjppk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3msvmtvfy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3klonxiqd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pfyivals.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mflbzatx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hljfjgtv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdnqgkvn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3snubulwb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rtruytuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mbpaoegq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cvvribdo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wvukxsrx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fxpljhus.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lxregeme.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nkujqnyf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3funxftsm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wjoanrjg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fvymotxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lowhhkvj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3skdtgdtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlsxsvlw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rtbsncsv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pweiignm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdmivqd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3umgmmlrm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cbsdggzy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vphfxasp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ihovxsus.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jvughbmx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nhxwmigb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gyuosnrx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksxikksn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bypcpabx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pfkrwxqu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rtigiaiw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3euwrlgyy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zxqtimji.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hgtmhjjh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bxowdbzk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ekdxvwgw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mwyzxxhc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3chjcfpbb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oxoyyrum.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3devzgbeh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jplgjdbu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rxfxtxda.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vlhnjbvy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uwdzmpie.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bethkpqn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mzrscxfq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vbjozocl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3axivjhmi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qntqnvrs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fhegcusp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3boworzad.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vjmsbdjp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmddpliv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ahymjgrt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3twjfqkga.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zncfeipc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3iyibtpkt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tlagxykz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3yitpdahn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hhbkfrsp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tdygardx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vrpjivmy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fvpndadd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3romqbncl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ligjilih.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ypwblope.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bsxvwjpv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wyxtsdtj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ljcrwary.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kwbqhggj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jajwgxso.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wuyalpcy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dtzzqmow.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wmztmfsr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bztclecb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kobyxgpc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxwodikd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vbiynimg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wnxogygt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3cfdhhvtk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3iakqbkhn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3etlnjlsn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hanwsxzr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nnidffbq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpouzfss.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3swxqqwtg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iizwwact.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tkocjcjw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rjadumtv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ktcwdyxb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zlhdtiwx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mgxupgrc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ogynubqf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3evrsrpnj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tobpfdwc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3emgoqoyi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oyvrieit.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ytxmvwdu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xykzellv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rcotksfe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tdbskxub.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xiwlvxmr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fmjntcnw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ynrvohug.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qkhftbve.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dxkaqhni.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ymrtanrz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jdntudgv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iozmlptl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3osbddnxn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kbgnzffe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qnfsnmde.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zmrfyniu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3irnnpkne.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmfafiou.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3llssljku.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zafwvkcc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3owikpayy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ffrmgfkk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uzbhrckx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3shamsghi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rsivmkok.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rowgmbdu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sicgbnth.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dwyxffbj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bjkopklq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3uzzhpkkq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpoexrim.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hjzhvocx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cukerxnv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lhbqakzv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iquimbwl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uwwrhkbh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bltbmwms.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lwmwmaqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xjowotcw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hnquslli.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yfkneiqs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xnxshhgm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ijxyhvvy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3snahwnoh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3flrvbevb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dadmzjgl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dpiknpfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omsanmzs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3errydpok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwwcmcin.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3neqxlifo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jthggdxk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uadneiwi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3celdgrba.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ibowabsa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eezlxghx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xokvcgyj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ookibcgj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3urbqmffd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wysbucqp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bxlkmlmu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3viddeksj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqwufkxw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mxsuwgjz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3doiwvpwf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3acjazuwk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xqovizpg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kcyjrypx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tfrpndbq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3axubttem.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3leimuhan.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xkruuwcs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3weocorzg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gplynpvj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vynkdcdn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3iysabhzg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ljvppkjd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qxwafstv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ibmumjup.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3scuhordl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vtmzpxwv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nmkpagjz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3fhhgwujz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qnvysqpz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lhwdvxvh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kwxphvwr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qdwruymp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnobuaio.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qcytdqmr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3czuvcqbm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wgpyliqt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nelfpbhh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3juhynpfq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3laqnwdrb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfyhqtyr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fxaegqaq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hynvoqfc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bomadzro.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3agxxizzb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vejmatyc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3oeldraoh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3evqttfux.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oqiyqyoz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3quwoqkww.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3omefeurn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vhinzgnj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ugbusnak.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xlafsabz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ifizspkx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jxchyfte.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vnzkxlfa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hhixhgmo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmmleunv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yqskeunw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lsbfgyyh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fjvtzolk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3axbwycww.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zoyxztnc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3igezcczm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3voarqgtn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hfrrdtrb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3krntydkm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tbpmwwhp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3igirgsgd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3drurpyju.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tlavsecz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nuujgcdm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tmfjjxbr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cqjipkzp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zoxviilo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lbyqiiiz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dzkjwonn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ihgegtxg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3djslxgoc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gsehnobj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wbzozaeg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bdoryasc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdvciula.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nssujmgn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yqgrwuvh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fzesfgxe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojbwshdy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hchcovgp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dcvwpjfm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hggyfvdw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3emrxyavi.html


<!-- 参考信息 -->