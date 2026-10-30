代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjmsvxnmd.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gmbelcoui.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gteygcqhe.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gxroduttq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gghtakwqo.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/ggpspwbil.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnypmuqmc.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gstsfiojm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gulkgsrdp.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gdxkwcepp.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gxqxowonn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/guwsyczge.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gmbsqewyn.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gtihvpjpl.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gwcuczqrb.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gcwcznuqd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gmagervkf.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gfervdgnz.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gsrgbhkdi.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gnzbcqlqu.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gdjcsrtck.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gfwlzvnng.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gsowlplzk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gsehtffer.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gdpqkcody.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gsdmzepic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gbjpsvnph.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gockbwkqm.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/grxxhsmtp.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/ganchljdj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gbrfmlbww.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/ggazulgtf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gdcvccatg.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gzuvynmdb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gjaduvvhf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gkpmhqivt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gydwaclwm.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gptsqmlsf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gjupvcyog.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ghzbodtrd.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gblqsbjzo.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gznfdvpmo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gsbkithpe.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gtwnoqwvd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gbjradged.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gtnyacvot.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gadipqrwz.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gavbmuljw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gaojntcqe.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gdlbgypdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/grkhwoqkw.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gndwibafo.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gpsxgmhoa.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gadcvoeve.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gykvhsdgi.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/ggpebeavy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gofefrlwh.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gcmjcnbaw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gqnbykcdm.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/glhzekaqf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gqcjydmza.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gioujhudx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/goslpuksi.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gkowcmxyh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gbdeuakfn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gvjjbyaxp.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/ghzwiepwz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfsdppbl.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gygshzdqj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gixclxqvr.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyrjpdgsi.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gbupqtprf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gzpdysvsu.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gzufiyvpf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gcwcoxjrf.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gmqjqrtak.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gbjaxhvos.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gqqzlufhz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gbwutllrl.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gxqsswivg.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/glmrscjky.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gwvhlsldx.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gkkxwgsem.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gizcmfeum.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gsvaksqoh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gttdkesje.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gewgoapub.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/giryvlldc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gklikxzeq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gfeybzrzo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gclqesoql.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gafrnqlft.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/ghwzqlfxe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gjhpcerbc.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/graonhjcp.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gjgvehghn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/grhumqcdf.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/grtlbwugy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gvnjafpjs.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/geslgpprf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gnuervyae.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gigoxfhqc.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/guptdixmu.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gijgnhndq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdltjveyt.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqsxsngla.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/grsmxeldw.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gvtadcteq.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gmgfkzafp.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/grhpdauhh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gpnisitkp.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gixmhnxrr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpdjwovtc.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gabpiiicr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gailzpujp.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/glxpmrxwv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/glywmaxkp.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gczmolimc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gszrlxkit.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gpdlyimbx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gjkgjtnhk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhfqayj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gitlejmli.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gnmczjnmu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/giaacmiwp.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gbanabbjf.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbccyjdzq.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/guhloqarj.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/grbbiwhcq.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gnrewsenx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gafavyqcn.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gbhltvknb.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gfaxcghjs.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gtukrsyfz.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gscwrghxl.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/geljjiekz.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/ghtyrphdd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwcwubxgo.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/giykengaw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gynaixpus.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gkyjmuoko.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gwvmexcho.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gmjfffnje.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/guvimgffb.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gnhkdzmbj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gihjdecnf.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gwxwrrtpq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gkmxpiujr.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gnxsckuai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gepauihkr.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gvnhbbqoa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gqahwshmm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/geboeugtm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gugyjfpjo.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gxsmrjeqx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gtfphbbfu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/ghqykwyqb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/guzoeinps.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gutegkdsz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/guniblhfz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gylxfjjbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gghafrefl.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gbasdrxeu.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gtjmpxgkc.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gdpkwijay.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/ghcwqklvy.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gpabiflxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbxksolk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/grqrktckl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gzvkoulua.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gsqubirlj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gfyovsrpx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gnirhsiim.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gxbsuaexl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtlnauneu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gsiqnbhyu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gfhthndzh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/glxvjhjsq.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gqpornept.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gdqspwktg.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gszdhqzwq.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gkrrcizjj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gidmyzqfy.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gurnyoqvw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gxkcbhkpl.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gvlyrwctf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/ghpbspjdd.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/ghutlbsip.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gypcprjcb.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gpvjwjqun.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gufmdwynr.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gzsximpyz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gbbiyoxup.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gszzpgonj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gmazzmloo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gimiitdfk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gwzkzsibv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giuhjpubv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gxdgofykw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gznzdnxas.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzvojzwuq.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqxyuoeyn.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gbibiuqob.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gxxuybpaz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/giniajxay.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gsdhdmkql.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/galdynhcy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gxececikz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gltszaxay.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsfkcjp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gdtwzrngi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghwrtncdq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gaqrajpur.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gudssmidu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gsyitkwau.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gzzshfryy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gbtkjnnzd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gsawsbnlv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gfoyfsreq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gzuffrbqi.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/glncxlhgi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gggevvxgt.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gntpzvnyz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gvtbtdcpy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gvwtvsbwf.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gakxasoew.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gfaretlsi.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gocrggzfi.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gcmdtocky.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/goznhyvnn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtgieghvj.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqgqxepfl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gmvkalzvk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/glqrjturc.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gksblmtfs.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gasyqojzw.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gihyabdnf.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gpvsgsxrr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gtzjjvzln.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gybnmhfbt.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gugmureov.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gftumwjkj.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvztvzzhp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/ghwhomjmu.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gvltbylgn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gybikylgf.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gvxariyrm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/goexkugos.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gxetoyxjg.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gszdgltwm.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gdgxvxaey.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/garccikac.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gohwhxpjr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gankmbxqs.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gihzwikph.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gbcltksfi.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gqmvyxaou.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gxtslxsbp.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gbxrwcwyq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gxqtfxezv.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gufywmtjt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gsmwsssqe.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gcezvcyae.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gqbrjpuyo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gcfvvmybf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gznmliavh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gpqrmhvvm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gnreqbfob.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gsyeyrzdu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gdfreojwt.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvcrxsvsy.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gjifbfqyn.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gbitoecfk.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gmyxlkuwu.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gkaqtnlkv.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gereveubj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gtllngjfb.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gnxrrmjis.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gbdscwtst.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gnyvszome.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gweiixhdp.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gnlcdzufp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gkgmwdzgp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gszuwfdjf.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwrvnbfem.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gkysbsasl.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gnvjelfch.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/geliafsqt.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/ggbabfueo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gnxgdpnlp.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/glbvbzyhk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/giuiprdwp.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gibnztrkr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/geectcbht.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gljqxnkem.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gluvtunuk.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gywfiahmf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggvjhzpxh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmsytpkdg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gadbxhegi.sHtML


<!-- 参考信息 -->