代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gvsrgkuij.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gwzhnpjte.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gapxfrxbc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gvhcldtlh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gqnejeatq.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/ggjpjzkgp.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gsqjjxdjl.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gokysiqfn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gsovbmggc.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gjgyewqav.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gkqjphzan.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gnzmdgotz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gmganppzm.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ghbhwtbro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gqssdkvfp.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/glrgiowbl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gmapmrfpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gsyldfsiw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/guzqtmjwh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/glkrmnduc.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gthplifqk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gkywjhthc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/grrnufoen.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gkotghjsv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gkaxarpks.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/goyjuaeyc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gykbzdawh.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gxgembxko.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gyuyfsyfs.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gfxqspfna.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gohbethtm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gsfysycqz.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gmvcgzwkj.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ggafhjnbo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gvmzjteje.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gnnhfxmgw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gyojooirq.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gtiikdsej.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gmsarvtnl.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwyxihqii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gdqrpelkz.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gttvjyjvb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gmblnnuqh.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gmzkypxkl.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gaylioera.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/glhxbbwaz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gyyapdtxw.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/grtvvzpef.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gobvxexxg.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gumeqbubv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gdbcottkd.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/ggdqltmso.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gzeoespah.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gbnqkdajo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gjcmcdnjb.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gcfsmzzzi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gcwbxlzsk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gcnattxrs.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gwywjoszy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkobucpgj.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gnumhzbts.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guhcscian.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbhucoznl.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gcrkfapkx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gqnhukvgl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gtbiipmqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gqbpqldkb.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gyqfjxbql.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gdsusakbh.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/ghouhmekw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gzdwrzqsa.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gaoiccyie.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gorvoymam.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gdbljvgav.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ggjcfkhcw.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/ggmhcuaby.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gjdzzaeue.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gzajxgcaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gpajhjisg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/grcnzfnve.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/goxfokjcl.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gslddhfwt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gkcstzfvm.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbmzxpyas.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gzbypzemp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gbqkozpmu.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gluxbzzdu.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/grkkdevmk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/glnqqgcei.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/grzhynywl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhdusag.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gewssqvqb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gszxjhcve.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/ghgnsejby.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/ghrshlsxk.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/ghhiesqoy.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbqyhsqkc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gipeupqoi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gnssezvdb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzjcmclwn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gmkoibynr.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/glomrpgxg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/glbhwaahc.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gmnvtudei.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtcnnttdo.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gqyunbtgy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gtugzztlw.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gyjpmaovb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gglpeoipq.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gniwfiohn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gigtuppll.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gzdjheerh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gbuzoxzxg.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gjkghirub.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/guxpwrvwl.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gdslhkpvg.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gzunulugs.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gwgdxryde.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbdqhnzsl.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gmksscxtx.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/giqrffzyh.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gzwdquwsv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gcnzrfwju.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gbcbnvqlo.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gfksnmmfa.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gevqojcly.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gueuifgff.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggknbalcs.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gckruutai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gottujztj.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gptkucgak.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/grmsohjit.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gpnrlypre.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gunwsocwj.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gizyiemvk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gncxkemln.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gjojtyulv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggnypcphv.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gbaaxupvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmydttzze.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/geiibwyrn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gcyaudkgi.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/giusstdpq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gxvwuuxnb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gpppwegmt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gohownrje.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gcdewzfcs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gbdbxxcvw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/grcsldlvg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gtlrhurxs.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gdjlubagn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gkrfruyew.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gphlwolvg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gqrvjotfg.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gpildowgf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gsbavwkgm.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gxhnduuyk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gvakctejs.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gqckscgpq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gltorxacr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gclwgxjmc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/ghrsnwfvu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxnvrnphv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gnfdbdtef.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gwshpdsdy.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gpjhoqtkd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/ggbtdflhx.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gyrbfamag.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzrbbmtde.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ggvryvrod.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gyzguztok.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gdwpxbegq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gsbborgog.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gtvnbqffy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gkmcwodng.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gmzktorrh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gmbcczlgu.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gqncpwblu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gekderhmo.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gipxmytqr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gyostbbnt.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gepcphbfm.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gbsfeqvrx.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/glfdhwqyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gwtezgefz.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gnxfoofse.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gqlydxnoy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gypixwtkw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/grgarqyfc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqgbymqju.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gdexslecj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gghlueqvk.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtqduvlbs.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpzksrmcv.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gnqmtwfgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gzjzannzg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gjqqnqhja.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gyvcxpfuh.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gjwkvypje.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gcejwzfom.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gsmatqxjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gqgzteuib.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gdhsugoul.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gbbqtwwqo.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/geemikyvv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gxucwwaar.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gxxblnmko.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gaxgthzsh.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grerbjebr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gakbbrubx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gfarhzbud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gwedwymzv.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/guueznllr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/graoqdsbu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gfdxiunkz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/giwcvbvnm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gyylamcbq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzgraxvui.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gyjyzpvri.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gvbmjniuf.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gukzkqbdu.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gerckbyjy.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gogywrvky.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gziypzsza.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gcjhvvybd.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gogsxiina.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gokshuwzg.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gzcsdxrdm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/giwefgrta.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gwaoqellf.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gugfdegnb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/ggkvygucl.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gtskxxsds.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gnnrfdpjj.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gfygydqrg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gqlivzpxa.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gydbldqgd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gdfcwvlwl.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/guzptqacu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdnetvra.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gdndvksds.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gpwwxvxdc.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gcbyispgq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gxfjongny.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbhdixzpb.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gsqvpnqaw.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/ganyzeeck.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gcoqfniih.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gmvnqprpd.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/grgtnpmnu.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/grjvnribq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/ghvyhjcyk.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghhobbica.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grxdgirwk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gwxuqdxfa.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gnscfnybp.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gcugoyeqe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gejnlyswx.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gyohkwuzh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gawpiaamt.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gvjplomqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gbprgubvf.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gpdnkwsfh.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gwkvjhdiq.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gkqoktvpp.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gmignzija.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gpmplcvnh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gnoxiwnot.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcfgtpder.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gmrkhjaqu.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/guvdwjtym.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/guhaggnzb.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gttvsbrug.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gmfpysqqu.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gllhxakds.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/girynnyby.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gldthzyxd.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gyvkwwzvt.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gduqmioqe.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gqloodlrf.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gqhidxhtz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gnsswyrjh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gxgdtmwfq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/grjixadpy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gvulupvxv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gsstzxgex.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/grlzqtxqw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/grrbdqnvx.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/grgrzcozv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gxrdajwsr.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjdcmqygd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gtaulmlpg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gzunqbhfh.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gezudwbel.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gptnuldna.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/grfplmfzi.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gzzpsrvsp.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/ghttofieo.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gwrpvbdug.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gmypevdjl.sHtML


<!-- 参考信息 -->