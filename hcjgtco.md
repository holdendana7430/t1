代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboukcjeo.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gawenziok.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/grbffnomn.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gtngxodck.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjxfchpo.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxiqslac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfedsajv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptkunzsh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmafvds.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghyamzepd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbcfqcqdu.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gscecvlbn.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwyfzigj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyubnmatz.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gwgaizkkj.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgouqtgs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaflmmsca.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkgfayij.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsreuaaab.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvwlcgzh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaoefjgc.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gifajxgha.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ggutbxkyo.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gieshqgfh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmdxddig.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgmkipqh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfigvtxtg.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkcesud.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gnsggncsc.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gfpjmfzck.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gnwkojhtn.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grvnxlron.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gmxrnqdyz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glztkmswd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxzqksqee.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkswoskcv.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gngfwdwgm.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gebmncpga.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgdvjwoi.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gemvvvxlg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuzbmwsf.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gekrvjani.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaodfinu.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpdlvsph.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfybvcijm.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gsnbuhzry.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcoysuliq.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/geovqkljz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgkrxxtc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcprbumwt.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gblnhobxx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejdxuptp.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghglrbbev.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxwfbzkcu.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqfbpcrz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ghcbwknvy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/glqzweqno.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnylmezgj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gostgnhwg.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gmtnwvrzd.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvacijajb.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gnfodzvis.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gqvdfzvtz.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzsuhkvp.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guowkuwsg.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvsrnwrp.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybgvtyz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gaavjiber.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gekjtmsmn.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhgguqfr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcaxlgfu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gxmeqyorx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfvoqdfi.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdldwnqxr.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqbapqqm.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwrraqzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gystssdev.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gluchbelo.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gjcvjctel.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gesqzbvid.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gutxuchjj.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gogtszutq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gngqrmqgc.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gsfomewat.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gbthvcavw.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgmmrlpm.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gouptrqfz.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgvprim.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxosmywc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsezjiem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpekbgcs.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghxjwvlpv.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/geltsbutn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdbpjkyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/goxdrjqvs.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gcislgquf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrmadcdf.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gxzisddpg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrdgaukl.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gwykotewn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gokpqnvsp.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gseoefwbo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gcbjxyxtr.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkrtvqdwy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuhpenub.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glieqsurf.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyezzqhjx.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gsirlzrlr.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gbhuqnxfe.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gyhkmhiay.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gzuvqgriy.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gstnxhnvs.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhvsanpx.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgdqsqlt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtasnzdyr.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/giktjgbof.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtgvrjys.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucsvsior.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gmojmpcys.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbirrxjbr.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtabrfvv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glkscjegm.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbggjwzg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpmwdbd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssffelzh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtlywfmci.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgfegnqh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhashbn.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gadassaea.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gafqcnusn.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbljexrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfddbmx.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/ghzmjjdkv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaqhxwwl.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpcwetkoz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghescpwbl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuwkregn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrzpgsbu.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwbotbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grceecvdz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/guikmyajz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gshpajfck.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gskiaswqy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gfcxntlcy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawayniwy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcbgdczj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwtfgqdw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzorfauly.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmugxsii.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gqtuhgipq.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gikzfualp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifsbqnf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsrstqmyx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gafmxiusk.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnkbwxxnj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwryjtu.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqeswyso.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkykiwfft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gjvgujdxr.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxflbhckv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbqqokq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gztnxirnc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsveuzti.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/ggszrujai.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gheomdvus.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gcomkczrc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzquuubm.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfxovfxh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gidwjtayh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzetihau.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkpuxkvp.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiytodso.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmqtczwun.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpquwzmu.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkswpmzci.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbziufdne.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmouanmu.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gchxetszz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgrctzby.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzqbtkkfb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnluvrnmy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeyewxaj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gswwpddzi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gojcbzofc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmqfmzff.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggctlfaqt.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjltwskdr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdntepql.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxchvirc.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxzzromaz.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gqmkngbol.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdbkkqtl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/goqbdaabs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gzftnsedg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkakhoqba.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrfhncq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdlrnbfi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfaqinxx.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvplgofnq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gopvgmrhw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gicskmhnx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/glanuapgu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcaeywekt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcnepvkw.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/ggkdskspd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkienqzl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gtfefjbnn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdzjihqe.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbczevadr.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gymfqekdf.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/groqhasay.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrwtbcog.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaccfsfe.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsuevkdu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjfaxsrn.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gkxxuhkac.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/godjaoxhe.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfxdmfwc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcknmdmu.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafbtpdbq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gboquwmxj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyggsokl.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzhohtx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtddrolmz.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/givgevsuv.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gusbjvptr.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guovuowbt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/grojkskcy.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnyxvzm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxvsnvuv.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gictcalyp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrivjiwz.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcijirzv.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/grtymtpfw.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gspverxfw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzgxyrdk.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/glaziibcr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsrndukg.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gmlkvuhkd.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrcikuhm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqmjltby.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gpzjtklgj.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwskwgaue.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtkzajmd.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giwzuqata.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzvxyyout.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geuybhzuy.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/grwayrjfv.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gopsblfqy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gctivzkdw.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/goomzaici.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/grbmqabsv.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gofydinzd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdawaipai.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkgamthrr.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/guzplkcrf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gzilnnsxr.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gktwwiwnj.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gsleulgsk.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gkmqsibfy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gntpyzykn.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gykmonjlz.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gjpbcircm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrxocbwo.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpcyyfwes.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gybcslljd.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gofenzurm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrfanyhc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gomzknpuv.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gvywobknl.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyknnzagr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gymyqqyrj.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gukqgfdys.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqphxix.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfllxvhen.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgxnrmen.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsqezcaz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtgfxsyk.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeyrwxai.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gedrnivsx.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gekugqelr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvcrictlt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkhfyjnbs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmklvgysh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjppowxdp.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozzcfef.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gphonemzp.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmusnzvqc.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdbqvtkm.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grsdrrdfz.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsztfaeq.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ghomcldep.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyiuttnr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuelybxk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/geursjoli.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gsrmnqugn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrxpuyqt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyxldqyz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlwlcgks.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpelkkgv.sHtML


<!-- 参考信息 -->