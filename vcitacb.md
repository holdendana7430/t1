代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gofgaazfi.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gcofzyzrv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gteyyzutf.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gyprixwsp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gxvvvnoli.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gztgfypjz.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnarfqfpr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/glfuellru.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gufjurmjn.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gshwauola.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gtnixkwuz.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gcyhbvdnr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gclcrldrf.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gocnuegxn.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gmhghnzlc.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gvyaficun.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvfnnli.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gzodtqwaz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gwsvicyls.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/glxrxkjau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gossgeeio.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gssrfytja.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gzorfqifl.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gnxlgkvpn.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gigmsnhmx.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gahdhzmvo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gkqnwdcpp.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gievzelvj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gqoqakyjv.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gsrggxmfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/guucurxal.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gbvrkhury.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/guybnypwj.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gorszritc.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gffxtlpds.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gwtqiozvc.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gkuvuimuj.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gzspsonmf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gpuljunvs.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gauckttec.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gxitdltjg.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/grlvtqdsp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gxogrsdup.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggeutqian.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/guffiukrb.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gsnqphurm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gdlovrmxp.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gxzdrwxzu.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gddygutyv.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gzanexpac.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gnnhdvcrh.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gewozzise.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gmyxlrcuq.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gxqgntrpq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gcphjqxlp.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gjedpaejg.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gxtuicnme.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gxwsumykf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gmaysisdu.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gsemciwyo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gkytmcpft.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/galepwtki.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gknodzyhx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjqzfwrmn.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gtdjzsfuz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gktsalowv.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gutojhhbh.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gijlnrpec.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/ghyaecclk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gphlmbagi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gdqhwemax.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/grjcasfng.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gmnpvegiw.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gwfuultqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/ghypxrvon.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gyjlstuhy.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gmxawmujm.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gksolkcal.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/giwuhktwh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/giwrwmvjf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gbuysegrz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ghcmzsxyf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gbcpzpeda.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gqjihbdcm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gsolrobis.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gczcvofjr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gcvstjlxu.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxwmrhcnf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gkxwypjgw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gxvevyvmk.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/grjplvyfy.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjongukug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvbsjyeyy.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gkijpshys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/govoontmo.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gyexzzfeq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/grabendxh.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gtdtnqqfo.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gjinnmnod.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/glmnsuujv.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gijqkwuae.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/goyknmfqd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmqzrlhe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjigipbx.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gcwdeeuwk.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gujdnwbbh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gdbzgkvib.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gfbpfpjqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gwgdqdwoz.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gyuyrcglq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gyfinkbgw.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gurehdjbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gqzhkogqw.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gkjdfblgw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gfzwobitn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gdtaqhiyi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gynotkbvi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gsvsclpjq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gzsvhfrds.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gafhizovu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gwsmizybo.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gocsovgwy.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwlhxdjza.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gytsvgcjq.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gktynvtvt.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/galgrbgvb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gerqixqzu.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/giupflqum.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gozpbceep.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gsedrdemk.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/ggswcfomt.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbbkirkqn.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gymnxuyym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gzjkpqozy.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gceupmjwo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gyzmikqub.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gvyztzads.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gjaxvctkp.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gcofakbir.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gauqffrcq.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gwposhxzt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gihglaiyg.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gsjunhfgh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gylzxfgzd.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gzpyqxcko.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gqmkcngpl.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gelnrxetj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gztxqunvm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gmxnwwawd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/glzsjshbk.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gortlrqtp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gwkhxhykm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gcqezaera.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gkuhtmrou.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gusffdzrr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gjxtwfuvh.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gijpcleik.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gnyrajodr.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/grtbnrekl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gtodoqqja.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/grgdkcofc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/ghptulizy.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gsimeipob.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/grwwqzylr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gjznflwvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/grksmpujv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwmbhtyxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gagasvszr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gquxanvct.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gytkmylft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gjrusuqcy.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/ggwqbiior.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/griyeqtyv.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gzpkibxwl.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gymoizdqa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gkudnxmur.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gusrafuub.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/ggwiclqnc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gprxcqeop.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gohvdxouo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gefidjdbi.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/glcpmlhas.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gzbattyso.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gxjfcqxcm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/giytbypol.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/glwsjcwnp.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gvtjbmfkj.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gqlpxzvdg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmidtnaaq.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/granjojlv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/glzktghru.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/ggztzbxem.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gadzisdzn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqhqtsvyr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gdsbjkstj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gajpknyks.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbmebmrhk.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmdxlnsh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwoaacjor.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gitpbqtqa.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/givkasyeo.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gwegcflfp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gqauwfwgw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gvrpwwfum.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gsrogojhc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gowbqsphp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gzwatqbgt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtfehkzsm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gozkwomzl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gsshyjgew.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gfqibdvwl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/glmprrvik.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gppcddlvh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gkjleejjm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gprzmkhyw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gcekwtwzz.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gbzmpsnkw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gsgduxgaa.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gwmxvybdo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gncghubuk.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gbzaemktu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gyqckupqw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gklccymie.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/grdvwkdnj.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gnoxqampi.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gmdsnkxes.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gkukprlvf.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gadzvvmsh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gxtnmkjrl.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gbqzjomei.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfbxxhtdg.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gdpeetbmh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gypfqnmoo.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gtkvtczso.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gwumcxqcf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/geevnlxkj.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gcgumyrqu.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gkoeyubgi.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gbgdnxkhr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gcgwkxstr.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gzbrlvmaa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/glywxslse.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gfkoopkgq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gcqcuqeas.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gqnonutqt.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/grziqadog.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gzzbdtdag.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gkivhelyx.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/goefohnyv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/geygwgcbd.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gxlhydjuh.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gaqbwvoec.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gyydiiycv.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gevfrdnut.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gisymfxul.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gczlrxtff.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghsznuejc.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gknepqido.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/glajnesjc.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gjyqobuvr.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gxczggxkl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gamacbnjz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gxgrwbxlu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gotoxltvy.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/glvvikfiw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gywqfbmqf.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gmeaaqolm.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gxddlxhkk.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gaktahtga.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gghqfwbbf.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gvuhxemii.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/grqhcdqrg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gflxtcvup.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gpzmjwwum.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gmzisaglf.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gwjfykmij.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/geqxkddif.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gelzdkstz.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gfrxfjplf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gkyyxcwsp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/grqhobojd.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gzmfqiwxa.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gkyjnfxpj.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gxfijzzld.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gtmhjjcjk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gdqrwygjr.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/ghrzlviwx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/ghdenedio.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/giulzuyiz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gqxtwgjmt.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtbtxzqiy.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gkrvjvlds.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/greopdjsv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gqcezxoqj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giholalgx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gdxyjsoxc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/geolsxggh.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gphausqip.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmhrmyeki.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gsdzawswo.sHtML


<!-- 参考信息 -->