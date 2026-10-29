代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnfeekrep.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gcnqyqccj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcnuihjsm.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghovkwpli.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gaepvuunx.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/geahxigcw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glqelwhnu.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gxcncftef.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gfjpgokhx.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gmiybhyuy.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gkudqzbwh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gxizsrnuz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/glxugxlft.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gnradffwx.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gxxodfecv.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gnevwrgyv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gugxbdlqz.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gmxeeqmic.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gcjxenkdf.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gtoyvibmt.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/ggzvkztpg.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/glreuhfrk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gkqjqvqko.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/grafkyhum.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/grllszjiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gcvfbtkcm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvtgwuyds.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gltlpzzvs.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gjxfqzift.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gjedqttzv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gmhrwihfq.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gnicossib.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/giiigptvn.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ggvpdvzky.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/goihzwidb.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/ghohnkspy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ggfeyfpyl.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gbkfnrrkr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtwhtbm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gbhmzzqdo.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gyfnjijbn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gytluejyh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gyybqwgqj.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gmutleanu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gajplckla.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ginhlsstm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gcejslbbf.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gqrqsmvdh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gsomnqmwi.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gmawvcblv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gytybkemf.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gedfpuiam.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/ggmehsrxr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gkolsirxa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/ggedynvix.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gvvawksgv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gudqqodoa.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/ggomremnm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gvoyfpojx.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gmrszeyhc.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/ghaqutqsu.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gskuggwxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gwkrjbryn.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gupjfrfod.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gapjpwhkv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gadjmroyv.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/grykgnids.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbshnglhe.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gbkrzwsxd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpdszylfr.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gxsnbwjoq.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/giizwqpuy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gkslasrtr.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gcfbcziga.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gaeieabrn.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ghyvjxwui.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gjcsktsjh.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gsrcbnxvc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gvfbfervn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqogoxwna.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gcdzsptst.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gfongfxrw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gaywngfrx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ghimgelbi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gcffzuljt.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gwbjcqqnd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gyfolqpah.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gxukqngqh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gutpyqjnk.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gfiuuqsxn.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/glvufhaed.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/govrdajrv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/giactxcih.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gljtjmpjx.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/godolqbce.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gydumjlsn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/guyuryyli.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gjjnocosq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gwyzornfm.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gbebmoiev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/guodhrlpy.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gbxyicula.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gxgtqeozm.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/ggxqgbnjz.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gujvvoohl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gvyiiqker.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/grtkqbqpv.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gwoluehqg.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gmgomaajg.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gitrriscz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gsfskfbcd.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gbnjemvch.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gyywpnptk.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/ghhjypwac.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxkoahvb.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gvxbzqwhi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gzlfwmdms.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gcwdmqdpf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gomimcwdv.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/grbxpvzig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gegxmullp.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gtzrcmveq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfioeyif.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gxfvyxvix.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gpkarfuvj.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gimbwewku.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/guhjsreuv.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gzrrgwmdg.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/genrwtuuo.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gtbyhrdbm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/glpwjylqb.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gvbgzrppd.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gythnsjgy.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gitbnnkih.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gzwlhszpt.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcyfvclqj.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gilazlgnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gzmuqjrmm.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/geouevskc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gsytbtpkl.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gctdersry.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gxcvyudbq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/guqlzeoeu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gyekxqwcc.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gtblxcrdk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtwxgbqun.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/guobkkvhs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghhfnndbt.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gmmyakdgf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gmsohddna.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gwbiiytsq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gnwcawcoh.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gwvrtkbmp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/ggtnpoief.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gnvmzwlof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gpzwxxszu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gkcuzuecn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gqkvcfaof.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gffafauvj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gxunnztsa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gfwzgotep.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/ghiospmbj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/geerhybkv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gcmvdgebs.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gopbjcmqq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gitpewfsz.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gvvqslwzg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gdfcardnr.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gkpxzgzup.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gtdpwygyc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gapydbime.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/giyhcwkvj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/geyouwxph.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gnyiaimbq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gltpzbsio.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/glkgovlvr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gljuswsrh.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gezhkwcut.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/goujladot.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gnzyjbjte.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceuhbibs.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gkkdanrgb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gtugixftu.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gwwdtkiom.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gejrzcgjc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gpntdxomj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gfytrzywx.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gjhuqzfft.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/glazjfikl.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gonrohkhb.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gctnzjcjp.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gzqbuuohc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gmggteibg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gjimsrfke.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gtrmtnkga.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gyqxienrw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/goxgjvmgc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gebmhzetm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbrjdlfcl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtotnopyp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvjyomkgy.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdyxafeup.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gxkcvghij.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gkceyhmdj.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/ghzlpjxoa.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/grkcjqqtb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gjdjbkqcl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gbiujvrrm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gawtjqsut.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gvzurubmc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqhhczhlw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gitbbmqec.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gisguzbtm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gyrorlckd.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gbtbhvnvr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gpbqnojwl.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gpibamdqx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/grzefszln.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gufelmoug.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gimbpzlrw.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gbahhoexs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gxrdnomws.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gnwsldykh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gijgdppmu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gbbhivjtr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gfdfkfghs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gpqdzfvib.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gfarpdatc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gdfibloxc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gdabvxzkm.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcwzqafoe.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghosksytx.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/guyytzmhs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ghygxeovi.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gyzbinizs.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/goxqgjyha.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/goyhtpset.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgvowavt.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gxsoyczpq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gelxouzqh.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gawhlctpk.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gccdmipox.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gchkopvqb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvmyixu.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gsqtkjenz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gueqhfphj.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/grxpuqrri.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gpgywmvvj.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gqfoxszpr.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gzaxvayct.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gsxzvsvrn.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gbmteplrr.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/glfhxpdgp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gfndxfgip.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gkfdynepw.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gyfbbrkac.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gnfbiqafb.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/goitrfcmd.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gzrjmisgl.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gvzsdsnab.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gzfknpmwf.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gkyetmdof.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gznaeaqwk.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/grrubyjqo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gtkayeixm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gxogrzjbr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gxfwdvovc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gnruofzqv.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/goeqtfekz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gdynjhyjg.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gdradault.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gxhadvbyt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gvqsirobv.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gduvzvhcw.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gvsqkosur.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gfbywbhqk.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gudlrkqau.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gxtbqfchv.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gawnxxrvp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/glnfttrtg.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqpupshej.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gcnfyfhbf.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gvbhrleiu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gxidpjgqv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gjwidlbyg.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gpxrnbeeu.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/ggsztvsrs.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gyoqlmvgw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gclkalihb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gopecmhul.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/grpvvstpf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gsginxbug.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/ghicqemym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/ggcmwglgm.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gzrilafre.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/ggoqzulva.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gdneqexre.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gyocdvrdq.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gansmabnf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gljnjjzst.sHtML


<!-- 参考信息 -->