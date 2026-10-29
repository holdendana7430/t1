代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gufeilsmw.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gbqniovpq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gnlvtqzfw.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gtlsybeqa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gditolfpt.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gmbercwfa.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gvocmbros.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gibomjchs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/giimhbopw.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gpcvwnzki.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gdrgabhha.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gceuyjrgz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gserspvuy.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/glogrligi.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/getgqyhkg.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gtjbyykmd.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gdrmclxia.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gmsaomkiq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gnzituatk.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gutrnesyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/ggnpqjldq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/grecdpuzf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gwdhrkpxu.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxlqcurum.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gqcxfjcps.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gbukclcwd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gstasgfsq.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gndznvwwm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/ghndmpoiz.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gigdmaidj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/ghmdeiubf.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gjvxlwvzt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gxxsdmxff.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gdodsrhnu.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gjkskzwev.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gmdjznlzs.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gzcjzupbf.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gtjvrfkjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghasexoaq.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/grnjufwvj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gldpeeczk.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/geluuovcf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gpibjhvvo.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gednkiatm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gfflaooxz.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gsthnwako.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gonooykkc.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gztqfmdln.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gyjcgxnlt.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gpzgbevdc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gxcbfnmyn.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gjtpsheay.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gemkrpwxw.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gvfykvnnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gdeypitwh.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gjfkslmaa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gnfhavvmd.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/ganqnivoi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gvyokplnv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gkjbnnkwy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gomkuntcl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/ghwvwsrkn.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gsypetqbs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/govjlgvpr.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqvtfuypu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtfmdtapx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfaeuowvu.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gwipanerb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/grrmykyxi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gufrofwsn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gkhatddkn.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/glqbdwxrv.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gczwnrwix.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gcogccnyf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gzqxcbbxz.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gsxhxbjdp.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gxkbmlzsv.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/grcwqfhyy.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gvuzekzha.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/grwprhkki.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/guplmtirj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/grgcyvsym.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gartxkfdq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gdtmyqpeo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gialkianv.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/ggbyaxpob.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gbyivdeqp.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gagbkmiit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gmtbeiolt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/greltqpqi.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gwcvsceae.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gehfhybow.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gjejneqfb.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/ggmierped.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gdaenjilu.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gvgorsqlw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gezxqtvkj.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gabkhcmcv.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gvhiclqiz.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gonunjmmg.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvgqvtler.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gmriujkoi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gqorsnscf.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/giurgllpq.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gvqwcgscf.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gusebjjep.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsvqencz.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gioammjtm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gbyfydact.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gsntxvioa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gzjolckyw.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gcxidvnwi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/ggzeuzxdn.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gtdvaqeaz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gscytabog.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gobxesfel.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gwheqwmwz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gcwxzztey.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/ghzenduqf.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/ghsajyzsl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gqyskvlqg.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gglhrcgci.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzgwhmkcm.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gdznshfho.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gulkyvltv.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gkvzwngkp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gwwtdgkav.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gqkvpiack.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gdkikucsl.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gxbqprdks.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gnccucyvb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggmbrwpou.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gyikfzdkp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gizwucmnv.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gavnidtkh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gpfxxvntv.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gweocdptm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gkfafkhcj.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gkdzbmanj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gixhfcltz.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/ghfwqogrk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnnxarinn.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gyxorqyoo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/guviaelfj.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/glqosigib.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gazuqfmnd.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gtfijlmxh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gvaegudzr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gtmoetfgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gxbfzfenh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gfhtoivcp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gjyezhwot.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ggxaeawfb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gexoolrir.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/grwhdlsdl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gplczrbym.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gggtjfwsw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gpxlxznlk.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gtvvxmwjo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gindvmjpr.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/glnzqvfis.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gekxqlrdn.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gmgtcitof.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gamnwcdht.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gduusdxjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gsobohhjg.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gvgqcsrqx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/godipmflw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gshuyjjch.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gdctefggb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gsyeovpfa.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gvbtobqrb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdootmaes.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gybzqjljv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gzratxwks.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/ggtstbvpy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gjonwvleb.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gfvjykkkl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gjyywwhoe.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gffsrhacn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gendedgpg.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gktktcgtx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gekenxcei.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqviqgfer.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gzlrajhjl.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gouspkyrm.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwmhbgzb.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gzerebmjv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gnfknocpi.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gscdhrnsq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gduwtzadt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gerycfjwr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gppjdzqqr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwlaphtvi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gdnhccgdq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gofhdhpcm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/grtvtpsty.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/glvxwqrun.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gtkhwambe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gkvjjqhij.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/grhygtuvo.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gusecuhqd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gzzqckjpb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gfslrcjoc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gfupnstbz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gpwgpwmyp.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gnlzlfize.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gshyyaptu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gbuqzpmzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gyynzktsb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gcmztptrm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gsupxrtvh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gakjpjvqd.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gjikyzmxm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkgztdhdj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gwtaioyqf.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/geouobwka.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gkdzcrutn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gspmdrkdg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gnjpgukys.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gfhozlwbs.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvnxpfool.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gkgnsjtkw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gelvnafwj.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gcuphtgcm.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gpdyaayxn.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/goakyptro.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gomkdlfia.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/ghrnkxvjy.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/glwmidzlw.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gjosiwwtx.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/giejfgcyj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gouacyuwj.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/grcyfmsdf.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gwtezzrew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/grzcihclf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/guzlaphit.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gkovenmjx.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gvxsvaopz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gepscwvtz.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gbekhjfom.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gtewgtpnj.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gxrdjlutf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gciclaoym.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gmjbsjttd.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gqjtjxrcj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gljfxrisz.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gwvzudsdb.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gtdugnypu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gxfokoffs.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gfjhrorwo.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gfhiyhfru.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gdsrvselv.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gwuwyobep.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/ggdeqwtpb.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gltqdwlze.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpxuypxvc.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ggzxhutjj.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gpgrbzbtp.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gowbpjsef.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/glgiwgqxz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/grthbxybg.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/glwfjofig.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gzouxbjap.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/grgqewncj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gbhaecljn.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gwdspsuxr.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gjlslpyyj.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gbghdpmoy.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gzaxbqknq.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gdgfjrmgp.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gfagaxuro.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvpuwchiw.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gdqvptmxv.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/ggztyvjhn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gvnrstfko.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gztyorsxm.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gmczjrtbm.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gxvpslzeb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/guhtjvcqy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqfsowfjg.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gytegpesc.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gqikkqeda.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gekuvhojp.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/grfqdlwzg.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gblewwiog.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/ggbfhcoyn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gstisdmvk.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/griwavucm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gjhrjuasd.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gbyspxzui.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gasjmxkki.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmwuuclpo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gxtxtsdpm.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gvrilusps.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gbzwdkyds.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/grtgruflh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gacpxnqsy.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsvtzbkir.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gfmfrucly.sHtML


<!-- 参考信息 -->