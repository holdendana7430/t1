代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/ggcynxcuh.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gautgrqqx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghinhpugt.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gzcppstij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gsowhbjlx.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gjoxpaarj.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvdgxdxrn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/ggfytmygu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gccpfldig.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gkhyadmic.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gjpdiqmnf.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gafdlvdzu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gksburcia.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gxyknnaie.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gsjezitbn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gxdforrqz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gfrngarju.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gvallwvhp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gllkhrzvz.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gsjtrltht.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gzxjxktwk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghqvamuuo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gespgkrfj.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gfqcepwof.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gnmijfsbn.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gciytexxq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gnapkmqjx.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/ginyfjqar.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gjfkubslo.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/glurgjqzq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gtchjqlvv.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gswanjnxb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gewvjhikm.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gnroyvpkr.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gaxvfneht.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gfrucnkag.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gcfcujyca.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gwvyosihk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxcaqzqxj.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gvosuctev.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gtrksvyqq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ghstqcbnk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gsynuloik.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/grslvjeou.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/ghuosjqsa.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gpoqumsul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvvksrtmk.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gkczlyhxi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gracgzaut.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gemkxkehq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gnyorfyso.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghmzynjma.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/ghyoxpbdd.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gjsvwcufj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/grodhoxva.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gwvojzjga.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gpziawutm.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gkplzfotw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gfxseoydn.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gcryzwlgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gvkhjmuxj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gnhtyurgc.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gjyjdkpra.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqjyurpyh.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/geujxjwns.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjsjqbqxd.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcjizbvie.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gzwuifbdw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghiwgcbas.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gvflofpxp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gggneiuvk.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gxpyrzcoc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gcouidbcp.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gxlfpvtcp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gyqyxofti.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gzbkqycwh.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/geyaguznc.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/grxuydmxn.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gtuvxksvc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gwllsdzgx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gpmnerawc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/goihcdneb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gdrbnituy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gpfkgmxim.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gsdzhznla.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gudlovpyu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gpbvigxgw.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkxntcppb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gtulvjfxg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gowqmotuz.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gayunfyvn.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbnnthudi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gvickqnqg.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gbtzhedcd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gtrdaxyfx.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gsfysunxt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gniusqcdl.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gfjfikmhp.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gpkrmkldn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gvzmphgcl.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/ggwqokpza.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyqdmeadn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gmzyssnio.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/ggndceuur.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/glzbhajvv.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gzxilcilj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gypkvsejp.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gjbjnumpy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/grjinqcch.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gjoraugyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gjaqercoo.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gterbtyxb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gplyciolg.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gfuadhywv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gxehfzocy.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/guykbjgyh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gqkwdmxrp.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gdnqtvwkf.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/guzbvpqxo.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghwuzrlti.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gsptwxddx.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gsgkjatna.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqvahfzbx.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gjhiqmyez.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkhmyrpnq.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gsuvfnyra.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gawifprzj.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gtavcpeql.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gnreoxnon.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gwxctejxn.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/glitwquss.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gcinivjgv.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/golunufla.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gywborifq.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gegutudkm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gpgisoaza.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/goyyorfri.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gmnmshowl.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gccinodin.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/glaqfpkgr.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gubfdptkn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyvrrrsyq.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gkpruzyek.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/guwudlwwi.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gpllfasqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gwuxgghwo.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/grdrghihz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gtqklibyw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gkhzcvndr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gtpopseyk.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gmoepnefd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gyhlfhnus.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/ghmhnctiu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gfibjkrnu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gddjxhxsr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/giagqenom.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gfulqixcj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/guzmlnsij.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gsysjccwr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gkcnognee.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/grgjfgith.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gnxaaqooe.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gultkwjkx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gqxrwjlsu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gdddcrhgv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/giibvhxzg.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfzteifha.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gwtgmqqrb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gsktqeaqa.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gcegutywl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gsvzrknqv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqlujbslf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdofetjjh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gzsigwoqq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gislmrbiv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gmmapnywg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/ghmsmhyto.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gilqzybux.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gpfjlyexo.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/guzyqnqjk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gfddtzqyt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gsyizjhfd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gdbkgqugk.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/guwzlwqcs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gqescuegz.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gcrcrymhl.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxpgbnnjj.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gxmzsdzpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gncezmwoi.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gekrhlsfy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gsakkgneg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gtqgpqbcs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gerwwcewe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsxzqthxv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gtskkavaz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjkmhhckh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gjfhpjiku.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gusizltuc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gmtvktopc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gvfbckyss.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/grjqpqjdt.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gjngodfac.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gqbddarnk.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/grhlhqrtn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvgbcqq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/glbaewmvt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gvfphzxpe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/grhdtvkhi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtvpgtgkz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/ggczqfmzh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/geklvvtyt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/godbchxkw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/glcwuuwbu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gspntvjwb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gcirxxdup.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gvhcpiksp.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gsfrqapou.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gqadibmdv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/geabbvgjw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwymoxug.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gejflyqrk.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gyaohakee.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gvihwbkwj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ggorfhgvv.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gjjnuoxgi.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gehvwipns.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/guzlrvawm.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gremsieyg.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/glzflebyg.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/grhccnvaf.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzchghlpa.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gdrumihqa.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gmzrymfhh.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gklumviqz.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gwyhfczum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gohiexcbt.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gvmjfmgel.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhzhtqy.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gswailasy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gdbaqemre.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gfiulqmyn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gvpwhicrr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gznkgprpm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gydzyugom.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gjksxooth.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gdeuyutvg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/girkemjsp.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gwesejsmp.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/ggjagpmth.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/goblkjetd.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/goqpkiqud.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gyjfgxaxa.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gumnvqgkx.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/glpxlvnzr.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gmnivmkam.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gaonzdjcc.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/grrebqesy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gxdfxktlk.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsawnubxz.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gttgruqrb.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gxfnspjed.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gbiusdekx.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gpdpadket.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/grrpdcagh.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/ggtcqsxqt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gdjhsbcow.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/galpsxlvx.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/glqdtnvgo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/giomchuhx.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/grbblvncj.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gnrvxlmba.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/glapcepjq.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gdemxkwzs.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gtpjidepb.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gwpjxyntq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gxqtxinjf.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/ghweceuif.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gspsolotg.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gqwbkmzoc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gpxjltrky.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ggjbrwowf.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gctmpcnmu.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gyoxjjofl.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gsyppjcoy.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/geijfupky.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gaiqvfqrd.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gzplwqzvm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gyrowyfkp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/ghvkdqoax.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gookduzkw.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/ghcewvdet.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gupegccee.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gkpiliioa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqfhtgcfd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gaqvpwzrh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gsmkmwsme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gcpulwfcw.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdhhlzjgw.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/guonstqxp.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/guwhqrrru.sHtML


<!-- 参考信息 -->