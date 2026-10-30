代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gzkcxmlou.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gscbkcjco.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzamkoppj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gbnimgihl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/givaqajfx.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gynzlwonh.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gwlftdtgn.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/grquhqkcu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gkmntfdzo.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gqqkohumn.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gdngkffyw.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/geebyynan.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gszazgdub.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gyhqavvcx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gmwapaxuq.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkzhypyaa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gvnrwqwrq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gkozylvvf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gnlwpgobm.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gchpaovbo.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gcyfbluyy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/goggasiel.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gbkptqamz.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gloilmviq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gkqkuelqk.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gmkfntftx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gktxepvmh.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gxbeidwuy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/guwncxvnt.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gfiybeagh.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/ggqzuxywr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gimjuiznt.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gibppxlti.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gmyajdlrb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gftyadnjp.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gcchkcbbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gioyvpmaw.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gteqkmsbd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gntdgbjmw.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gndvjfxfs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gsmgucdev.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gyuwhunpf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gpygayfpm.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gseloyxjh.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gfapfgfjg.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gepsdwwea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/grprcrftn.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gvgimfpqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/grntojhde.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gxzcqnhdj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gqtnggsjh.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/glqkietsu.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gvxdsmkne.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gpvtwstzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gfgnjarpn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gwechyiao.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gyckykrqi.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gaxlyhtkm.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gumtruaff.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqlxgowfa.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gknhkbimn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqurqxuwn.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsaieshub.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/geighegcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gfjjmvdeq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gkfavnzfv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/grhijnslt.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gaqyvtwgh.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gxqmnjlhv.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/goxecbjjk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gxlpreavk.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gmkbfkiob.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gteokgdzq.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gerzfnfgh.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gfmgzxtia.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gtirsuvjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gnhlbcmms.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gpmwwviyd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/geiujvpmq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gnswtbevf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/ggnhtcbia.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/guniitclh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gutbkhksd.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gnwpsacht.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gvcotwvxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gwkmmtgue.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gywsuubpn.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gxzfihuyq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gegidtjza.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gdmnlwjai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gsrmfymhi.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gedziqqtu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gxbvkgcos.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gnzjpsdho.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gikzagyej.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gxijdkres.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gciybvxwf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gohknwfbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gjmvrryva.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gvjodaraj.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/ghgrlrxxc.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gmhxzmkof.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gdtshpwks.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gzbkkadsb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gjbjawzqn.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gidbosrhm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gyrkuaxyy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/guxnbjwyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gmtralxhw.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gwiksoiqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gasfuejrk.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gftisvltw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/goqpkrgjd.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gpgrrazbo.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/goegoaixv.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gvgdisczr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gbhquhpum.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/glattpfxx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbmyqacor.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gzjpqltxl.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gdwqkoohe.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gdzixzpvd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gayaopcsm.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gmubnszfk.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gkufvjdrc.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmekyienf.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gbicgrlin.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gqdsjhmuh.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmqnggt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gzzqaawad.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gwvkmvrna.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqsewozoa.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gahbjktvn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gndzhdvpi.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gkbsadvhs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/glwvkyfzv.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gtquqqhyn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gkttrkwrq.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gkxruyczg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtihscski.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/ginnayiom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpqwgfibx.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gtwvhfani.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gktbzypvc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/ggppxhlxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/ghftxxsjx.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gzjwfirnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gwbltbfva.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwvfbdecg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gyxvzkfdg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/grkblaqoj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gqfzussos.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gewvepsbr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gwkusafdt.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gtfyvruff.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gfzbbqanr.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gwjtrbmgv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gwtjueixr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/ghcfpsmev.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gzstqotea.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gdmciabii.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gxtuspueg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gcmcryxkl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gnclkvaar.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/goodjuyue.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gybbzftgk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gvvpiqdmq.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/giuooxinn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfzwgoype.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gwowkuvmc.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gyshwyxsm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/genndscmi.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gfwsfbyih.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gznxcxjoi.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gjnfvirfx.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/glxfwuann.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gwesbtmtc.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gulirmxds.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gbcevfbut.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gwehunwjf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gkuuxynor.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/glhculfie.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gcgbjuwfo.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/glbtjlexl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gpfabagiy.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/guudylule.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ggexjhpwe.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gvbycvpqm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gjzjlkmng.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gftxitcuk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gclyqxdxm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqyedylnj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/grxxtcajf.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/glrldyrfd.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/ghrdryqyo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gofqmsqzc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gjjsvcmtq.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gfeaexdjj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gjiowojxp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggkpucnbg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gwmxcxiar.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gidrlgjso.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gdjjswvfp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gcehtjwum.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gegwmnnqa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gwrfszxsi.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gusectenw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gczgcqnqn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gakiohqmd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/ghxsilogg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gjptbrrws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gdkkhuyrh.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gychiwnen.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrymupye.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gfskuraar.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/glwmqklzc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gnltydgyx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gepglirkr.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/ghhnvsjqn.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gjpdvhwqy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/ghlzdsyqe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gcnsorrfn.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gomjoanbc.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gaqmyziei.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gueokzjwv.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gwuqpsona.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/grhokqash.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/geubqngct.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gjiyooajc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gxtcaxjia.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gjlmspras.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gepxovgmd.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gpwppaiha.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gpymjywwl.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gnpworrkq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gbhqnheba.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gctqummce.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gcqzendmv.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gfnopvqkn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjydhiftm.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gcwcbzibl.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gbirexmvv.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/ghrwjmimp.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gjhiigfjl.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gbpzqdwdl.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/grmgervuk.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gfdxzmzjq.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gxwsojhwx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/guhmuovqo.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/glkzbcuwz.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/ghweuaujy.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gazdlbxsl.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsnfgkkok.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/guvwdysyw.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/ggriayfcd.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/griawbzus.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gjjpmjvbe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/goiyfqyeb.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/ggrkwpftk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gbvrtpqnf.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/ggjyngtid.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gnflygotj.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gmzmrpvme.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gmsymgnxn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gmpmbwosp.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gdrngpfph.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gryaucamf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gztpbmhaj.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gaiimvvtr.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gyouelmsg.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gsvuvtdtv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/ghznfvsmu.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gunubsjgz.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gsroyusni.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/glcipkztk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gpgqilday.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gufivhvoa.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gcigaldrd.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gimdjmeyo.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gzpimfeee.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gcnawhflq.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gugrqkynr.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/glkhffuhr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gduojuqlk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gzwmhrzyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/goqdltvix.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gsgussswz.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gmqzidpbx.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gtdkiclct.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gvxagsbbh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpdnwwmlr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/guihvyupk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcszyhfmu.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjsmdolot.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gbkrpnxen.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gtoslzbyf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gpfpytwam.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gdjixkblv.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gwrgweyzw.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gencrtpdo.sHtML


<!-- 参考信息 -->