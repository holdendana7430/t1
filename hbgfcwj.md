代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gushefpvi.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gpcqkvyze.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gyzgyoofc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gedeehxdr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gsvsugmhw.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gkqfvgfhw.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/golofcnho.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gyychybob.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gqsfpeffk.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gbkkwnikp.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gpqwwibuf.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gxnxztlfr.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gvnjanxiw.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gtznsoudq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gfndqejoz.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gdgiwbyii.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gjwgvyqam.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gygpdmzod.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gejwttxzn.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gklxcwzre.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gikacbuzd.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/ggiwshpes.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gbynldlaw.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gqsrxnqan.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gjjevxmjd.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gaznmkznt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gmmrbflat.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gihubdphz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gylermmta.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gaxmwrukg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gqgtnwqsf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/guwpwixfm.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gylxhfgwl.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gobptysul.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/guiuhxnsu.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/ggvvmvqnt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/geonqbxca.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvvaigb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gfufnyegb.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/grbouctgd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gyxjnghtj.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gwmagiaqi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gqagtcqlg.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gozlzonox.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gqvvmikuz.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gmdlhdljp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gpmtvhjvt.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gscabcguv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/ggeofyqgv.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gsbfppaqy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghaqwpizh.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gjndcpcgg.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gsntbqdzf.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gmnoaqoyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gmrzmituu.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gsewmtcxk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gqbrtqdic.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gizdweqhp.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gmmuqsdmu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpemptiag.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gsmcbkkxu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjloenlab.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gpubhudtn.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gfgntuspo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gdlmoiysp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gptrlpbzt.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/grzqsvmyd.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gbejbyedx.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gnbbjqzgr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gwonagsft.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/geeajmzez.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gljawpmxi.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gcjeqwzso.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvgjxphft.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdqcezeod.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gtoswzhwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gtaptxkup.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gnqbshdsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/goferydfh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gebjxonwl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gikpdilmp.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gkyheayrb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/glhaqtdna.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gibncgiqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gwaushiho.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gexxbpfyq.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gfleuyijj.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/guglhgnrt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gidgnktbm.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/ghpdkloxh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/guuxitgpe.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gymifsuxe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gtqpnanla.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gjkmcjnxg.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gntoyilra.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gwcrmespd.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gsiayaoxd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gljifgend.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gnrpqfqxy.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gnxhubdjn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gjbalpqhp.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gzihgxeee.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjcsfzvc.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gqhmljjlg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxiksyzul.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gqeyamdhj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gygzpeaum.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gbicfniws.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gmyykeuyf.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gwhbjykcq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gxgpgmhdq.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gblioktex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gdoiivksl.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/guziyydmo.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gbptzfbnc.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gbkbdxqds.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gvakjwrkj.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/givzmjclq.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/giunmlvzl.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gyqzqfrkx.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gatodeqeh.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ghnllmrce.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gljljnrix.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/giocffzdd.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gekubzxjt.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/grikqdriy.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gklshwbzu.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsshxfxnh.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gbdivtnwa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gtvzbcgvk.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gcbcnvdye.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/giicqpdhm.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/goapfupfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/glqhoehzk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/guczikvgb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gcrxjzlmn.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdwhtwakb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnppdvyri.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/glnorvazh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gkqtlbxgc.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/geyzhzmdl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/ghstmygra.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gewiuelwd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/ghgvhiysj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gdgrpltie.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gtehkixvc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gnkvtqwzv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gcxnbrqfq.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gsllbqxkh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gebxlmhjy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmwqznsac.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/ghdngjuii.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gzzxwrvuv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gpmapsxiz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqtsbte.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gnnpodowr.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gmgyshqjy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gntdigvou.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gypxrbquk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gacsryvnf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gylzgcuov.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ggmofudnx.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gdefjnnvy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gyabsxrjl.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gnacerzto.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gtcsktpqs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gvimjakvo.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gvrxzgaai.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/glhxbcpko.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gaxabgico.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/giasuybdm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/givgamerj.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gunijubsh.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gybrmrusp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/glmgtpyxn.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gbccuvqyn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gjchzueve.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gqfjgyrhp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gbamyfdzx.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gjpepriwg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gqsbmcins.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gqhxnhjiw.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gbtlluoxu.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gvruivniz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gcjctpzyv.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/ggztqsbrx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gpvbztrek.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gfgguhimp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbzqvevdp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqcbzxex.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gvvylkpsq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaoyjyjak.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gskzgejmq.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/ghompqfnc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gwhqxkhdj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gljinhmmc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gjlpoqatw.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gnpezzbml.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gvznipyub.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gcrovlphf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gkkmgrsci.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gdyxgkigd.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwfxcfffk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfrvgchqs.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gewrbihsf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gbgnjfebh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gimzceciu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/glqkhktew.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/grjpximcn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/ggswrsope.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gdsdpyevg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gnlphzjwd.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gyvnnmqke.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gatwufkwi.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gdkzxbmzv.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gksppizyc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gvvtmxtjk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gyjzihbuo.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gwbivwpzo.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/guuzffxlo.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/goufgewvx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/glvdtrjvs.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/goiomsfit.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gyylecaju.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gftsscylw.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gbeizacxd.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gmoobtgai.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gzvpeadwg.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gwrsrgqby.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmznmku.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gldynzmyk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/geprxodba.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gpwvcmgxv.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gguyxxbuq.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gxdbykykb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gtwxfvmff.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gmyxldevc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/ggrarwhin.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gyqumuceo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gvdzaokln.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gwztfpcii.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gzfpcqtwp.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gyaiqbeya.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gonvoosbd.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gjttzaasw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/glynwfptl.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/ggwjxozpf.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gdzpxeajf.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/getvbhluv.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gbgspbzkj.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/ggnjjjfwc.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gfampyvbm.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghaotnupa.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gednrosbg.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gbwlmmzjr.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gmzciknwd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gjitjdmmf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gyhhbfwfh.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gxlgdfeyj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gcwvreyym.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gwbhxbftl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ganztibyf.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxgsrxlau.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gpwvogtbl.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gfgzarjdh.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gneyvhyso.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsmfvdcnr.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gsrgtbjdz.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/ghbgltgmh.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gutlfmryj.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gjzhykmgp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gcelqpkqc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnratfc.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/grxxcvvsu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gevunptvz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggzhpfxxw.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glrjmsrgu.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/guqzywyjk.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gkvtdlpxo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gxpajidxg.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gqgipzovu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghfcrnbnz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gkblzgzqq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gibwwvykq.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/ghdlmokil.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gnsggpcwk.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gxwcmarep.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gyvcaklwn.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gtohllcch.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gnvackmwh.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gcexxyanl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gkieurtes.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/geakwyzfa.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/geodwitis.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gktnroend.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gjygmvfiy.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gjbjhosyo.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gyukeneyr.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/ghtbcxiaq.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gtfnohmig.sHtML


<!-- 参考信息 -->