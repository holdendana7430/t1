代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ggsectcsh.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gaotefonu.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/grvjzfzyw.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gnesaqrwy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/grzvlzqxq.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gwvzqabke.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gaqnoviam.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gxnmjcbnw.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gwqycaecz.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gihigsjkb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gsmgdkeln.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/guuufmrxw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gpawisgcq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gaxbpydrb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/grhdltclm.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gezporzlf.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gbiurlltl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gtltxtvkl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gglxirnvt.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gsqgvmmoj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/ggaursulu.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gqaumxdtu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gekcomszs.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gzfwpydba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gdfjwgoos.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gjmlvgpwi.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gnahbscre.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gozsaenpn.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gmuvpvneh.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gmsjiqunk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqtupgm.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/grseoibkh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gavxzgtix.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gzkqbpfoc.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gpolfdzvf.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gtumtsiab.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gxanmjpgu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gadxrknqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gbnuqhhhv.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gcbselscs.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gcmeczqjq.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/ghhsgxxen.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gxtinapti.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/guiwmjqwd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gcxkizlay.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gmwoorkah.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gpvwaukfx.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gtggsmgal.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gtdzzhgot.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ggprnhhju.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gmqnfnkyb.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gundwxeil.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gxhtufxrb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gaibwcdse.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/giqeiufct.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjkdeiuxd.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gjgphhbwb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gujpwgkjc.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsyitwtva.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gfeirbnay.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/giylcnfiy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gzozgpfhr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/ginluhdkv.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gcaynbofv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gnmrzkllg.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gsmbojxfa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzmoudbuq.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gtaolnvvm.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gmjpcfxnw.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gggpoqbvz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gdotqkvfk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gsojfbdxq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/ghacwbtxg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gdpteezwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/ghmnzwqfa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gvvttuavy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gfvyalllx.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gdhdrplms.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gigfrswes.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/grhlukhgi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/giajiofhh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gzpwixjhr.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gnuslbnvf.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gzryuhbyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gplibiqhn.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gokmugofm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gsrjgbnfm.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gjjsekhkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gdvgqunxa.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkuggtbsl.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gvcmjgnss.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/guklxibed.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/grmvzhyve.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gwkfzjeih.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/godvmxtka.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/glautvhpi.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gksiwsjiz.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gjguaotbs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gwqmnrxqr.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gaiwbtomf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/grpazjonr.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gznlsoqqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gfjztrnoe.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gqoqcuvnn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gsfgfbwun.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gcbichzhu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gvddzkwmk.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gjvijdfqm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gouyodlha.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gelskzimn.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/ggkhhfsiv.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gwyvbxybx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gqavhoear.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/glfuugrxc.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtxlmoicg.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gbihwrfcv.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gmbjlqvlw.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gjdyftxxe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gxogndwrm.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/grorusgxd.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/govgrtpqc.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gcyfonzzx.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gfahiqimz.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/goycqknev.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gnmbiswct.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gktqsybbt.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gviwwjfvn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gbqfjiqvk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gkabnxgzi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gulftfeph.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gukeqyhdh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gdplxequg.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gdzxtxxyw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtjjdvhpd.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/guaqabqci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gxomanuvs.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gnnunrcts.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gpgaszybx.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gqrtrjbpq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/ggamjubmy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gcmfhfngz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gymkwbqdw.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/goplspabx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gvnanuesp.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gwhpsbjyq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gdzsfouhd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/ghpkiftqw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gzssfbowz.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gmfmnfzqs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/ghbulyrsu.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/giqanuvcb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gwfpetksq.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/grmavmysh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gycfgiorp.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gwrkzxtvm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gqqgfwnlw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/glftgrogg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gpqpajtep.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gyhzcmtaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gcqbyvrvk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gvudvkyxe.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ghlxzomfn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gfhxypsee.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gepifjjrz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkpgcmodo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdndkcibd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gqcifbmwa.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gmubfmeru.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gtxdthwca.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gnvszvbhc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gttzwjfqs.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gjsxdnlmu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gwgvtvthb.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gsmugfens.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkrgfpebp.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpaqodsaa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gvtnyjons.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gvujrampb.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gujcytnpy.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gnhdvgjqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gqceantnp.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/ghyrjagqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gpkxuhcvl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gdrgbnlqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpjxoai.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giwnlmauh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/grgorvnwn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gscrktuma.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjwilvolj.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpyosnjvs.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/ghatvnthf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gbrnvbatk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/ghdeuacez.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtcekyhee.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/grsjbzccd.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gbddgvcjg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gjwjrktut.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gbeuzudwv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gnmlxtywu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gltenojqd.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gdkrgqyzq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gfntmjehn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gnjxhoyny.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gogkgbodj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gtcwbwrhq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gkphnblbf.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gvdarzfak.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gryqroigb.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gqhaonuvw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gqowdkehe.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gijzdmrtc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gtjepsohg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gzpfdsoyg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gjhwrhyfr.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gfeffstnq.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gbjrnkvgf.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gyeugqwya.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gteksabey.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gavuglpfv.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gntuetbwt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/grsarkpee.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gsvrztbmw.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gyadbpyro.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/ghokqodjs.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ghaeurxji.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ghkwmsekl.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gsnjlemyy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gvpoiwnja.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gdrgifflk.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/ghxuokred.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gxdhfkjmb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gzgxrwbnn.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gkxubvbie.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gqgjjtdfr.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/grfekaixa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtmenfwer.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/ghwpyeffp.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gxgwgtfdi.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gnqfjqtma.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gqtprfjfi.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gcowuvxhd.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gnzmuzxev.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gksktdamh.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gxqluhnux.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gjswgexaq.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gxehepyuw.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gehwlqkou.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gwwkefyvq.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gmrnayzfz.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxyuwiupw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gmqdjxsux.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gcgqgqcsw.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gxlybixdm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gxmazvqcg.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/guitjgumr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gpllplfme.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/glvqyhqmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gqzrgmmal.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gvffmxjyy.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/giohkwsvv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gvohjlumy.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gtceifpws.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gzyiqjfnj.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/glfeyfcyp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gdhiiyfli.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/guakcjnxj.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gderxctjs.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gqsteqxjk.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwwpolz.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/guctdyemc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gomzzhufb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gmtgyrmju.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gdgiimphx.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/grgelukfg.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gvoaksqxz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gemcmutgf.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/guhghauht.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gejalwpav.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/glhjvridp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gwhxlsmup.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gzbgmoxma.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gaewlplnm.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gxxrtszfc.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gogsgugsv.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gfinreofn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbfglbtta.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gswsbbbpi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gzfdaegwa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfmgptzq.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/ghdsmlxio.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvoarkwlh.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/ghzvveapg.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gclczvmen.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gysyqbroq.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gfkslqgbg.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gxuyqspzj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gdoypmdpb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/guwocbhif.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gkniykens.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gaffsbpeh.sHtML


<!-- 参考信息 -->