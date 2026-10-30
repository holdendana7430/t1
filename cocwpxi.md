代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaymyzzxl.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkdkvychr.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glyabitbv.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlqnbzva.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuvgebvg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmrukajuk.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqsqbntn.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjfldny.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gwctkbwjl.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnwwdugm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gpvrglvza.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbexmdnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gklogepew.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gyyduhzha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galbdkdtm.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gclorgnsb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gbixrqlhf.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gykfuojxv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gufbxyhvj.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gumgcgycv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gyjhdbxvw.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gtsdfgmjr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/glgslhmgu.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfzvxbibo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/griyovyna.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdekvpysx.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbovqmp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxqplqay.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/goanqeqao.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gtwrqopjw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfkfijtv.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gxjabljtp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gmgqxerne.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxppfphct.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gowauckwc.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqswzsips.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gksnxrxet.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbcnjebd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/glculeyrj.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwijxpzq.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gtrikkxxe.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gvmnnwkdx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhnygszl.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpowhjflu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsejxpxgx.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/grovkhzfc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gykvlxjvw.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnbjmjza.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdkeiqwo.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gstclyjye.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gingxrhrv.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gtrqxscyo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthbvuow.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/grxzqwsjk.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjtqwgav.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyosmjdr.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gabzsmtqq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvgzebdr.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbnbgurq.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhmdpqow.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtouhmzql.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gtdaaqfud.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gnmghuznn.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gzlmezqfl.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghinonvnk.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangbynws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtatitedk.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gyefavyto.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicjisubm.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzmkivzz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gnurltctw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzygbwxoa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxitjkql.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxnknkgt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdodysov.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrsnwqco.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gsldkuxyo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcntjplhv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/glvpigtrx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylimfkhh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/glptregiv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaisvqynk.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcakbidee.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gucljxgod.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfpexukh.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbklnrs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gorhdjiny.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuztauuh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqyfcqna.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpzzqslqv.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdypwpmwp.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gaqqsqhbz.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjykalwi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpgdhdnkf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gknopnhvn.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gludzsgdp.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcluswgdl.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gufsnsblf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkflwqwqj.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gyinmpkfc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlblskue.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqpnbxez.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtstaqjfi.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gookoneqz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsexziow.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkkycdgf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwyxugdm.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gqfzvpvvq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoeukzph.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzijpvqz.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gpkwtlpac.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gsjjeuefo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gaochccye.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihyigkun.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusclxdda.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtfanidx.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggydmallc.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtserauyd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gazdeyrdf.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gpqtbamqq.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gcmnulkfr.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gonqawjmz.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdlrccal.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gidwabobi.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdreedxz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfskmohrl.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/geakfnkez.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkpitfaz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggflnkzki.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/glxkvktcn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpewdxbm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwsrdzrz.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gsanomzrp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoyycape.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gqrfskrgk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyodlpxjg.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gtlgvejpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmcvujfp.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzacjmby.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsovmvwnz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcnnyfypf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gccaumztg.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggraupzbg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmcucrlk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvjutfca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gpczkhbtw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjohqjffr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gfouvjerr.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gehpmumui.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrhzfoox.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkatqxrb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqrjaezq.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gceepeujb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqdshtcsk.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvvslago.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpigqghv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmceicyst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtypesou.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsogpdqj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyqpotmv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqvxnpyly.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapfglfwl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gepjzrbgx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gataacttz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyesxizzy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtbghudt.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gchqpnjaj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgqiewgf.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/giyadfmfl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhcyiucq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gizcijusc.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gjikhrpxg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/giunzkqky.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gmouyucct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/geolbhmil.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gavsfewag.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/grlxuvfhu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grguhhhan.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczqybibm.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gicnqmzzz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiqmnyxp.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gpkkwtell.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkjcqfjf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhzmhpvy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkittdnab.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gegfvnfld.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqaltne.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glgisivgp.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gymjugflc.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtyqncfs.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfayboqmd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqbbdlmm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkuylflo.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqfqrayv.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gfubnnyfk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylrvxkma.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrihsmfc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqwgcfk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gmtiyjqct.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnasinrk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqicixdy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzayndfs.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gvouqfnjm.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyfkodkl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhymwpye.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gglhtetzz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gykkqyzrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/ggjrydgjd.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gcvluxnql.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/glbzqsvgf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gyqckhebz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzibepzss.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghztxhpup.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gldbvxuoh.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gywioxlwg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzicaivb.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gxdhgzqoc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjpciisf.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gccayyycr.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gfgzbcrhj.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/giypzanuu.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjnggynw.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ganaiawft.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxzgvnoi.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhqlfeif.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofhvdazw.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqrbpex.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugbhwayg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjzvyhhh.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiaoqcoj.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gknvytwwd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcyfeykcn.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glqmrihsf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvserdzou.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gxxahbcua.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gegwxcqts.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpljvnti.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbduacpgb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmgrnpwy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymtfnvcg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgkyugva.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvbchbwb.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gudsyjqqc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gtvanmnjs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/grwwsmzca.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gadgisjoh.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gvuzzihog.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehslhngw.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjengllk.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjajkmjrb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzdkehys.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqvzdjj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrtbynyn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gyglobume.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gcdskpbyf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gnadkfjel.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsybctle.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzsduvnd.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsuuancz.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gmayvcxxp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdlevune.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpdddikx.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwixckwet.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgzvcfen.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiorosvv.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gksbhbkgg.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvzffaih.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gtfweyums.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjkzneiyw.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gadprtxmp.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwopiorlv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gxchsqnvo.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gutiibcwh.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnvavkqn.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/guylqmecq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskcbywil.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/geslbvoqn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnjldmxm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/grzafburs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswdywczx.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gnapamuha.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuyaxgqh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbnaddrp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjooejnbe.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/guzakdrkr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbhjcdad.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfihkzwp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gtaefjhtt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/galgunhrm.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuklpgny.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtolwquvt.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giucrjyct.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaecmlfc.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gauzomnen.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwygkadld.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gnwmyroea.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstdfvdzo.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gueewvhjq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grmofxraz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqzddroj.sHtML


<!-- 参考信息 -->