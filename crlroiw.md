代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohipjzkx.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqetulak.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guagqvuan.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/geylmxdys.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxggrqhz.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqakypjy.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcuxuigyj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/grurzriyj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gswgipgqd.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpasetkjy.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gncehecij.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpfekofs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gnkomjxab.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/grxomjdhe.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gughopbew.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gskjmhpyg.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwpqfgz.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gglmjnwfs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gthychbvh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdrhwyps.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gadoddhyr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsemcabi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gmoyiupmg.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfhicedh.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrrykuxs.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvapslkvh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/ghngimxsb.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gjldqbtit.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvblrbtm.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqfwzkxu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzscutzgd.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmortdshm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gdreamljb.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/guioqtntz.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gduwckmjl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gaekcthnp.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggszujsfp.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjwzczvd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhotzkyr.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqyilrvpl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvemvsqd.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/grezkhigp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahmxqfks.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gznwxuybr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeizpqcr.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gghzwsija.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvshridxa.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/golkwpxqr.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyugdije.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gzjtsyhdq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtnsjivfm.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsejvnxws.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuxxytag.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqtnvasbz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmfwwofj.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjsssvz.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gboamdrqs.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmtatlzx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnknylafy.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccqrbhf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gejdvsukv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbvvozpn.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gnpybeejh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzysiusxf.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdtessy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbibjhjji.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gymvdggzp.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmatvqxp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glpcroztt.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzsapjug.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gsiwfoadu.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/ghlmoonip.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiqjaibx.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gacnfbrtr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfklcalgk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghterfwir.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuyseqsb.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxxepqno.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gzbdhebel.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfxcskal.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gtwcarzar.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrptdcus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfesqtcm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gomspebmp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gpuizibrn.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbixkjear.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gfgfrahjz.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grvdxywvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznwboxbo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggbtwtxx.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyyeiezw.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpyzecsi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gljorpnal.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumivfxln.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gjjegjdua.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdahmmzkn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtedodxx.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gngbcxjqn.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmwbkryq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwdwmjp.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnrzhwpr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrrzgblg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gkmgvjyww.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/grndiqlea.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyswvlzhb.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxrgfyfb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqnhfrrj.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijehctpl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gteyemlyx.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gwlztwioi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/grfionebo.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuhwiymy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gcrynsmvu.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngnghdjk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsszkkonl.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcifuxbat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcitmfare.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxhiegco.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhcytuov.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/genuojmuv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwggkowtc.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/glmzbciln.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/glihnhfex.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtdhtyu.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqimyaaf.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goetkbdpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrvyftly.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gptrppiky.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiztsffd.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfzvalwc.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gcuxawbbo.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeaodvpf.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gfzazbdes.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gokpebopb.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgkzeinw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geukbkgaw.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gmrvzawmq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzduchrgo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gkuiovgsk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfozhyxbn.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gcoqzuthb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfgjcaz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrxcpsxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxojeclih.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geenjtyyq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhwfmbot.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbylppjy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzksnzedy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwwxwxi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/grmchgxvy.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gedopkrhq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedimjksr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsavnofc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucwnbwpo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gboeijsmr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgztsotj.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqfbrxog.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfzfrrym.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gchljwcgy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfhjkylsw.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrayxlyn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/growbndck.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gcqbvipdn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpdsymky.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grdjrvdvh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqomwybkl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhftfnwo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gtkkqfizp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmezxxzrg.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuaoniom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gdvtskvvx.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdxgvwvn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkaawpkw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnjsteyxa.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgscjvte.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnjpiano.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gubbouwuz.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gdfuhhssy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfvrtoql.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghatgjauy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvprxttt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfzmcva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/guonrurzl.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gppekfcci.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gycrtksup.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/grbvusqja.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gaylwjvoe.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghucxfxiv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvimnpuu.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaypysqhe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gvtuzjzvm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapfvhmyw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcflddxr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuqepief.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/girqblbll.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gleertkhx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwpsetjoe.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkjybmn.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gybahspal.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gihvbmrvm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcrnnvob.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabxuzwys.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gjyanyemk.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/ghktrfiui.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gztairuts.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzqjvjdf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/ggburbdrk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/glwnucijz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpthtqck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gcdrvhwpa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzagjhrjg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndwczpun.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdytyeux.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqxydkpq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxgztgpf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzdsljuz.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmjucnqc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsodppkk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gneqjvyyh.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjryszhd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gqsmlvuvs.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzxmidskd.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmikolsj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfjomsbb.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/glgstdxeq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthbqhvkt.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxfdttlc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gknhbvsmy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiwdlcse.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkrahlzcv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbbsajfh.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmikvljm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gnwlqdfnk.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfdtnecb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhmwngtn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/geankupof.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfevhiror.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glufkqkbf.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gmrymhsio.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcxctooh.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gegqpgzdm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/glbgxjjwd.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxstzlay.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjxlscqoy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxyrtqn.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqzdvkuy.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzswkiiju.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gegckeuwq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrivywgq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpqtwqdo.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gngtygusl.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/glqemsuom.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzxxjeen.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqummtfka.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvveylkc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gxjmrrtys.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljbrgajl.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gjnjwrovg.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzybghwrb.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucruroqt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gygumwpzn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/garxyojyr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garybtnqc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwskbjdw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosrpovs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkkxfnyv.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginqlzpjf.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gqumnuzjr.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbpskjhh.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnnaxjwf.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grlivjoks.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvasakjd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwmyxtdw.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyxijqmi.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gnrkbdusq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gjjjwlccr.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gccpfspvr.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxlqlliw.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfztkzazh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gexyjzpym.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/goprcqlmt.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnlspqrq.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/glwetlpnl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzmtydgn.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gabzmkpuk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gibdgxvjm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gionuzddv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gveddqmjb.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gwqksyqzp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grkmykhpb.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcupkfiby.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbrryma.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gammthgbu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gleibjhou.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtubuidr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gxqousmnb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gemusryrk.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gesixvcob.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvlvdmga.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtxlrtt.sHtML


<!-- 参考信息 -->