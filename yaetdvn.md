代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvstvijlz.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gguaxgqnx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gltdfuanz.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/ggogtbvqr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerdkamot.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gonjfqjye.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsjvhxup.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/grrpvumgq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjksulqze.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guiozvrtd.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/givkfhevo.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ghikcpuzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gpndtpsxb.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkwjtmyu.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/geeysnkrq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gfhisonnd.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/grtdlofvn.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokddudth.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsdwreqk.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gvyximeiy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxuucepuh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnuewkaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghtmlrxof.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhorzuci.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gttauoclf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gakusljzf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gkpmgzkmp.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghebzecao.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gpiofsuez.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqaplszv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwymwbayx.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzggbnpst.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gmitsmqnr.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqreljsox.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gxupzgwbp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gfmhvbeus.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gjsblshek.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqhkrozb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gchfngkjs.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gecukqgmo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnjecil.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgkivus.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiyesquo.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gjeowwjff.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtcnvtnp.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gusapioec.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grspfwqvk.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwolpphv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknliewmx.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdogxfrhb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gupalbmcq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givdxknfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ghltizbqg.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwqaixrld.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpxradqu.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/grkqdrjum.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbxejzlm.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gossrxsha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjbovliv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgtltgjy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gycrjhhvo.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gyagvitls.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gsmuryswa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ginsgeuka.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpvfxjx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbfswxtrq.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnyzwwzl.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxrgkxbw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpfrwezgv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaovxqdww.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gmrbxjpzl.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gtppsiagq.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/guznfbgci.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwovpljoi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gnfxrvwso.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqarhxgdb.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdyfngau.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcskbzqtf.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjljqnix.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gpuavwdor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gjcncyesk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gxflaxdwv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gkxpoltcf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrgycbre.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxehvsft.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/glsnmpfox.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgahwwyu.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grfvdgzht.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvpalrni.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gbtrtidow.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvfuztby.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyjvtpxs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqmwrvqg.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gkinffubv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfeemoqz.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpgicnndf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/ggubfumob.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/grkfxpvbc.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gejbkibtc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqixhgbw.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxgfpaqs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnhqomacc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gwbydnvms.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnnqgxnk.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gqyrhxikr.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gitdibkug.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmobhpbrm.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ghaqeaqpa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwbwqxed.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqswzzhg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrabizjw.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gegcizqje.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfjwrnem.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/glwxlufqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcupypnrt.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpwnjandk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwasjxsd.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlrkgvzk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvqbeoyi.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgucrovv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzulglntq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnklsbzju.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gielorlmn.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtlihzjj.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gomtteccb.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfmqqavh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwerdxck.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gsmsieroq.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gnbnfsoig.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzimhadc.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gtifeiwho.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvzwkfyxw.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/glwrfttbh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdygltkd.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gudgbpmdw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpjxkxvfk.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gmaawgfru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsszymxqa.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgksncvi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfffzurk.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gtgkfelwc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmcdyrj.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gikfnimnh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmtujyno.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gbiibtsec.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ganlelceu.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guarpwkwy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpplsbdy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjzeuswg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gmwvnrpay.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkydpile.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrwhylbe.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/guxtjaajg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/glpdgiquk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gthapmxoq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/glfebyvul.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gabguyohq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtifzayn.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuysgvts.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjngqqll.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gnbpvrwho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfstikdt.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gplllfrzj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhfmhayi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcnwzkmdb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlvezyfs.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gplrxyapr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gheoujosi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcabhetuh.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdnbhynm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gicjuwweh.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gukapsglh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/giasiwmff.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbjbaas.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gvhtmtasj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/groewklbr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfxpbnnlx.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/glnrgstjt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaycvecvo.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/goojavzjc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpuvvpqvx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gvahbjcpo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gtfnhobou.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseqcvmcx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwzyinpz.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gojxktoea.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghegsxoxq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwyigcvo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gezakabuj.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/guharyebx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gddzmggae.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggnivbhfx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpegvyaow.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gccuzkdel.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gvunhevoi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpornief.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggixzzxov.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggicnhhvg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwodztrfl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpzvqerq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gxebswkrj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfdewgfq.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gpfhhuyxo.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/glqtyluxx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqobxefhx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwefvvvgu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gjejftsui.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glgxftzpl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxjhrhnwt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqpgskqa.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/goxfobsax.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvvycifp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyubaxdl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gzapamyaj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpncqttp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyxxkquq.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gnvihjigr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsglqgzm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gdxwlqxqe.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grxouawhq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/glfqyotdq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsostcmf.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjkjejzgu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gducistfx.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxtqlgmts.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskumpotm.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwraivlje.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkzybpqm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/giierlmen.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gegugyoqq.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/guvlfxtpm.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmxfdxuz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpratdpn.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcbjprxf.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjuwkjai.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozlyixxc.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gafgtymdf.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/glurjgnwi.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmqrkudu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimryzha.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwbwlpii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppaynxek.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpnpfgkr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjifghhf.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gosodbqse.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gatgntdmc.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/grkdvaqbn.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gnztktevx.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/guqbiyzoa.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwcwlviv.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfcrmwwx.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/ganpchxnm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpnzinat.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gfooipvre.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gzktgedem.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gykkbzyrn.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkswfrjne.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpxdrxyl.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmthzgzy.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbdorrrsr.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gaujkrbyp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/glxjeagix.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpemvwuax.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gsdebfffq.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnsacuz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsxxytycw.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkzooxmb.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmwfwwuc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gsixurgqr.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gvijgmxwv.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpjyrmss.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gisspwrwp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggquqtyio.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gptuawubn.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlozvmfn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gnmktwwhm.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grheypfbb.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumdypfde.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gmlzyxfvf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsivqslwg.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gsaargdaa.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/glzplhflq.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gptczipmu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gruhgepje.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ginkoumfe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giywadrqk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuyxinvx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwesvtguj.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaaelnmn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrletfbu.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/goeqburor.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gscpyhgus.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbpvmmly.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gppygwexg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gazexmixi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gwbujrotc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghmybnldq.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grtjnxsoi.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gkaoidsdv.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/grilosmog.sHtML


<!-- 参考信息 -->