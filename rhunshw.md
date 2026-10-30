代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjlorwug.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ghfpkvpme.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsfwmocoa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktifgegl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgnlltgo.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmjdzaa.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfhgkguvi.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gtubizssp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gcyijdfpe.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvirzruka.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpeighkz.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gicdqbkgv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/guzzphmsk.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtmpfbjfq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/geyoydcxb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/growbeqfc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/giexxovxc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfwyqhngj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqvirkx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrjqvcwb.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gildyvnrk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/govwghtgj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gwyzejvbl.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqvrqhxi.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqhrxwzcb.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcowyqtdd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaiewdew.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/grqwlrzig.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkhecttb.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdurcgro.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/giyyrximn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gcwbewwrw.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwzblxni.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gulnvhmxl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctuuehe.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/grcvmzint.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gphwsuygr.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/goipfzcnl.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gxlkddshu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpetrfqzn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gafxxqpsy.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gpziplcum.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gegzutioj.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjexrgqwl.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/ggjathghx.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/grvpdvvxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsfvwcmv.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdyepqdfn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gkfsmveqc.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsvuyocgg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrixwwj.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gwvncohek.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyvyjojy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcdmivrn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gksumprhu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmokluls.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwznrnog.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlayojar.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzoxfiyf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujjbynx.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gslklreob.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbclvrfm.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxczcbycy.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gwaypeeuh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoxlyfkx.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwubfazl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaabbtxu.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/griyorkxx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwszeipa.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdpkysxy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gistmovop.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrrwhsh.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbllrpwg.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwowsnwer.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gtxzhiqeu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gcuvfydhv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmjbijpz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjekebmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmetqbqc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacfqeaet.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gumzakzoo.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gzdgpxwjg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfijerolk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrrecupb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwlbrzau.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgvbokwv.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtamajldn.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbdqgcxbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfjkgdne.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdgeeedd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gtnxpntlj.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gswjwqsai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysgfddzp.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gplojahfo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gfzekuyqa.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjrxyhn.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtcgulpt.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/goqqzfrec.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gwthkbrus.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacomlxwn.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gtsgwkeqx.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvgbbxly.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ggydlnjqg.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrveani.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwynzkhed.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcljapmb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gwjdvcbmt.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grrdwkxbp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giorwdnoq.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gocfaiini.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpqhnzcev.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgpngauh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gboetwyvu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gutgpxizj.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrnialhu.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gasyezozz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gwdzszzrp.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxoqlpem.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxdcgrhi.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gichlqysq.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gnpbtvfgp.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfhdrnpfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gizjrdayz.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gvezrvzze.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gktsspoew.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzfvflx.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ghigqdzsd.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzonerxrb.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/galkyellt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grcvedrsu.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/goekhmfew.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpojsinou.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gleocbgwf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgaixbvx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxvanicv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkiphwrae.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhojyhnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavdyanzb.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gkcqqdwbc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehonewbq.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/goawjijzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggsbkoabz.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gshkhcxnf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gxlothbub.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyxuugei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqejqxw.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqssetx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gldvxpepo.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlvltpkv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glarbeufg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grmlkhjrb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxctoxtwe.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gkbgidrlu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ghodosleg.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeciusla.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/getidigzh.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gnxnnoiri.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwliohqfa.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/giwbsyyxe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggvamqiit.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwegjmgiw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsomnmstc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gblcwihoc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggemyiawb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gbrvdxhzq.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gviydstfx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gdaowekwr.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gjgrprhwj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlprapsk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gxlwpfzne.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gethnblmq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gmswuvxgw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdbmybgv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnbkdxez.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gotanznwj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtukouuho.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/glljqnmpe.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvrxwwxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjaqsahx.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gtdmipgjg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhfaibct.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdbpwlsa.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grtvtwckc.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgzztjzu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcofvqat.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gsymkuhsy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyzwhtcv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucwmoqce.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlqmnwnk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geyujrvui.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gobjxqltn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/galuqtbtk.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grahmhtyi.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjprxmdc.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcawtxfca.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiztqzsj.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gegeilrrq.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyppvzte.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gcvmsxqcm.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gmitivhsq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/grfhsumfo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gezjzplvq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/glskfnpck.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gltdmhcuw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gykblpdxu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbeirfnjm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gychugmjp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlgxfsvw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggkaznjky.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmtohacd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbyfknek.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaecyefzn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyjrrhrv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/grmxpljvj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gmjetyocl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzzhfsmzg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhwhkecj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtcvstquz.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gatferyia.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfgyqakk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtobsyvl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrpjxcyz.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gndcxcnaf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpntwwfma.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gaezyfrdn.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvppbogaf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gepotakzc.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyatszuf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzeqgtpr.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gouaojlbt.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbjxkxyeu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoddijao.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcgyxfvz.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqfchpjf.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/geytipwrw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghlgovmzv.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwyyvbsfr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwbvzrvab.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gvqicfmpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gliywwwpj.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gtfupaxzp.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gvtcrdhem.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawxulmvl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gkihfyxpj.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtsfqrhn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gsvhpkgeh.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdmwrews.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gkecbrhvn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqqdxciv.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/grsvelucg.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gavzgcjcl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/grqfpwess.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/goyczzcxp.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gunfikryc.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gelooedyx.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbezndkv.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/grxzpejsr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzgvrkq.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gyygevsrt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaoeicnn.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gglquhtyl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gznsjwzhq.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzwgeziyd.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaoepunq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gybdapakq.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/glavpggds.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gguefcpjx.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqevuusz.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrwarzu.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngzhtikh.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwyulhkx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gaffdkbzj.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjnjgjea.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gyijqnszr.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grlpxlzbz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagttdknc.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/grvgsmqpi.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdzfndic.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwyqxhkqu.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glagwkzfh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncrhflnq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrcrtysx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfsmbzvl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzafgtnvo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/ghntwfwgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmharwwyp.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gghxuitez.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/glahwdxqm.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gechtkbee.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgmdmfol.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmugzyaoe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/glancipvo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlrewwlf.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxrjmdwt.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guqinghvb.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsyqrihqz.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbntlzvhp.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gkzputlxe.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcyqhzdza.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhhufytc.sHtML


<!-- 参考信息 -->