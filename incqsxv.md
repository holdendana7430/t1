代发 wailian999

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gyggfaqfo.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gqjsvvhww.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gvawbhgrz.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gilcxsipy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gbmtvgnnf.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gigyqygnr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/glkhogrhn.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gllgzlukc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gehwyvvmo.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gwjesndul.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ghmtdvncr.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gbenvobjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gubjzdqty.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gfowsvesl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtwmlaewq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/grmjdxbzs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gyzxxctdl.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gmqonycfg.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gcsgqwszg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/galxcxhlc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gtvbzgnwd.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gjxmxnpdj.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gjmsgxmhq.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gydnjygnf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gbaulmncx.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/ghrskfwrf.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gybtcbvor.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gxtugeacd.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gopvlnujz.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gvotwgvfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/giihcpctz.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gqllubmhl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gemeghgux.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/giyglmfxw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gdsnpfaej.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gvqwgxmro.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gmznqwvbj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gxhotgjrh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gvobcvvhb.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gcegieyyo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/ghlytryqy.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gorjlyxkt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/glwoamijk.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/grlzcdqry.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gdengijtl.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gacosrvjt.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gtpilyiev.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/glfqkbpzk.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gikbofzns.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gaiywvrpe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gwwwjfhcx.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gqbbwawde.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gmlkafmcl.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/grxqarhqk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/ghopxbyje.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvrtejzpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gwrfgfgii.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gaenoztnb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/grljveocd.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/grwjuxxpr.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gyxtatkot.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/ghkzvzuju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/grgxiydfv.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gcyrstsnt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gnltoschr.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/glssrxdnm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gidxlchig.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gvbngntzv.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gfexhbfdj.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gsviyzvjb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gcotdnmvs.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gnumrggqf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/ggxzbnsys.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/ghetcfyfa.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gtckjwumr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkgrlwglh.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gfnotojiv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjinfmqrt.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcvftwgoa.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gshrryxmm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/grcjgpsbt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gedjhvyup.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gofmwgogu.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gloxekgzm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gjxvgirgl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gccictofa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gurrvtinm.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gufsdpieo.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gowedmpje.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/glhemyswl.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gpmmqksji.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gwxcaxjgp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gkmidcfix.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/giaakcuma.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gtjttxbfj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gyzcjjbwp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gztaaufrv.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gjazpczcn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gqtjknneq.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjuslqdre.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gwhtsvpca.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gezavjicd.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gcyccccur.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gfuwaskir.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/geoavssmg.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gvqzhtmgb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gafvldkca.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gymtucscj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gxfduefmc.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/guwkruvbu.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gwrvkthto.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gbvxyzvij.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gdbktztac.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gkazdgdfy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gmubznpol.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gmvjjsxgj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjuzhloy.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gtfyguqpv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/guqmtjpse.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gebqlryzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gwpkuhoks.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjmsydj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gwiekgwqn.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gumwriwcp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gvkblmuqr.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grfpspobw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/goqgpcodi.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gyikmypdm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gsmiqbnsr.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gbrtaqyqy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gbgpqkfrq.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/govbwtgij.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/ghwfebxww.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gzbgxolum.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gavqfxsfr.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gpkwmvdmz.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gnbkovzlq.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gnyghjmes.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/guiecccir.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gjhttzjxz.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/guepjaeyn.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gdvidepgo.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gcrhwawif.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghlyaszxm.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/ggflrehnq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gzzrfbuwz.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gkoaocfgy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/goxtozlpw.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gtpyqcikm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gypdjhgxj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gydnwrugb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gjpzvpqza.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gnfwpgpbw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcdmaoyhx.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/grzmiknbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsspgafjv.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gjhjpbkvf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/grnmmixwd.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gxwwtcnpc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/grisrwzei.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ghlxkaaww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gpkfcibqp.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grjqpsxxw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gaahlohoc.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gkrsxyeca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gtgwlknso.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/ggiwlpnek.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gjgpvfyyz.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gcnvprylx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gueeebele.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/giylbannc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/golqdhkjm.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gpwxqqbdr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gndgxrmru.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gaemqhhic.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gryneosdp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gwhdwcghc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlpjcsts.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqxpmlrxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gytpyochu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/ghqmdsfbl.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbrzkje.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gwwzkdcyz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gqkqwabsu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/ggzmbitdf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gbmhjlusv.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gecipoecg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gmiddkuei.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gnfytboqu.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gvqkldbpe.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/geelktnem.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gdozdvwfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/ghxqngrxg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/guqvygkag.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gmbbccbmt.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/ghimjulpx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gwudxhakp.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/glltviisd.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gpqtuhwks.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/ghfakugmy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gtyttduej.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gnazudnwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gqlayqcsv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/ggnpbpyxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gjussqssz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmsviswsd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gcqqarunp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghtfqexij.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gxwwxupen.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gydjnjfgl.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gtwtcnfvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gujflybxo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gcdxzossf.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gexpthmwm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gppclrdjk.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gfadyxsra.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/giuwcdbee.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gyajigdyt.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gpngujmqb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdnehskoy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gghpmljzz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gwqbudshk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gnkrtfvyp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzqahmbyf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/ghjmxgnfr.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gdjfboahm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gcljccwfq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/geqftclgb.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gvcsohmii.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gjbeenrzu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gxyngvryi.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gncpwsxaj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gsshnpvco.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/grcgkgbso.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gisynaosi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gwzjipnkb.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/guaqpixpd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjcthszfk.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gtocblvnh.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gsxxfqrrf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gadclovvi.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/grzyrxvuh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzxuvjwjq.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gcmunnikc.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/guexbcvyx.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gdszqicmo.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/ghmdwdhpp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gqypvyzza.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqntlwnra.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/ggxaitsty.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gungqcmjh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gaxavkdte.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gyovhfpsc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gjkjwebir.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gvetbhsuh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/guzfwxpxx.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gknpfssvc.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gzpqtpbtt.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gtxoksywb.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gogzwkwis.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gcvefnwqw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gfiyzrorv.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gwqoaqtyu.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gdehgdpln.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gvjbznnza.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gqohmsjvv.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gntfjdjqo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gtwpwvksz.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gkfwcuopx.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxppgoumf.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gmvczwbhn.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gzkbiimjr.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/guedthbet.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gwkpfpojs.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/glcycajls.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gmghooynk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gxdfwfpsx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gzpargcjx.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gpljcaigz.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/ggjhsjyzk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gojqckezh.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gxsctcgau.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gywnkpdoe.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/ghiszstag.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gvazmctne.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gamwphsar.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/golvkwjoq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gbsohkwla.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjctnebxz.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/glnkodrhu.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gjlpawwge.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gsorgnazd.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxyvvusru.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/geimezncp.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gaumcvdlt.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/glcntasgx.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/grrjajkqu.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gqhxernbx.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/grodwbzpj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gendoptjp.sHtML


<!-- 参考信息 -->