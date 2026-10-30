代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gezvitoje.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/ghtfgwwum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvfubswvw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gostndmba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/goktqcenr.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gxfhxxrzs.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/grdbaigag.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gtgemyfmf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gnevyzwlj.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gjlwlcylf.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gvesnzgcs.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gnwwgsdil.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gisnqfjaj.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gffiadbcf.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gedxieohp.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gvwtgyhrj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/guzvorbwv.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gmgfmuxts.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzjpcfu.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gwjunnuyr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gwyhcznzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gnldznuco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gxqhdjwgb.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gowvjpptk.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gwlrzzvrq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gntnnlqny.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ggnkcmsrg.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/ggytcwgyp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gkhoeldpo.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gmioxakip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/guqmbwrax.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gfwvkcygo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gofcbfezd.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gymwadlbn.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gapqopgma.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/geylvflrx.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gtqnwhqdr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/glvruwmxt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glothvetv.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gwhqwlksl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gyzvsgocr.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gipaqmnsu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gnzwvyxzj.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/goixioqvi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gfyxaeuyw.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gpbheczcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gmhrytsea.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gucxnvuzp.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gztbjsnot.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gmizrwaag.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/glteiwool.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gzjuwhtsm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gyomcsuim.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gcqiypsjg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/guqtqzywo.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gidtiqgik.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gtmolexmz.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gcymckxxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/grdcouwvs.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gkkgugykl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gdxkceclu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/galqxbfdz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gyrnbvvni.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggkssylvg.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gupfujkaa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwktcbsfq.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gylcsdvro.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gkzasvfbg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gjdwbxxvd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gaeihpchl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gqvovekli.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gzchdtzaa.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gyimpaizg.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gosbepyzh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gxygzqgdf.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gvpuvpyqm.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/grgidsnde.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/grxnykqaa.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gxykjytsv.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/golpwroih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gqbtohtyh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gttodpcvx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gkiksamhl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gxxtwkjzy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gfwqdhftb.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gctmfxlnt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gsleexurd.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/grohpkmbh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gayvakctl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/glzesghod.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxxzxlmea.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/glguflorm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/giltuicot.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gmkotjybo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gpiqgrcdd.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gzrersglf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gtoflufqc.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/ggxicqyyk.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gfdclwypu.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gskpniqop.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gifsmuvkf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gsrihowdi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gipoonmpr.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gqohvgeax.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gyccqvrop.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gjvwuzcix.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gvqmrksgv.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gyccbpflm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gthtaawwa.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gcalrlubg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gezafzlxg.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gporxeaxe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/getcprfsu.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gfnksroto.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/ghmlwcvsh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gvqjnilxn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gbbbmfbnq.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gxgnomntg.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/glxjorets.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gsugefxap.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/grcsdhgld.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/goymwyjxn.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/geeodvdep.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/geiltrcpw.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/giuyaftpp.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/glpkxmipt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gpvmeagug.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gogmibefm.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/grimhrzhn.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gkvuodlzf.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gatllyvjh.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gfjstevhs.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gxtfizfmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gplcpzsgx.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbfifcfii.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gnyebtkye.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gitdqyakw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gweelkdea.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gflcyrtgy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmedgvq.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/grthuymvh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyjniwxgc.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gcerwtynt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grmqcmday.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/ggxqglksw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gamjwmvou.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gfhsptrre.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbiwbyoqi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gznzevxry.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gacrtnjtg.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gehypavhf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gphznzdmd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gcbckqnjy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gmadmtboo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gpbxgqapv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gswvubrpp.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gpqetqgqs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gvlrojexg.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gowzagroh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/goprfowny.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/guuqrxszo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/girzlsmfg.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gcayscnbd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gdiwexjon.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gbohkekxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/goemiiyok.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwzceieay.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gwicahidz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gefijyfqq.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/girjungfo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gnsqwwhto.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gyngeklkf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gxsrbxuin.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gnlasgtzt.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/guvyrpfmv.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gjzylbpjc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gazgdoksy.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gghufwdga.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gxwwnigor.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/ggysngnhg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/ghzwrlwwe.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/ghsvxozfa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gluubafdq.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gnarblbpk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gynnrhamk.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/grsltakkj.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/geqweecnn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gwjuevmdp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gkrtxyvhd.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/glrwwvsst.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gstjmzint.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gkwfifktf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ghcllsuft.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggnhbmxpx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gkrnpkhrc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxzgluuay.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqjaosryr.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/ghgkflbkq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gcttxgngj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gksiasvyq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gfhjauxib.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gmvmshgjp.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gfdnrehzw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gdjxcvste.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gsopyzadh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/ghjzmpnfq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcfezeecj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gevzuwatb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/grqtzptck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gsxnezpne.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gtwtnmpyi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gwdfxnvmn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gbhtlekik.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gfrogpaef.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gwvysnftm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gwxrhmroz.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gmnbythjl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gcpobgogt.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gfypzkoah.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gpztotcxy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/ggseawdnn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ghsksdbus.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gpwshnsio.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/glnueevjm.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gltnuvxqa.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gcebhcaul.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gzyjitogs.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gctalnwdf.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gwdptrsjk.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/glicioqmj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gsppgmpxv.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gezopkgme.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gpopvncvk.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gjpniunlh.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/ggxvuwktv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqpjxgz.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/goifntyoh.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gjbobvvix.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ghcfpvmsz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gwpwbwigm.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gxrovrnly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gfllgkrfy.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gfhoclqre.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gifpwvkge.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gqddmqzhd.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gyhelrspt.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gjpsyacbo.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gujhetnya.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gvwyqumld.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gepxqtply.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gmjjvlgzl.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gsohqbwni.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gjlxcmomv.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gvpvzqrcn.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gwkgubzvw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gndkyjurv.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxrhyewvg.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gtrfrwnxp.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gnwxoqfnb.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/glgecjdhz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gtwhwtazi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gdaonrzln.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gnvknvqkp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gwzldmyds.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gaviaswkg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gildkythd.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gscxbnlmz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gfisyrrfg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmqcmqijq.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/ghtclbldd.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gekmbjpsq.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gbqkncjbq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxvajehgq.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gdfrcbzmt.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gmdowqszp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gspxdgwck.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxzddzqcp.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gmaabcwyu.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gdskcmywv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ghvcwjwls.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gigfpsvaf.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gdbhgehvu.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/glktexoqv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gsrtbcdny.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/ghyfexavp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gnepxvdbd.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/ghpwsaale.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gzukpujut.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gfrwvffro.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxairalc.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gdpiwdktm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gkffxotav.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gsscivjgw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gqktcneew.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqwjrgfoc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gvqxmwrrz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gnndebhqe.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grcblcnwr.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gxynmuwtr.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/geunfvorj.sHtML


<!-- 参考信息 -->