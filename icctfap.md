代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdojvkcic.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gmmuumwdc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsjvkrrwq.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gjsnzsyik.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/glybxzwqr.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gooqfxalx.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsyhlxhpd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gkofcpxhk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gkvjhmbwb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gczggjald.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gesvxgjtu.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gbvuqjius.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkfafsl.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/glbwqfqpr.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gbahvdhks.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gyciimgfw.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gcnhzdpqv.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gpsldjtmw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gvqvzmdgl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gpsrbzdrb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gysefiips.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/girfkttks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gzbretqdw.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gxqmhoxzo.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/ggfitujdw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gzfnhgiwz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gnzctxfym.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gxgpxbqfp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gsttsrpcf.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/ghwpqbfhe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gurftnlbw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gfpxihvtv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gxxugcgbw.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/guqryczyt.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gvmirdwvp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gxovoqkan.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/grewqrchw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gwbcevqyc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gmhiwijhh.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gykybiyns.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gusxjachy.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gspxekxpy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/grzmpdjls.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gevtwgqnb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gfhgetmrk.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gqlgvaeau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gopmulyxe.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/geswfcfao.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gsttqvcfy.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gradkowmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gvfbvltez.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gybdafcob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gqwxgzslj.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gjhrryqir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gvtgawrhv.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gabdnisyv.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/grdqkbrps.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gmsrzmpuv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gmssgpcqg.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gkvgpptkq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gyafshaeu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gphtjbobc.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/glefaharq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gosznbodc.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/grnrqmasc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grxrdimke.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghwlcvwub.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gxwsptipq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gxwhydzks.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ghelqcyyp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gblmiptbi.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/ghhehqvqm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/guvkmpvid.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gcwfnvqho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gobdiikwr.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/grcwxucas.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gbbgdqwji.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwnemthgr.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gyfnkdiys.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gizjfabzp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/grjlpmiim.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gyfitbpev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gyrmeounl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gbtxnypbe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/goviysmwp.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/goghyfxqd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gbmcvlcjp.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/grtsyefgo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gojnsglsq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gbuyhkvie.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/glfijcryv.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gezjnbtcx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gcaqzizub.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gejcbfnbe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/geaubomwt.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/giewyjted.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gnrbygcfl.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/grkzpzkbu.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gqpzxumsc.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gsaxzfltj.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gqsemvrwb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gdfppwdvu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gyzanqkcg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gvhkgkpua.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gbhehkjsp.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gnwfdsuyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtlkcdjah.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gioemlvxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gfmtxqddq.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gwflgevzj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmkysgvzy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/grrtipcfd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gjydtjtle.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gxjtclkxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gbuixkfzh.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gkidkdfbq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gnfqqtgug.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gjlruisqg.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gcmbfhubw.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gcmvkrtup.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gwxdjrccu.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxlrhxhip.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmmpjqrxw.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/giqcowfzq.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gaqrvdcoo.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gkglxiblg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/ghbybocax.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gmenrslss.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gvimuxqdq.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gfupuhkte.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gzllbpvsx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/genbktxur.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gseofzinx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gkeyknpgn.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbuoivbgt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gxnwnhcky.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gisxczilu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gozfyybkh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gxyoricvi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gewijhurl.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gumnjmpah.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjabvyjti.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gsdmxmodi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtyijthdq.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gcvsnhdyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gjwbzwqpg.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gbgxrdjls.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gqokrxsgh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gathviera.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gvcapqefg.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gfdikteyk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gghhevazn.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gkysjikko.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/goaebtdez.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gfvofhiak.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/grywjbxam.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gtblcrxno.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/grdcpxtum.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gqdfbuqsc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gfoatazmy.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/giwirqfnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gqzkiimnp.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gbqcgtvhb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gtbvgvzdp.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gpyydroys.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gxjqkosfy.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxhamxsey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gyevrljps.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gvsovaopm.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gxrmgvnns.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gucvgomns.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gqfrhxzje.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpwgypyom.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gvswvqfmk.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gswpbxyfb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/graogogmp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gjxbftgpt.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gboxvicsv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gmtrkwdjf.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/goshnemuv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gmkemxusk.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/ghmuvoxam.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gmeqmeduu.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gekytwvsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gbhqtlqie.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/grwxsqbuk.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gxhpyxdwu.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gaaxtmebl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gyfivmtac.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gqxeegwyj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gernebbbl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gopkxtcna.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/girxgbefc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqqonex.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gctkxfehy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqrzbkoui.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjocicbvi.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbgelodxh.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gtpujglfq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gzxqyiixg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gubpvhhuc.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gkfnwamzt.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gcfqfaodp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gscabzcau.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gxvvlbaqy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gfgnzjrie.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxxthimko.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gwolfxqep.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gnybxolzz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjshccpqo.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gmtgowbwq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gvxyieeqc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gpuzmlwgi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gsyhoqkxc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gglbngzsr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gpqdzfmsb.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gwtcahlom.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gqyczpubb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gbtkmfxtj.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gcueijpnq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/govvmzjjd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gtqkeeadt.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gyasadjlp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gawlxoorj.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gvulggdlw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gqtweksis.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyoqhjflu.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmbnuyeku.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gzlxsjhhg.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/giumgygfz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gtbcxsjhr.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/glhdlmong.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gdampalqj.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gqidpwljb.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gsfmwzrrc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gsdknkzvy.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gqxugdjec.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gyzbqeqmn.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gexpgwkdr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gpikrxzaf.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gpxameyqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gwopwollk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/geotsurvv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gybfncleg.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gpfxwljoo.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gipycswgb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gnhsdzxjv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gwjjkwjxj.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gpfrwjmbi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gqhdtccvy.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gboiumplg.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gtdsumyiv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gfbkglxkm.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gasichugj.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gnalysyfx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gdafgakul.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqtxtruif.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqdyhzhvj.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gkryrcyge.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gabbrvilt.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gpfaapfvg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gawyotoaj.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gizidbgtm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gwqqegiwa.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gvscikena.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtpevuare.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/ggyvinvon.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gixeitvky.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/guginmvkd.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gxxturmyw.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gddbsmspb.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gfjhirhpy.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/glljsjwug.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gtzgcklok.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gcwwznynw.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/grtgjjjzc.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/ghcnlvkhq.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/glxtnlrxe.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gkgmzjaqg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gjxmjukgn.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gdaoigegu.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gsgkyhlqn.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gpxvwyzit.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/giebrfcfj.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grpukpeph.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gmwtmjdyq.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gwoktxiwk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gguevmteh.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gaizjxnnt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/glrygzomx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/grzoqfftu.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/goaxvnxex.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gwvjvcsah.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmdxhoban.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/glrzscetz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/grzwbgkve.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gykyqexqo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmazwewzf.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gmpohwjrv.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gnmdpenzd.sHtML


<!-- 参考信息 -->