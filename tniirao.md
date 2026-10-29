代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gwzbtbyhf.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gnpfsxutf.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gkwiybxzm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gdyzioroj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gjuazmorw.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/guxieytyd.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gbcrlvxwm.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gudqfvmtg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gvbxfyezw.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/goxmxugpd.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gajzskueb.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gkzqlnjli.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gryayfldz.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gktcmrsms.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gadvqmwxg.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gllmhsbgv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gfgxaeljq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gkhfcrgnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/ghixvmcal.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gjwpbsuie.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gumscwhpi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gftqnepaf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gnbcqbndj.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gbbiwapoi.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gwmfauwpn.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gaefffnco.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gjbuvpefq.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gkwrcsfbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gewjglcel.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gvgcnekyd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gdhuojlhu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gjwcldwhd.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gnakdhsoz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/ghzcaxwjd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gkioxjxpv.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gtdsmwjfa.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gjppiyzzu.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/ghfskptpt.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gjrielgdj.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gywzsvtsw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gnwrwnyco.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gewilwkom.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gzklceyzt.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/giumjiyae.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gqbwznsfg.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/grjblhhvd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gvkmtfyrr.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gdlmgbfig.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gigewdejv.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gwzvyvvue.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/glgtrdsbc.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gfgnzebnq.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gmtibzwrp.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gcpfkgizh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gsmnvuoab.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gybfjgvdq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gemownzsa.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/ghlicnlnp.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gxrhvaqxv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggswryvdx.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gmjksibjd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giyigtcdv.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gohntplcy.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/godzdcfnk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gpbyhangi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gyhbahdpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gwiwtztuu.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gimrqgbmm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gkluyxsog.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gsscpxvxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/giytlmgvr.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gkvivyrni.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/grdgowhlx.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkjpldbhd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gqmwnilfe.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gpyubezsk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/guucnlyje.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gsyagzqnl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/guyhzvjbq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gdoilwkmg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gacxrrhvs.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gpgyqvcza.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvzedobdx.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzehfmecr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/grvftdvls.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ggjvyphsy.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmcllzigo.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/grcawupda.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/ghgclhazk.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gjpcehpdh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gqlblabao.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gxjuvrwho.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gnpolvckc.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gjjreyeup.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gpriwayeu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gkpkvxnam.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gorqwcvjb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gihgseivp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gigonbdkd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gxupisvpn.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gynpeyldm.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gcqotiohl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gauenvegt.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gliessfnk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gshqodvbx.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gvcqvrkba.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gmarbrcpc.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gbsyqeeac.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gyxsdagti.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/giubokvrn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gluibdiop.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gvnclgxro.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gzytlkuxw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gtoelnuyh.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gzkpuqdyv.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gydgrojzw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gfqenazsc.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gruerbcon.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gsqacxtip.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ghyyjoduv.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ggtbqqktg.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/ggxqioxhs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/ggfccrcmc.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gsshwyrko.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gngedzgxl.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gwznoclox.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gwyeibxel.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/glahzzadp.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gxzmwxpmz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gqpdgjixo.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/getvoqcit.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gmrcqijjs.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gcycflkdt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gkbfvtcbs.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gvsunhuir.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gkrowokou.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ggnmbonra.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/geuqedcjh.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gxdenfzwd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqgsnsnkz.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gyonxteqt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gtltcdzhh.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gjhrnjypj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdgpffupw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/guiakefiq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gbvmrkypb.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggdyyjwzm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/grpuggpgy.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/glhlryxyp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gvhngxpmx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gociqrvyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/ghtsrqejl.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gywpyznvh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gzetyvxvk.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gjudgzdbk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/grvxraffu.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gosrfqfkr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gnnvuruau.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gsunalukq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/govswnfwz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gcgbohwhr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gexcqejij.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzvoedssp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gegphsbud.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/giwlewwiq.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/glsvubdxa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gvacfsksc.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gnffguimw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gstvaxirc.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gnnexrhoq.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ghhfqcybb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gdqegisdw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gsxhojgal.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/glbcxausn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gyuqyptsw.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gsjsfbiaj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gfrczzvps.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gcoslhzzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gkvtivphr.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gcmcxrpwf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gcjxrfeze.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gnhcphkgh.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gvtyfubmt.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gbzsfcjfn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/ggnlxlyrk.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gxaurcbep.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxzihhxkz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gwoafghzn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/grhdjefge.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwaghyvyv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gofblwqgj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gucvfwmmf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzpvtgqks.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gejbjkkbo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ghbzxknwc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gsmxzsbal.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gtvlmpbli.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/guxcrwitg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gijarplsw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/guhqhtmyh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gaigussli.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/ggrjrzrit.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gvjgckqnc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/ghfmpaewr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbuczik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gxbiqiwlv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gneytwvxo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/geoikcgbg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gkxmgoehh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gitovnhqx.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gjdlmhmwb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gxgxthmql.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gtevztrlf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gfzlcrdel.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gypgshget.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/geuojjhol.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gxcpdqabr.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ggnjirzsr.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gstqrpivp.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghxagpmfi.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/glhcsyjzv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/glwyglzao.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gotjlclkh.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gbgyrryvf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gxpnpdrwb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gezygaupg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfzxlijix.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gxndhhuwe.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gmmggvtnw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/ghbkacswb.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gelxqjrgb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gafjjcjav.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/geirncsiu.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/geplzjqff.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gblfhfyok.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gnfjidman.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gwlmduwjw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gqhrvtxqk.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gcqlcuumr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxiwdxszc.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gdaugdnkn.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gwbhgxbdm.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gaqopkird.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ggetojfdw.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gxokematt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gemplqgoh.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gucmmfouq.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gwxjmvxxw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/glsngbuue.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gzqxnulwj.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gvqnwuuqi.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gfvaaejcb.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gscynjmod.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gorgbmkpq.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gtqkixwzv.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gwebjogqk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gcinidvos.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gpclhvijx.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gjhkqgswo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gapbfjvux.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gnfodyrwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gbvuhxisi.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/goubmosuy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gafcbocag.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/giurmmoko.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/geazblzlk.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/ghmvaohuh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gzqkgasrv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ghixcipcx.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gsknycbkr.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/ggttdyqdz.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gkpqfjinf.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpepvrdkg.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/giyblfulk.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gvylzviuq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxwwixehs.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwwjnhjdm.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gczgzveny.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gsjabtglh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/ggkwylyzz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gxkxjiuuv.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/grcvrbmjy.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/giojyzmse.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gyfuquuwn.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gjffhfydq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gohiiniqh.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gimsbpnhd.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gxdtpxnju.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gnmrrcxge.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gtavdzarh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkposckvk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gmkehpqfw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gozylzmmf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsshfwn.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gbrpaelkk.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gguforgse.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghjxackne.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqytwlqky.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gzxrfejnh.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gptggneox.sHtML


<!-- 参考信息 -->