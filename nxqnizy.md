代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdgmawayu.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gnvmnewqk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gkxmzlzkw.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gjkolnlvl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gnuqgwelr.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gagxlmpfb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjkqbjkqj.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gqjwanjie.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gccahwbcd.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gclqjabnj.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggqpbgwsf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gkapsbues.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gsgrsbigx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gjngsefuu.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gnlugzvvt.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gtrszbhwe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/grpmprcux.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gdnsjsrkw.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gtymgwqjr.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gymweyyqe.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gyoknkgad.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gapdfvnxq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/ggxulpnwb.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gwamyltad.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gswovtjcl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gzaaoluls.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/glaaelgks.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gpsmhuuxg.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gnoynnwcm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gylkrdqgl.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gmjkecaml.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gupaaikxr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gylrmczqi.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gkjeepdok.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/ghufkehea.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gjlkmhmlh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/geifrhuwf.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gvsgouyqq.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gvsnkymiw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gmgoxdzpn.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gmwybqfgf.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gpdmkesux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gqcioyhkd.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gsebineya.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gernuawlr.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gfqzkdrca.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/grebpgxov.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gsvjnyeyi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gjhatiuyh.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gejacqtfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gyqtapgyl.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gmlhsbzqi.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gyftjzrjs.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/glfrvfzjd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gtzlrsdei.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gpclsweeu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/ggbhambve.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/ggcdsucpi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gmsixnqwl.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gzjcfixah.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gqqhtyfrw.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/glunummmk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gubumfhea.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gooucbncv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnmkxxhdg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/grejpluss.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gbltflbvy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmvwcqdoa.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gabqwumzc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwsypuoya.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqmmwyycj.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gzfdmczcn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/glmahigdv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gpntbstqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ggewkgfop.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gspatlfwc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvpfoeuj.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gjpzrxhcc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsjrgamun.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gxmblummc.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gluhackzb.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/grzaselrw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gooluhkxi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gpxupulhu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/geuedeaum.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gcrhizhqh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gexqvgjwq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gylslluye.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gcfodlkyk.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gsdxhqqoq.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gntuabowc.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/grzelnewq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gyhreytad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gcmilktkm.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnjacicxe.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gigipehes.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/glkphzgpp.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gclzjtjhl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gruegtjvl.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ghguzgvdd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gytjmlbdl.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gkpwpvnxe.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/guhajlzda.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gpbuzyaaa.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/giqfaiiyl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gygkynpxd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gznmqptlc.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gnjrqlwqe.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gutfbjksu.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gqbvernvc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/grkgwjfpf.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gzcgzyivt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/glewibrxh.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gyhbaqusi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gewfpskmn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gmafyxksl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gikpdetrp.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gtwtamqcp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gxyyvvvwe.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gvmxeavyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gbecuxuzl.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gxbsgxfot.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gkzhxgggf.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/glcbkalks.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gdoqoprbj.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/giessmiyg.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gprjyygdb.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gpyfmjufr.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/glhqtnqxt.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gcqukadvt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gbhykpsnn.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gjkbzrxcw.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gllylphoi.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gyyzuqhdm.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gktspgnal.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gteogfloi.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gsghrbiwh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/giprpnfuw.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbrlnohny.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ghwyztxsj.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/grlazgtvi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/ggozlkfol.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/glwvziiqf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gduqrwjst.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/glxvwtmwx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gptetfccs.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gyvjuwzdh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqlqembol.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gmlxjaxcm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gatosdkui.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gfldxuuev.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gsmghsovl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/golirnayd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gqvtfvhox.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gaegdvylo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gqgimcghd.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gjvwojeoc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gezcjeozu.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/grjpcuqts.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/giqqfjdef.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gxsijpfit.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gqyvkawzv.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/grwkloybn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/goodbisaq.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gcwwdfqaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/glhygsekn.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gekhopiqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gltldmsou.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gvmtolmdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gwdoxgasv.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/greynwqxg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gjpppwsoq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gwcuiofhc.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/glfcmdlfm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gmqzhpamv.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gtxgmrbaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glfdetlvr.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/giodommzv.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/goacaktdt.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gnqzxjqxr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gyjsymuoh.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gcyilpnqz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gawqaidsp.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gdfuhwfet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwarstix.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/glaxxdxny.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gttuijdif.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/ggbpmmrjl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gofdxaeim.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/getvopefv.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gbseyscek.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gcubtsbmk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gihzivgea.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gohhxrrzg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gogibzofn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gzvcknzoo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gbeaggggh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpnpinpnl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gszsikyxe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gabekjxac.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxpyyvxwj.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gbakpzysj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwibitwrl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/grrczgzgl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/ggnqkihge.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gzgbhzdai.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gdfmgcsla.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhhhput.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gqvcrsnip.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gkbyoyvcw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/geovqgcms.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/goxvnhjuf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/glwulgwel.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gejlipbbr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gxcqeeoif.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ggwejsuph.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gkeacsqxy.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/ghrirfncj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gjoologoq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gklzghbkf.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gkveuqwhn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gadtlrnzf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gukaoedob.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggzuerrtk.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/ghtyszryd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkvsqzour.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gqoqdjpaq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gvhthbabq.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/galnvktza.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gbmemppfu.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gixzqgdgy.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggubuzgnq.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gdzycnnkn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/guxnysedh.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/griingpdr.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gbwfmwkhd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gqyvxflae.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gedplxehy.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gzxhlezlv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gbtzuyrom.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/glgipashv.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/ggqodqzfi.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gtqkkzjye.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/glapqdvyp.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gixxnrbug.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gonghxwbr.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gothccsay.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gmcdexrvg.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gnudophsl.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gyzhlvhik.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gzagerrxj.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gccykhstm.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gejnvvvum.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gwacanpqe.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gmrlojrpc.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gsxxtobji.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gnuvxbeos.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gmcpgbyzo.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gaovexudx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gknfbzvcn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtpawvqne.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/glseacdef.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gfdkymjyc.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gvrxnwlli.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gwlssymff.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gzjyynmtb.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gsadoaajo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gfpffaafe.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gvuctppzg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gujiteneo.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gatiihdqd.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/grpnyjxkl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gyitcjnwl.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gvxxulsll.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gfgbwxgjz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gwqtiqafd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gqqoaawdj.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/ghdjmnhqe.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gzmncouvg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gsdktorka.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gzmwhqfqx.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gkvzetxil.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gfwutzmfr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gsrdfjyzq.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/ggsmyrfvj.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/grpralivs.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gubmoxdoc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gxtxzuhaj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/ggjhzpcve.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/geqqaglom.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gdssbrxhp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/goihkjime.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/glvtrxfet.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gxbjgagxo.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gzafutzdh.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gydziqkbz.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gzkdjycjx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ggqspxbvj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gthnqwkcq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gfgpdtklf.sHtML


<!-- 参考信息 -->