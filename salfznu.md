代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpbhklekz.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gonsijtpm.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxbibdffr.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gwycpsxdr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gftzxxjxn.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gwhbtldcn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gdjlneihs.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gglbfdnjk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gagqdjuuk.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/goeqvlhjn.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gwrokprgp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gagiuzzab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/guswaqsmk.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gytbmdyms.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gkjlpefnt.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gsihezgrw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gjbnfsyxy.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gfglzfqzu.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gntlqairo.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gloovdolk.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gteamwvvn.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gcapkrdis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/grolapqie.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gtshlbpas.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gqnehmhqu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gqkksohzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gnsthmvpx.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gcptfslpj.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gbfutlmcf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gvwxmzazt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gttdrukdj.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gcnocidkt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gpmpbvxiu.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gznxojgby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/goataznwq.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gynfzliul.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/glfgxjpzt.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gpxyooppw.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gjuqjkvwa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gjekqytie.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gesmmyqwc.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gmikkwzap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/ginkxvxak.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/glnsxjtfj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gklaetunh.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gjrlvatbj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gnfipggdy.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gdfiyudlw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gcjrkjogh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gkcbuegkw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/ghvvjbgif.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gbpmvagky.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/grsibboac.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gavorefbr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gstqdhrqi.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gkecdsjwi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gwluuhtkf.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gthegydcx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gsxpocagc.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghxqzbvpv.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gqtprhmso.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/giwoqqfrg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/ghqefjnbr.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/govsfbkvv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gslytfjko.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gusbowdgc.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/goiebwvce.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcuoehyhl.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gfptcpssm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gslsgedkb.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcybanwoa.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gltfaitcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gmjczilsc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/grcamxyzu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/grbynbdmd.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gjgvofjmf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/ghbjouneb.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gqomkqoac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gcexuyqhd.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/guwoldzpr.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gwjvxbufz.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gqqkvxeze.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gaqwabsnq.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gvyfosoyh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gebeardxu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gvsnsvwto.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gqwpquagy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gzdkaixck.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gqhnwmfsj.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gziccremb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/ghvmwxnvh.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gpwqkptai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/glwnjfkzc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gnjkfbydo.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gtacnvmwt.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gybxtwxzo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gatfdlums.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gqptetphr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/grojdlcdd.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gcvfafrkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gjwhdwpsm.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gohkwormx.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gugwuboqm.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gouenvfvc.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gscavrxdj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvnwlfuus.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gbemytvgs.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gfjzecwlf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gkkfsbxpp.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/giqxgiuyo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gonevaztw.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/glwdiheon.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gudkrdywt.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gbkqqhqzh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/ggpuwjklo.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gxegecvdl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/ghzwyjnyb.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghpwiccwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gnuaixoaw.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/goreucgpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gxnjecbbt.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gdrbxciuh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/geaqbrmgg.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gehywdpzd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/ggviqvkat.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gcdbbwvbt.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/geqtoutxv.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gjlwqmcfn.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gnnnrujhg.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/grfytxdvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gidreiqqa.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gkqztekna.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/guuamxuxr.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gsybvxedt.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gxthbvlar.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsdacuukn.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gmmghtukf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/ghobtcfmt.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gblomuvhf.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gdsoldfol.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gsayfmoty.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggglubiil.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gdlhvocro.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqxamoqhj.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gbphjggng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gaffwkaue.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gtcijlujz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guzoklaiu.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gdzqdmutd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gobuhilvr.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gwyrpulsc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gdqxikcku.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/ghsdwatwt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gkyrnhlnp.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/ghkzcuwsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gmucvsmyd.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gjsxyphst.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gnnxyxwho.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gcdgivxmq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gtczapkcc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gwentcvbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/glcrjljin.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gqcnegcwv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdjxxhdky.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gjemwxvmm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gyryomjhs.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gppjnojqp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gvdcaumti.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gsaqgbsmq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/geozyadnh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzrwfpkft.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/groaqqttn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gnrrauxxq.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gbibnbjpd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gjtmtbzwf.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gxbgkmblu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/grxofzyvc.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gsnxsgose.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gbzqewpwb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gdhjrdhrj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gspraztac.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gojuhpxku.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/grudkvtqz.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gzkwkoezp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvpchzyll.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gcuvokuij.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/ggmlpduxf.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gmyccpruy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/grknylksd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gpvzjktzk.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gkgruzfmf.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/ggazlcroi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gldtotlbf.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gxyzlxwkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gakcleits.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gubwielqy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gnjvawtde.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grkvsjsry.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gzyytzqge.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqkkpcvzu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyfezrxdk.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gsyigsgcv.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gqmqzuwrz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gqfkdqhar.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gidhdqtfq.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gmbawhbia.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gssxpkyjm.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gyvuzbkqb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gwhotpjjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gsqdhmnyv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/grvhjdnfj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gepagyjql.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gfsszgmga.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gipjyeorh.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gjgoaeoas.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gikuyjoev.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gehenxutf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gzvgonyac.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gliawxorw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gtauswexu.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/glvjqcpej.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gvclnafjn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gcyunwfoe.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/ggvjluwlx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gdgmvmtrt.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gxkznavtz.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gcyevsxud.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gtyytkrol.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gxivevjyb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gmttblzts.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gafhqvdxt.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gdevysgmg.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gghpzudto.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gelbqtfxq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gisobkzhs.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gbckzfnaq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gaqqximoj.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gxkhhprca.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gjcbyvhzo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdvbxsmwb.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gigoqjfuw.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gxcvctfcf.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gwgqwoiyp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gjlbroqpl.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gdhywjtnm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gzjvxwtvf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gvleyurmw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxcqqvszq.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gbblogjbu.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gttdxrnja.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gxzqqhara.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/grlwfcdbx.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gggmkkzhy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gfphghwbb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwsvmsu.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/ghqtfwlqs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gfooxtjft.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gajsdilfe.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gahubnxnm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvobubpwe.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gowgtjcgn.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gmdyhlkli.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gqhpcfsnq.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gckgeuslc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gwcgjdxrc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gzumtbrye.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gbcrfdmio.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gilftooea.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/guaqfifkk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gdvlwxgqp.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gjtbxawqc.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gdiahbnfh.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/groykfdup.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/goouuvuzg.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/ghaqesckr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gojqqsdve.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/glypiqlwz.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/grrvqxnrj.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gffbrefnr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gnmowqhow.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gpgnzlaea.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/ghhlunnpo.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gxrmpckfw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gxxkhmyvc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gvimyvwwf.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/ghowcbqxg.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/grwgydsvi.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gvhodlams.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gpzsspnje.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gzxqxpcty.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/glqcsodqb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gtsqwiomu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gsvqsjcct.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gmiycxlxr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gkjeikstm.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gtlbkcrkw.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gvfcspbwb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbpbrhasn.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/guvmbgchq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gyousoevr.sHtML


<!-- 参考信息 -->