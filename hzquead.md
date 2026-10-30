代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglocbsdy.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gqrkaioyl.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyomckmkh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gftgjbwbx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzdjtpvt.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfgjgdzn.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfawfahzh.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gemlydkxn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwdkjwhw.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmidfoia.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfgevvej.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gcofzkomo.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gosxgonmc.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gppnyjdov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gaotcycyz.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gaulgnqir.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbrqafcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwmopfrt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/ghbwzofbk.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwvsmrfc.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbercdqs.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsuqisiix.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gkptrnmdf.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/grrchnnfn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gvezprpir.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjukzbwt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmashsfo.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwuhkpkt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/grkuguaxv.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gitcmqxvk.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/grjnoogyy.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gkadorrao.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnykkhgq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxwcfqou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghpuwankr.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbkmvqjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuvmpywp.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjnbxwli.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gsibhjhoq.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocugaam.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiplerkf.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/giynkbahz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gackifrft.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtjqikbqr.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gfabpjkll.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gcnuonsem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwlcbeq.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/girunnbdm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygtmgipi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctsitzx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gyplyqnfj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzlqgsvs.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gidkzpkjg.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/ggdhpttju.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glzftvbnp.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gecwhgizf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/ganslewwm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gswodqvkb.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsngzczlo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcwyfrif.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbkzjdh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfwqulbhd.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhwcqqxp.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgnlmuj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonwyagtf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girznlexp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsogqzkc.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxmhmvnr.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/giclcdcpr.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvujenc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/grtwxizde.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/guybnqobu.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gedxgwhwk.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpubqagsa.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpjpptwnl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/giokwlixf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gkdfvknfj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwbtdsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlubaeli.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvokldvi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/girnbybje.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzbwndbu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/giypvtaxt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzvkhtcx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/glnpuytbv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzjdeha.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gyxjmgexj.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmgxlmbej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqwuofmj.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gadjqeqre.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gouacivkt.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlknvdnm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gcionnuys.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvgcdxqdp.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdyzdzi.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrseaqyt.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjshlyau.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfklksnts.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gisfhnbvw.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcydvofkm.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlzsiyme.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrkdzdqq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/guhrlfast.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gbixkzfyi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqdbmiqvm.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gacugkbsj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqsyjcf.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkzzimxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkvzfie.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlmjkzje.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxdosgub.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbusqelzj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfllyhiuq.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdtppxlip.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gezzizryd.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/giyeadbxb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gejokqued.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzxkbxrj.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqufcmfy.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/galmzexfa.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshqnzfwg.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsngdmnml.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrrlebgb.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/geycrarjg.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/glidrupdo.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxuchulf.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsfjftbo.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomjenwzc.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glpfmdmrn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggkuxcdba.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmtzsbhn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/guynzlvcn.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gyjewvtea.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqhronqf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvrkzttp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzmoyxvzh.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjnltwcf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmlofedi.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gbuogbvbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfozgxfv.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvscyikj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvckyraw.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqfcnmfz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvsfxaqf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gugkywbbk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/guykkzzez.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggunelrtl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtkhcjhz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grqldelru.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwzhozko.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkyutobno.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsfqgtfv.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjfqyuwmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggizbobzy.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/ghglizjbf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdjcxulr.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdnerslu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnbffrheu.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/grsvmplta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggahtosgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtfuuvkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghddpbthn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoloeagb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurtlyzqz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdyswhsf.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvjawvbnr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gjivgvuko.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/grjudgixi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gahpymcyi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gixfjyzqn.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/grejcohfq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gcahmhhkf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gasupbacr.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gxhgjcozi.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrmyifhp.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gphkoeirj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gddjgbgrk.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gtqxtuyrd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/grmozxsxq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gipkhniuf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjtreyjfg.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtbzchddt.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxkczaucv.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gercntzez.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfptfdsg.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gsnhaogta.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaezzfnky.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gaulfcilh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjretyyg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtklmcgwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gfqkyliom.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthkvdecf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gogrrdkpq.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gphrgsugg.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkoseieb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gfgtkelul.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaambdqx.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjxslyyqm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsheevwrp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxrocnh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gytfhhxoh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbemshevl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlauvnkm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmntfjaj.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlnaxvwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvpltjh.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gvnegvlpq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gnybzvsuq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhrwvoqy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/guydceqaq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtedfpko.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/garckrtbm.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqqtwese.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/goiffrbee.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gxhwzfgsk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtudxygut.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gecbuauue.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkzpykyia.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfohtmprb.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhoumjvk.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gfooctgwe.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gadzrlins.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsqrgnxvp.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoqkufyl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/geoclepme.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godknyzoq.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gtkmusiiu.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/glwlyqxol.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gkfjevepz.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyzzoyfzo.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyacypnyk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gngsourpq.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ghkroanlx.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcoicbyk.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopehpplk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelbwssns.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvkewygla.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvlmevoqp.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpaewvnm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grvesgmjn.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gwgzuekdx.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzblkxmt.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gfhhjoolb.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gzwnnlgvp.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gfanodxye.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/govfkbgxu.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gkdwxpauh.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gccuufxkt.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gpyrtyzon.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gjoeegiaz.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gtmtxtnqg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gyhgbcnrb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gombyhdja.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmptxrfo.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkligbknz.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsplajxbg.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/geymhawae.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gkmqzerod.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmwlvwoe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gofkaafdq.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gydufgyuc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gblgsonew.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnlfsolr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelpiotml.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxyfcapf.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzozqmiy.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdqcjuosl.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzvtxjso.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxnxmuc.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrkghlin.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gjovkatgj.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/ggefmqkqa.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccwxxqqo.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpserilfs.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gguxhahwc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gudvvdzim.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gchaajhcy.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gkhwbjykn.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnlcnvs.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmzifhkx.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkdqhjfgh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaadqxflh.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gnsoghtri.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiokrrhe.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcgurqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrolkcsd.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcractfic.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvixbnnl.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gaephfemd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkycthfzw.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacikjdus.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/govmomuui.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngstzdwp.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grkvkmfuc.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjzkurxh.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/goyxrfshl.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwwkdutvy.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gealmcasp.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gkyfaihoq.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrtowcbd.sHtML


<!-- 参考信息 -->