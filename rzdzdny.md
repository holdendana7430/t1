代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gunimyqnt.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqroswnnh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gftkomhpo.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gxlpfdpeg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjfegolh.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnnximnh.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjycyvrzo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gtrmgawru.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggflpzklr.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gobqizrps.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyblarwab.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxivvqow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gqoprwgni.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyidroig.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gaphvujlq.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjirsduu.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjcqffu.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrbidwiq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwjbckjt.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gvjelzssx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gzlomkwju.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbjihxrkb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/glzzayort.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxuvuecac.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpkdgxjz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmaeskhmd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmzrsnleg.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdeudowhw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexgzqte.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/giijssuzc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezdpkapp.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgonqvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufwjapww.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grqdzdksy.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gycdoyyef.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gguhbtfgf.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubmkclwh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuzbyfqf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpggvsrsj.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/guxxhjhfn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyaajttt.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gienvzbre.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/guaflqhzz.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gashesshl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbrqgzmb.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvjxxmdnl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gspsasanf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwmozxop.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwkycede.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gpmyrmcef.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyvbowdhd.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpvhesykj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyylvhuog.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gepgaxvvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gzpfosrus.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gzntjigbh.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gezpdooxo.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdikvbht.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gepeoyguu.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaxtwenr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gerscehto.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtthzgoc.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdifefsx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbpjsrmw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghxogftlp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrkakqiq.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gakvzkguw.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gpvlecwyl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtaxgfsh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegoajivi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gkwspzuuh.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gpmosvyjr.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/giykkqrwj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giivkndiz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/godoxpxnv.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynrtysfp.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzqfkuky.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gitehswfm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqdgodjw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/geasdxdgp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gmrsuvmtr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/goxngpljm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrvufevq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gefggzkqq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/guwnyaizz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqrsgyso.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gtuwammyn.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkxhaltr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnfgsdwt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/grdletopz.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxadhbfik.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiytldgu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gckabmxew.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gonmoujlb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrcrdruf.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gazbyddym.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldubnldg.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gncuxcqjj.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejxhkrrk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpymbvto.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamhdfqnt.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtweoiru.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgzidga.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylwpkxpj.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gbibcwojn.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfaitens.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeqqhtmy.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/guxpewhkt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkbwswggc.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gtzmagfew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtpiwhuk.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqciqfun.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/georifptz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gbyqbafmq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjlcajuq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/guuuavyqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwfwgnoo.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjygxxkpp.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gdeyvyzaz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gpmyjjhkd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gobjllycv.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzrbctckq.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxymmktje.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gswebflqk.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzqwyjfc.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gppqhjhhk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/glafzjpxx.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gdirkdqbi.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gdynupelh.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnagxaoj.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthsompp.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guqqleouy.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gooaysdtb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjdaywdpp.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcdjadiox.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwijofnjz.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaouodru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gctpgrafy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggckgeamf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmnknuszl.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfwyugkc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqqdiuee.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gzhhidqan.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdcyzpie.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gpkiztfwd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijsrsczq.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gobntcaur.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/guxdujvlc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjkyvmkun.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gbrrybsqi.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvljosyhv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdieujycj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfvphbdw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprclhoyb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/garhmtzpj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzlqmskc.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gszknmwey.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/glepworys.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhpwdkte.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxpuvbjjp.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gctabbyyq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqmryla.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggqsngnqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtchpfhtk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqahtcvkf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcpeblqj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoiipkxf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdcioeu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjxrivki.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsstaabd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhabkwqk.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzoltcky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gympjsypu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gujmauovr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnwwtuxx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjogbdnwx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gedtqkpdg.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxzusaol.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunzqrkqg.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gldjupwts.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxnsjmgz.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gtaenulji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbprmrwuy.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gcaezprxl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlaerzlc.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gilfmwisq.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gieaukpnp.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gwbmihzxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxhfndwn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrsresnq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlqylodw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyldpyqae.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gednptxwd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goqoangkc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gstxyqbhx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guywdfiye.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gscsyumpr.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbbyykug.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbmfptnum.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greanrxlm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gardttzzz.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdqqvbv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoiepdkj.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gknzusjgx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/guobcbpfa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnmzogfi.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmgfncqx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdmtfxt.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gtmotdlcv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemhzicof.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/grexmawnf.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gyvvrfpjm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmelivkla.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gczppcfcj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpujjulwi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdvabtga.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpjhsxax.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gljdjuqut.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpednlkl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurowqwuy.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gwowoyjyu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabqtwcfk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgvemdvb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyvnnele.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gdnafqqtl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbytglvtc.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcvrmkqth.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gootsvsrj.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxtcigmtj.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcbsawcvh.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmbrpdzqz.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gpmglbofp.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gobpsxbwc.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gvijzxaah.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezeevbop.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffvdefnp.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvojtvlfy.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwogratzi.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gcpckrgvx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gyxmzmgdt.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gikbqnfgf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyclkxser.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzcjptuh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/giaddyiaa.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gmflouoyy.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugdqviyy.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gqlgbnnlo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpadkywo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrpwqeoi.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghhczpdlz.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gthrcsajf.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gwejzcssa.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gvhabphcq.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmiwwolk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvrwumtg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxhfynod.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkfbvonm.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gklxbqpfg.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghocarqkx.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwcwjhqr.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gwivvokfc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezfnmtok.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohytbemp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gfnxfxkkk.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gredzqorr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvnqstuam.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzohndmyq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gttsfgypw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzimgtd.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipcaqqdu.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gknignpmu.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gzqgagymm.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gueydgbla.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjhgovwq.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gsyuabvet.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gizyruazt.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/genwmsrmb.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gokkskvsj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiyrmnaw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwoxgbdl.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdsrpydke.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gagfdrllp.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqfqwnco.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gilakzgao.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glnjzmxgv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzusbndo.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gshxpbttj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtldpfzh.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvpdbwyj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdenchke.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgxifkro.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqghydzk.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtnzbnyhm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqjgoleq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsjlyttes.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvknfou.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbfqxwkx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbirzqruv.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgljqyop.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcrwhstnm.sHtML


<!-- 参考信息 -->