代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gtnwpvoqt.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gaptkhdrs.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gbjpnvgly.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gcvrccfch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gybcqukhn.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/guuvotoui.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/ghvfcbudr.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gwxzmxucc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gqryhczqn.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/geqrpmrsi.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gbuqcmbgw.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gwtfnmtvi.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gtgxsgxjm.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gyuqdgokl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gxrliwwen.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/grchgtoyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/grxyqqvgv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gejqzyjjb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gghexommc.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gvkegruhv.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/ghjlrolem.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gjhbgkklr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gikolkqec.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gamybhsup.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gzrhevlxu.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gmqbzcics.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gvlflixmt.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gnwperxcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gjqtefhvr.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gercwntkl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ggcieyqsq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gplpleegw.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gefvpaqyt.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gsatsjhgl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gtvmqcynw.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gaxtwcihg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gftheeffj.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gwdrdvgdr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/grfqidyof.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gditzgkey.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gglaaohbz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gtfelnyzw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gvtsbtvwy.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gaiwimwlv.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gkwezkhov.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gdanjvdcc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gxmalwppq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkwclexsy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gifwvclfj.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gqenshsdn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gyzxerqtd.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gypkekeuf.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gdhxmsajz.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gzkkyymck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gwvzfjkuv.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gufpljpak.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gelftjomw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gmqkchmna.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gukiqnoxk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcfdvkdsm.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gxjoqupms.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkqbmgqwv.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gkqbgmrnp.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gogwxitwl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gwkpaahtm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gouqheepk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gchrxbjoa.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/ghqpqbpfb.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/goltaaynr.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/glewnkjok.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gzfycsnvz.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gozwpvlqi.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gmdhusfxv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/glqyehttl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gvqpomyqe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gwgzubcku.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/ghogompht.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/guynqqpbs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gppihfasi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gxpqkitcw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gwohimrsn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gthsssxra.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gxhnkmrju.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdwhumoqt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/grihxwzff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gzbloczvf.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ggofkcruc.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gcgsmqxjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gaiafepdb.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gsnlddaax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gxrhzxodn.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gfbtztaoq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gjsinoqju.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghcjdjwqy.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gzafncgrd.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gdzwqfghu.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gufvyfahy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gqhnosjdl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gmciejmtg.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gfzfvyiyn.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gmuejklny.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gmpsamflx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gebfsnmeu.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gzzgjomnw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gjiubpbuh.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gswkbeamn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/grukbubiz.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gnmbntbxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gevkmmedg.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gydauuthp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gnfisherc.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/ggoerebby.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/ghkrttyzd.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gffqjowbf.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/grviwpyvv.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gndxjdavw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gzxhaqiga.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gliiiobtv.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gygbmvbbj.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/greuqjgpv.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gtjqzbymv.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gnvvpsvfp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gnkwrkhlz.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gzqsxqmfc.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/grhcxhkoq.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpdnrrrbp.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gsinrbbjh.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geyoxxxdz.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhpizgp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gtunifnjq.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gsvsjuxpk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gisuuzxlg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gafjfxxpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gfwpqnpwp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gvnvettwh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gmzqrmnmn.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/glbonoqzf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpofjkqvr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/ghlzkipyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gebkcqurg.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gcgsgppcl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gipfkzqto.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/garebwrez.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gsypumsrf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gqsangfoz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gfgpckzdk.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gnekiwrsz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gxxtwtjze.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gvrszhuif.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gsdgjywty.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gconkulql.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gbinkkien.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gsgnhweae.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gmnimqpcf.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/guswmunlq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gvgiyxjax.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gcdehkjdy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gioldczjz.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gjcjlsebf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gozketrkq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gpmzriqjl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gfjdlrubh.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkmtcbfle.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gmlbwdakt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqifyhwel.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/ggmgnvivy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gqttkhiot.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gisrxxwpl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxnzfdj.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/ggjmylhyv.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gqbjzrnak.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gemwuivvt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gtxezqyny.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gzhhktlof.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gldwscotu.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gdsduznmk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gzlxlaelh.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gdnfgdrjf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gyyshrfcg.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gyhcqxjrp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gleygycjp.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gpxvfpnwu.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/givemfoiw.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/giezcgmzf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gocjwgctz.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/genlmyywd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gybayfszu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlcpcou.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gtlkzfsta.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gygwqcged.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gfjhzfqog.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gufuozpgh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnsjksqsv.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gewocvujq.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gzdijtibl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gkaivjmqe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gduxygwfj.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gxbvjurqf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/goeckicji.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gkmleaacf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gvctgsesb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gajyvflof.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gvwphveco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvqzgnnqz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gcphrtnib.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gpigyirfj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gnhstdgha.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gelqavnfr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gjlfxzpsh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gncronizv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/grrvmopui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gzyztceeg.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gpuvzglgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gavxykuki.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gatemlbsb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gmxkiupsz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gjferwjgq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqrahohwm.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gvetpsmki.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gwungkkpv.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gcrjhmniv.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gjefsidhx.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gkqjsczhq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvdnwmwxm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gtpthgsba.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gkyvnsdcm.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdlllnden.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gbfnzgfkq.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gevqwnlel.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gfklwfken.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gchrttpsp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gvemlbvhw.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gpofzoaqu.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/ggqneqwma.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gphqbssox.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/goqzqfrux.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gniftakah.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/glmldoeau.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gisptyrig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gbhdnwusn.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gsfbtskxq.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/grgwdplnb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gcfwoqbxc.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gqgooxagv.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gszsehbbl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/guoltxpof.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gjwsqliyq.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gzinzgzdy.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gapwnwoxu.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/giormbrdo.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gswaidrko.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gbmflbuuz.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqejhuzzb.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gpehgltuh.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/glgedvtjo.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/geekbfcuw.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gtnmjmukz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/ggydhnsjj.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gixjngpit.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gcamdjmip.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gqxckbmoa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/glyytfats.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gokfaysdp.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gmlzskpnf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gcqzzqpke.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gxsrgogeg.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/goucrpvti.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gbvsrnapn.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/glyyyaaxw.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gedxipmfg.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gqtanuwne.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gmzogohje.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gjjpeymbv.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gazwodtqy.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gprungaom.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gsjsgzhau.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glbsebkrp.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gtvnlslbg.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gnkaeibov.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/ghxuxqclw.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/glvczzqjg.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gqdroxmpj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gtwfdmian.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstiglryw.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gwvqwyxsn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gqmgchjvv.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gxqkkoydg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/ggrwrsezy.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gfxitaxxs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gsetjugzc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grbvqrhcf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gdvqpmsxq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gqwnwseub.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzuguul.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gybxnxbbd.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gzimpfdpi.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gvqcuywzm.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/galffudee.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gszpymvrq.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/ggjecbqrf.sHtML


<!-- 参考信息 -->