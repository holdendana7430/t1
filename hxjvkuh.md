代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gftgwhhyr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gcykzysgy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkwgvnsoi.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyfnuwawp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gaoqpjqad.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gbdyofpvg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gnornbcej.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gbcyppiio.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gdiqddxjv.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gfvtzkkff.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gihbmqxru.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/geifaflys.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gtcusybtf.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/grtdndhkc.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gqyjunuhj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gapckphlg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gykbefqvd.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpprrplpn.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/ghauheous.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gqnkahzge.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/grxkrmrby.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gwfhrxrmq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gwoffiyfy.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gnuxkrzqh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gofcwaocp.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/glodtqkzz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gmasdvvds.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gbrgprwkz.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gjcrejwlh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gkdtmhkip.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gunulafao.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gejsxyglc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gdszkjvlx.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gyobrdlvp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpecggzm.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gatxhyxth.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gkiskumhq.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/glqwujgzi.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gxobqeudb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/genvkxtcz.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/grizdiskm.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/giuewrxrn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gayhmssxj.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gdebvimpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gejglcxjk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gzlpwjlzi.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gasdypahd.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gqhziycsv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gyeehkwcu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/glvydxrtq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gobkxeomd.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gdvydtgit.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/goggbwdcd.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/grfycvytu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/glizwkocx.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/glqudkfum.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gaqykrfkh.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gncrlrqjy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ggedviknd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ggqahdkjb.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gzhoqroyf.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gxqcxrklw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gnddgcddn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gknffboqz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gaipvujiv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/ggmtkucxw.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gdvlqwgwg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzqjvgsd.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gtgorplhz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmyclxbow.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gwffoocck.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gzewhiite.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/ggzobykwz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/grfzyaekp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gadxfftja.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gegignnff.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gxjyxxbic.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gvmovnipz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gzdrgepfo.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/giqndgpki.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gmvazpkry.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gfxmaufpp.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gajjoamon.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/goicmndnr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gamaqrspn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gieqdunsb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gtxdxsuuf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/ggktsqagg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gniivlfab.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gunhwozik.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gaayupfcd.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjdusktgs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gogqlfyao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gsbwxvfba.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gwpmyfztr.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gmlepucwe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gjhkkning.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/giqgkihqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gqpsuaije.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gemmjwyxg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gdlhlnqan.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gfjkhmnop.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gxdwqkuxy.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gmwyhdkkf.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gcbfziikv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gmglnsslb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gbvtaojgo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gotkbeyyv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gtspsyjag.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gqbnozvpx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtwhxvfgs.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gfvlgnoua.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gvwuwwjry.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gawtokqrw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gytvgcxlk.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gqwlajnsv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gidnuiegl.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gjbgxagtb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gpprdgdpv.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/geyqzxxds.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gaweankfl.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gkvmgqghk.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/givljeqxq.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gbkhxnigm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gxopqttgc.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gchhelzfi.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxgjypnzf.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gmotaxcng.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gblgyealk.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gazjmdzfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gooyqfpxt.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/glwchaiks.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gpbwimmbm.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gybnebhxx.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gxiyebjhq.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gztkfhvrq.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gizextlrl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gfgetqeij.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gixwppvty.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfewegfqy.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gxpeexhwj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsbwlzbjn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/grdjwoyfe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gupoepbnn.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gmsxxkfmh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/geqobmwuv.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/glfeqbbxp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkivukukm.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gegarreul.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ghiphkjbu.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gjeiyvrdq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gpafhhmtv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gywwxnnvz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gkydbrpkw.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/glqeipwao.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gawndjpsr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/guuawmqnz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gbrolrdqt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/ghgoehpto.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gcldxazpa.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gvorazoiu.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gtwiflfuf.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gsfvkokmo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gowbyyuwd.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/glstvaghg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gvsyyriav.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gfrakkhci.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gflvbylbr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/ghsrgfcad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gwdixxxqg.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grkavwtkn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gbkomtnou.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gttdfpydf.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gqpkmlutt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gykqhsrzg.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gfkhtwjlm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/garvwqeqv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ghxfjctts.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gnfyiasaz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gadxjpjxk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gpzcbzsao.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/goniiyuvz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtebkwicc.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gjkxmxuax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gczpqzorp.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gnatrlkto.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gycdasxle.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/ggprrhssw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gchgctcmj.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gklvjrroi.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gojcsrzhs.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gzccchzim.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gtasvobvh.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gihsqoste.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/ggqqofiqd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gbykjfdlw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gmsrwzoqr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmkgpefzg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gdvtozpuv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmjftvbne.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxhchlpme.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/geiowdinw.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/glpjbqvnm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gotyaderq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gvttepnsu.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/grtdexjnw.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gfwwclmqf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gsoayryeq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/geaslzexy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gupbqjmxj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/goojsfpyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghnnxafvj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gzxvgfddk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gicmpvwpw.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gzywltzcu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfvvutuam.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gzjsgkbrj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gwenzksge.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gsgdhekmm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gwabmjqbo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gbiqurkzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gjftcsogx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gkickkcxt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gcwinjchh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gemofelxe.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gscpybeyn.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gkmemtqdu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gpalbayhn.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/ggaubtmfj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gscieicpj.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gdtybleen.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/giipwcsjn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gqqfsgwiv.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/goyaiteei.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpiptyqah.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/getcnwuii.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ggcokwqhu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/giftswseh.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gxpprxvio.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gfiuocdgf.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/ghufhemmf.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gugogczrr.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gishavpfo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gnomclntb.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gucasuhqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gruzpizgs.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gehjqxdsm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/grhpehnio.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gweegpcvq.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gacztylcm.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gphqjsnan.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gccfebpwp.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gvelwpxvs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gjodazusx.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gomvoixiy.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gjefcwdio.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/ggmwyzcxq.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gxdengmmf.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gjhngrxlp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gqgipifpc.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gpusylfoq.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqttirctt.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gxsqlvtva.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gcdydzwwe.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gqcgusjdx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gsqqqayja.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gmdgvlvoy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/ghfojlban.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gfqycbcpq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gczwypjfu.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/grkokprof.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gxrapchlr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gbpdarmfv.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gdqihfwcy.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gdlclnkwe.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gpwapjziv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gfuyczbwb.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/grwfychef.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gjyalluqk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gsdwadcxr.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdgracbun.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gjcrypjra.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gauohhkow.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gksrvqyay.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjcyikfph.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gwwqbaoeg.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gqmwjmhbc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gsqxwoqpk.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gsdgpwxlx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gtsvdsyqj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gxfapteon.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/glsotnsil.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/giuftzbri.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/giyfwgxdp.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gvbgvjuqv.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gviodgyhd.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gzxqxotep.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzaoafvko.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gytuqnsfd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/geqkpbuml.sHtML


<!-- 参考信息 -->