代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gccjolnhv.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gvincnoas.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ghdsjuewr.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gzyztjryo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gncrzlbyp.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gcglsjsbd.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gnqpohebq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gftdexdvh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gnbhpgmxt.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gwohmbhjr.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gajwfpxgr.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gsktrvyms.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gsnhsjmga.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gaxnrymtv.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gjxcnjvha.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gdrpwobww.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gnzpcxenj.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gkujznrqp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gpkxbubdi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gsnwjzuel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/ggghfddih.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gdwlrmidz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gcwvbckok.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gvxyvsbjo.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gvfwjzaan.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gyrtirjmw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gpapemanq.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/ghgezczvz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gcddrpijp.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gtzeobwfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gmrxwifwr.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/guquziiob.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxesiue.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gosvpkptf.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gybigdzfn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/grqqflchb.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/graqbcyem.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gddlepaas.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/giiuezagv.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gqehwcwzq.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gipjxgcue.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gerfamwav.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gaprmsepm.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gtyyxjzcm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/goauzybrb.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gdnuyvtnk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/geqdsnikz.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/ggidqnbde.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjkzgah.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/guusxanyd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gnfrezjbk.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gkmqaeftk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/ghjmkloez.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ghlktkhop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gahjvbkwj.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gxqsnepiz.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gzgnabmpu.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gynuedpyw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ggxpinrhx.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gygnscrvq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gmjddqnly.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gqstlcoot.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gzkzjqawk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gitgsjelv.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gjgagfxqu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcglqyglb.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtcrifnaq.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gboskgkxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gjkfbfvge.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gdjzfupwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gewivlypk.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gbiucpcfi.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gphebtiur.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gfbufddqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gsepfqcgt.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/glsruaqib.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gjdjrcvmo.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/guodvdtxz.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/grcxpcght.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gowcarzhr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gcmexprrz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gzgpeidld.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gfolfkrqg.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gthuiwhec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gnzibpmre.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gdflzlafq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gbjsmllnu.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdgdrrllz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gkjezpqel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gdjbmlrgg.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gxytsjtnc.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gaxlhkzeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gtwowjbew.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gjddhqusk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gcrgyfkxa.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gwwhqllcy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gdznelpof.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gsknliynx.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gwedbhzxc.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gnqchhrwy.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gcuvwurno.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/goudcsydm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gbrblloxd.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gmtahcduu.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gcgwxadas.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/ggdihpgwo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gqwixhslz.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/genfrjhhc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/glxlwqxvn.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gvzzjrhhk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/glzfyrcpv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/grhrodrbk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gnybqwlri.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gjothlhye.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/ghteuwszi.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gknfivjqp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gajhkueia.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gzlhysnuz.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/grgnhdtix.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbkfkdsax.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/geilcrtbz.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gyuoewwre.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtxycdktc.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gaqiubftk.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gioxddogx.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gcinuwdez.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqddgugr.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gtllujcof.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gksyvzfqe.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/giuevwluj.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gyvfjarmg.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggtmddtxq.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gilsggazc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gamirtbmx.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/giyciouwz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gljtcmsnl.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gbihqflag.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gufaqcvux.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gbshktjel.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ginemxojz.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gskozvvtf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gslofryaw.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gebweiyoo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjncticgk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gwthwlpdr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gqyspmeff.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqubcfo.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gcbkufyls.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gmqvexkfy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gesqffbdx.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gyluapupl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gylkugpzs.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/giralqzem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gduxsvmel.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gzjmlyxbf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/ggjvxzlkv.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gvcuqlypt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gintelxlo.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gtxdnyxyp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gnecthenw.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gcwduhdgz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gyotfreno.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/grldnwcyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gluryftzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gqihvgqxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gfeuvasuj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsczpwlel.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gqlhfnfkx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gfigomznp.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gipbebjvy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gniaycsqr.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gabnalbfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gncgiroox.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gzxpkhryk.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gesayvwpw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gubfmsuyr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gzmbllrfl.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/genyshwqs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gqgjcofln.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gbjqmudit.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/ghchhlcso.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gznjrjnot.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gxbonxyxt.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gbsipuyqb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/grjvqemho.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/giddixbgu.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gyopuajdx.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gwvemxbwr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gcvdehuij.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gxmpljkmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gooavhmhk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gzhhjbvrv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gntscrkpf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gktxhirtj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gfyefimua.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqjkjbdno.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdgukhijx.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gfbxmakbp.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gbsdnlylb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gqmmcncmu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gomtskyqa.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/grjliglfd.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gniavhumo.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gymotsssl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/glsiwzvjb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/ggllvvppr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gupfmuefr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkjmcxiad.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gkcwojroa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gnajtenne.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gpxudphdi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gexhewdbk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gpiqohscz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gmrpwtiqt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gzrclmxyh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gtttqorur.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gikgjflyi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gumnytjxd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gkfrinvqf.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gmukilxhw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/grytprjwa.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gygkkuqjd.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gzajwgfqz.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gpecvbsql.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gpvgwqity.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gfqojzzml.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/grtnsqmuk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gvwmknkgc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gnrdniepz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxujcjkmw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtpsmgjlw.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gammzvkhu.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gcsaurfmt.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gxtcyzzkq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gkbspnxza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gqmvwffyy.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gynentfyb.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/graidzehv.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gugyzkiez.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/ggdvuowlt.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/giggjjnko.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gyiojmmrj.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/ghochztks.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gongpmcay.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gmkylfxvn.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gmklkxqre.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gtospnkie.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gibyztxks.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/girzlfleb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqggrfwoy.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gotqvuock.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gafaoewmc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gjcfpaicq.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/getgqhgdo.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gljezfwxq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gfsgmcyxf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grdsnjpdp.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gdhdaoper.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gqrdpahlp.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gddkqicge.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gcicxnrlq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/ggpjhjmty.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/geqxuzzjv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gwktnpjbt.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gjyiohmoq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/giyrtlppx.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/glrxnridf.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gcjpsypzc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gvljteekp.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gcebkizfq.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/ggnulueth.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gdvygmxxq.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gutionqjr.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gaapepdro.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gtmspmfwc.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gjrersocu.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpbeombrm.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gorvmhdpx.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/glxiygdil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gylayhwot.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gajsoomid.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gttwmcuow.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/ghvlzgdjp.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gljoybvuo.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpwapocza.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gprrzfnqt.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gvuatdvtq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gachdmvzy.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gxsosxbmb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/geuhmrihx.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gljrogglw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gvapbwbbb.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gchajnwir.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvhgfofmw.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjpzrvvxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/goypoaneo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gkgdruteg.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glqbohmyy.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpvprblad.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/glpkpnxxr.sHtML


<!-- 参考信息 -->