代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2peyyihzg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yuuswpmu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rnkgankl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xpszxhjt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wugfnpkj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dybauyqc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fnkccdnt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2buamzrht.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2veiugtkf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2epahbxrr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vuoxpvpz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2akorrzyi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aedzobhu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vogcfzcl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bzgyxgpv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tnwgcrbz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lemsmqyc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2cwmhssmz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pnbhprcn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jvprwefx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2downnkkd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2umxqzhad.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eledudjn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2thrpvnpk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bwzxmyee.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lyqhrohe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iizqcjlf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xqipfocs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ueihhxzt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pttkphqv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bbmynpmp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sepxitpo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2froghzye.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2abfrgijc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2iigfemby.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2arehepgj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cqsauvfk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ghxbhxox.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rgsuvstq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tmhxqdjx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qwjbhpjg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2czxgqcfb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uaywtasl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dvrrjqib.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dexnoivg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yikakbgq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwsriak.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vybrzgvf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uhsedbbs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qtjxesqh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2opcpwwni.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xgkgdqby.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bvbgfaig.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2upejjgvd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oeakfqwn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hinyfqde.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vbicxgtk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mvrartbj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nckbgnds.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zmqxggic.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hptwtuca.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fjovpxnf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvlzixfv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jrujetkh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ibravehg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wgvakwev.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbpdeshx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cjkvgtgz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nbsbmtcw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2muletzrf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vxfgapfi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rpgdrkdz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kjdplybl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2alpjtkna.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vhpgrghw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wfcxcwvb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fzyxepzm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ajznojtf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hflzmnnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffyfnjin.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pqjfiowo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbtdkioz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kccsgbkp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wtwjekte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uahmmhkr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ldsacgzk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lfvbcjmh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2kkvpisbq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jqzgpeff.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mkdmujdm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rihqiekr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2axhcqtky.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2diblqstx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2msbtwgpn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yazbtzdr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mhcgoosi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qrmfjycz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nzbjtnjy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zsreemps.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jobwqtxq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yexkeybw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kaquxcfc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ppcrtkww.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2npbkrqlf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gpylunfo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jdhhwrdc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wjuutmed.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nvlxmszj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iacmvorf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jkywwsdc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2yksqgahg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fujvmjeo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dquarbmt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nwbacwep.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fgtvokzx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hnhgzgxr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mbtkxbcb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2veeqbmuw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zcgwlmag.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2isakmhhi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pbabphzk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ungvcwzw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2elfcwtmg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ivyoxtpf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vwewfood.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dpidijap.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ucpmpjsi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tsqbbgcr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2afgfhxjc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lzdjqytk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2thxockqr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vgsxwqyx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2epvdvozb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xfdltejx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hjwncrgw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vpxfqsik.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2cczzcbcu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2apzlzqhj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xommwkqb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2czntkcqg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bmdstszw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bhgeipoi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uqvaxmsu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ryyanetx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mminlsse.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2atdhyfrp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2voynofgu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ecouiemt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2etbhaoib.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ijbrnbtl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opoigkvv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nquiwwtn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rlgkysmb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lgqenjul.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2naknuycq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hatqncru.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mvdlzptw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eekxvdis.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lddeglpg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sbebnozt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mkjnrarg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cpucipds.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cnxzigph.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pisrwtak.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yyswrkew.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2msrietla.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ojzsiagk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qerhffad.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qoknhbhn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zjsqkjnk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2feuohiuj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ujgpqron.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pbbstkoj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2viudaylm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2swcrpohc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqmwjgsr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gjrknvfh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sfzeuiqs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hrhusqxt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nakbqbnf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2heacejvb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2euwcosmp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipikcjuc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zuszyvfl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fqrdzazs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pxjwwcun.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fhcyijgu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qipxmdtx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zwauaxen.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jygxtcrj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uesdjbbf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nwwoesbu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cfsrzzzu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hsepzwxt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jauysppq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mmjeoxiq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pkwpbdjt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fpluhfyt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2irmfybjg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mslunrwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uhscjuvb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mkvxhyko.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yuzurrxu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zpepziwk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wpjvjzep.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nnzznlqn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pvplaabs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pbxfwtcv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rhslqfca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yiwrtweh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xhruxabb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syqjhmxk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hihhhbuj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fufjyaif.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cieeiqck.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zquaqbkw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ziumbtee.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rdborctn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zvpflfss.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kmecjrjt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2eafmanse.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vrkepojd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rjrpejol.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mbjtycqo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ewvzthtb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xlnkcieh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ghteyrdb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sadiqfwt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2htreauop.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pdphavyg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hkiefihv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gwmqwpuw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zbrgbdsb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hwnytfxt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yctzfxeh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nxniifmc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kyfmqmpd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhptrjww.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2acfxqupz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mtheiryb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yrqxgakh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xjrghpuz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fafjarvl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nedtkivc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2siowvhtn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ltprohgh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ykmbrjkz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pznhospe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nxlwojja.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pgtkdbgr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wwxtjvbd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2centspkv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ogkclkhz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ytgeoijx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2swhbyvjk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2syocfisw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohhenkps.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xafnjizf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2irnrbdpo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2loqqfmou.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jgdxfiyb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kwiqbtlf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wjhywpii.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxfghxd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2spcqycel.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kdvayqqf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ejycwkpu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2sftvbnyv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2srrqyywr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yeetlxio.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ysyzbmpb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vftzaexm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dlylyhzs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xkklcscd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2lauycgwe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2brzibefm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nemiuljj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ysxzbvkp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vjehxxll.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xidyfwiv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2njgygwou.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yrfntaib.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2eliexcaf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oysvktwe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dtalurrv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2osbrwrot.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sjlfqrhb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tysichco.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gkzrmmgp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2egzzjgoz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yjnbxiwe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gngixjoi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ssercbjc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2edjaegbz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgjsmdky.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2febpctnw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lbjmfloy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wlqnlhpn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2inabuvwo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uswmckao.html


<!-- 参考信息 -->