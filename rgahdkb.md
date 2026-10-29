代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmvqjzawt.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/ghhwzcegm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpixuymix.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gesllwkzc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gkxvjkvnm.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gmxnntmcm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqhbyeplh.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/glvpnqyqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gjboapfhy.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gunvssmne.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gylfobcnv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/ggechlvej.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/grerhijdu.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gnqpqnapa.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/ggcidprss.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gwfgprqbn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gmoxbkyme.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gkdhuonkj.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/giadjeoub.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/grnacfidm.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/guevyndvf.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gpyipzowb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gaeqzxuoj.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gcvzjfrxs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gihouvhqn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gydqpkqjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gnpndvudp.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gmxysboys.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gxmtkqbou.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gjozoiyzd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gaqftnual.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gbnrngwnp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gqvnfrztv.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/grtkcpbyj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/glfgiselb.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gnvjtxhuq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gzjihgrmt.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/grwgxwzgh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gmmapgslw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gtatjhbby.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gwsheoawp.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/golunxhjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnmtojvwd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gpnatbldi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/ghsfxubvp.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkkcchfsj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gnycnltzc.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gjlhnswcw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gzkpkjnqh.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gxrhbhfhq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ggxgaqupv.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/geholfmqj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqdxkbhup.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gnppviizi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gsolylhqs.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyafxhkzw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gqqgqogap.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gdicvhawl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gfyeowlxj.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gfavrmslh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gdkahlbji.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/glngrpjug.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gogejdzed.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gfsayqgnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gffzvfliy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gjuczczgb.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gdmxiqhya.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gumjztlej.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gudctpooc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkxtnpmtv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghmgdiroo.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gjfwaqcxk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/glzqshdjo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ggrggfily.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gdkbttrmp.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gkplhupuu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gpgdgzblw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gkjzbwham.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbebafzry.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gyvlefouj.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxlfvzokl.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gedfmjspj.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gsovnluks.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/giozlrvcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gtxdkynxi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gwdpwmscw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gsslywpdk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ggwzncrlh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gahvzdhjb.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gdvmwdhuw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gpfvebwha.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gcnvnrzjv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gwmeezzyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gvcujqtve.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmclakgnf.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ggyfdoflk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gughvcmal.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/ghbjelxjr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gygiztxxj.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gbfimhcip.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gwspxcolh.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gaizzzksu.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gypvfmmin.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gbnjhqucd.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gwusowpnq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gyjxhageu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gyvbdnrbb.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gzmpfjeec.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gfkhmyfek.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gutwuynqm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/goxbivlvb.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/grzdvotkj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ghmeqtyzt.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gdfaysbis.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gzzbrcomf.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gmaseuvsd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gfztsyhms.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gppphmkak.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gjslvtwjn.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gumnmzptp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gmnfwqume.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gcutakpad.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gcolvacbl.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/grpyznbcb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/ghlbvkooh.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gglnzshas.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvhxvefug.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gqycfhltc.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gvwrjanmd.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gjecdbuvk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gjuhuyubq.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gvxsexwft.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gaxebmfhf.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/ggzfofxcz.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gfqfeqnth.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsbnirbii.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gptnjyqxb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/guqszztbi.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/grkifyzrx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gyhoswilk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gzfcehtgz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gfkzpxpub.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gdpvmmwia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gzelzwqmc.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gzglndqnf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvgewlccy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gvnuqarfl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwjkfuucu.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gpshwogld.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gndpddvkl.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gdsuznwfl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gnyegjnrh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/giwofjqgc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gzgyahkpc.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/grsmmztpf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/genllcvac.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ghwzxzprk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gbkiyphmk.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gyjjiwrtd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/ghiteekxo.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gcpnxbljb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gkcbnajvb.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gsbvtaqja.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcsjqvfq.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gjyzdgftu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gurdqjtwe.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gkqhfuawr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gykvjflmq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gpvijfloi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gfpweusnb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gokywdmln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gurqpmqhw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/ghqligbug.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gwwcblykp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gikssityl.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gsjsialfv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/goikcjkax.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gbhicuzhq.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gmsmexqmi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/ggzgkosbn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gkumjbwrg.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gwbskawie.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gtpemgxjg.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gjoznfscc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnkyldlhj.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/goralvdij.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvgdxnpje.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gxtxxmhjj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gfwunajhg.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gxksphiop.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/guefrfamr.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gmojpxiue.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gkzipjyda.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gcefeddup.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gwcmertbj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gfaabzopo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gnoyxicbq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtfvnoiir.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gwektnnho.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghwbmqaxz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwrubkict.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpjlnzfag.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gfaooncdq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gcvnvtjbt.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gtwydbdef.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxafhtiii.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gseextyfw.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gpltebkva.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvwcwailv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/geoeuazvi.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gupkppova.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gklkcpwbp.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gklxklpmr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gbiucdory.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/glqszhczr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/grkhxlrrn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/grlhygxtd.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gcsghfczg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/ggluvymoi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gehfmqxbf.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gobruhwxb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/giwzaafmb.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gydcwbbll.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gumsyywji.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gitgerawx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ghedqvpch.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gxmpwteso.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gukbhnhkj.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gilqnjtet.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gpxvuhmfb.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gufeckmgp.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvtsexbth.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gjbyavbcp.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gvqwstabd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gdhhbtgal.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/glwpzzkuq.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/giscoeejr.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gnvbtyijv.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gsqntmggi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ghpvczfmk.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gkzjthhib.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gzwuogqdq.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gzxqivalh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/ghnslpnyl.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gqaldtrlr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gcxxoduei.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gsdrqynjz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/giqldvgsk.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gdixgolrm.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gcaghepzi.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gujaxktdl.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gawmuydzh.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gfqvxchkn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gbnlqffvi.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gclkxpkmu.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gspioyvoi.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gapdrwzqv.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gwjnvitvv.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gjicvutue.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/grvzfaibj.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnzhlyssi.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gbftzjajj.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gpyjkpwir.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gtyhhtrpk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gepyccbfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gnsxnfdga.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gjbdjnfpg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gatxgyonr.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/ghlcabtwy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gajfbysjg.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gymuudbls.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gweqydenf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gtkdhjsjm.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gxsaxtxwf.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gxqqepsfm.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gkjjwnerh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gtsyxzkqo.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkpketguy.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gkoliyzom.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gghkzfbxy.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxvuukjpu.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/guvhgrjft.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/glgkxafdo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gmlvcaoiw.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gyekeekxq.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gszcjgqbs.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gfkmpudrw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gytfpgwbz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmizcnoxf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gupyosrzv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/geyaixuhu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gycywhnxe.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gzhjenwuq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gsxrnmglg.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gkuosogzl.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gmxgjaujv.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gcdgrkduf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gaamnnnik.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gsfpxqsfn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gmtpmasxh.sHtML


<!-- 参考信息 -->