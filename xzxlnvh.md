代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaivgovix.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyirbxkm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjnhtdcd.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyhhwxiwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/glhxrldyk.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gybiozvje.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfqsjdtla.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gknzsvunq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gsghktrom.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccdevlbx.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glksqqfjq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggumhnjuj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwzysnsg.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcobmsatt.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuswznky.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoukgqvu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gyzuapptt.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwdaulllc.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtghidwlm.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gezcotpzv.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/grfokenxy.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoottaun.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gsupscrtj.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ghiztxeir.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gekygabwi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gysjmenva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gsyabuvgx.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpkpxsm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjowuoxra.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaanmknyy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/galxqmvfc.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgfxuyfa.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gliumxvuk.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaikadkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpbsyhs.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gocyjbxlz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmfkzsqr.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gurvqeebu.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnzwtnjq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizkfslmw.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gclvgnxhf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqonecomm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gctgfitwg.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gfgigioyl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/guweuqojn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdstuvekz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwyznvay.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfyxmfcqw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gaiatbahh.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvetbscaz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowfgvgj.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gecygomqr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginryhtse.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbrvnrwpx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghvhiipyl.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grzfhbgbc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkulslpqp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrneosys.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzwiaban.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grteiamgo.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnonjsdq.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gmjwurbbg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdbvztur.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtsydpv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjnbdpifs.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gjkmgsgif.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grslnrwlv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxrthadkk.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbxlxwcf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvclkltc.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghckmxwgq.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbuvylpl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyzwrcrp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/ghoxluamb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnmewidji.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsnxsibf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcapomlff.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsrzngvi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gojovfitl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyxwdhal.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfofipvn.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubffutk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsngxuxx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/goginglxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gnizfhynj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/grsdxygly.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/glnmuhmnm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gahehouvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gcovfxehh.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gaciuluvg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gsskisvhx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohqkjqnb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gynkmpcex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmcocfz.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhmdczjv.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwckdxtmg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqwjsveb.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhbasabu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/ggzrjzbvn.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvawbbyjq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjanhpzv.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwxxktghx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgouihyv.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gofxavhix.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzrcihod.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgyaimaq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gifolegir.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/guxgtlaex.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gykuatwlw.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gsscfuxde.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqenuwwua.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gffmawuwh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtrwsfqb.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gitxpdmrp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjxvtwoq.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gbibfudnm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcdwjjdn.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gawrankja.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gpcxbzucs.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbwkhtyeo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gpyblsdtg.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbgxaemec.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxvlnmbf.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gthtcvvtg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gdfxslcws.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxewarore.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdijqyih.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gegfadsnf.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixpqcszs.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbgifqqra.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gbgpqbkeb.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/glntadnxb.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gndjwjiyf.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gswkyipft.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ghayftwhp.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvcytney.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gggifbruk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweqkvdpb.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ginrrvxwr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfgiynyk.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gecguwqsh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gonodxazj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkgehovl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goydryymr.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxomekbp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmenlrgqd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcstpijm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkkeakleo.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeeacljh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galnkdong.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapzeuipp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxukmrzn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghccscwpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/ggddgpkif.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genpfyjeb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxphxxopm.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxwqtntdr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkmuzrzxs.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdtottdmh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gulkawhia.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkjxwjsx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmslimb.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gevcmhwff.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkfuvkqv.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gidnjrzlt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvongfkia.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/glywcmhno.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glcgazstv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfydmrpal.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcullcvp.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjpxwuqhj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gziugejfe.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpffkpuod.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/grokpsiao.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/ggcnjnaqa.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/geyfoesxb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gcllyradi.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxljiwldt.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gevmisalw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gtijyuork.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gisusoatk.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwutttnp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzertrkvi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnshtqzq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gikyydwjg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gjesslofq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gbeapnlwb.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfxdbvxm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsdfwrezr.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/goqywbwkv.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxohiays.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybciitvk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdvkozvch.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhifnmlu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gtiwhaqek.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmocyubgv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmznewsr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqsgjqxft.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfxydcef.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwdrscful.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstpwzmq.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrbedbyu.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjhngkxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gptltwfle.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnzebshb.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gijkewrbq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gqhplgxmc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjauwiln.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfljzdg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gdpjxmxoi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/grscgpgpa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpydhhdnh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gyphqxjfb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/glusfzmsm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/genprhjqj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzyqftfd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyoytaqqr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbehrkei.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkurecsie.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyazplfof.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxxmuvsv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxplbujk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbfcmel.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpcrnuxi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/growyvnji.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxssmrnka.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/geobcntzy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeygdykw.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gaazmjxgg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gqaaylwdw.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwlzlcsd.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcskimpzo.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/giojhpygq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhkduvzg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkwmxzgb.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgjsjpcq.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/geszpbydp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrdbalmm.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/godnyijhw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gxeyhmjex.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gjnmnnqcl.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gweesohwq.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggssbsgyj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gipgdfmmb.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhaifjvn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gacbpapdi.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/giecboylh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgkaztpo.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gpxjgyzcx.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjfkrfkj.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gazqgymbo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswkmtndf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihdswkoo.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxgzsuea.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdfoqwlw.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyoovkqo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ggowujyim.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxyvshpx.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gqocerbfq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gksrblvsr.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfoohdxzk.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsylyvnjf.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbodpdqer.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghkbpuube.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gzswkrymo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwyzwagj.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gfjfzilar.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgqdwmgi.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gujznixvb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsjygija.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/grpnxnmhk.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/glggkzgsg.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gjocioddz.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpuefmkgm.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbnuzmyms.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gxxntyuyd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gimzjenzd.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/glzmeoecl.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gyifygpoz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjywhsxu.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbcblcktu.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gksoonnfs.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzugxngz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gllcdcgvm.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gxbjvnwjo.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/glbruzorp.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxpatulv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhczdyic.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnoxctqnk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbsravoks.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblnegjtr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govapgjyb.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gdecqmqdl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxivpwowf.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geloybuba.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gxscsxabc.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gceysqhel.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvivnfbbf.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpzqznmpj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gyllzhzjb.sHtML


<!-- 参考信息 -->