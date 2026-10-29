代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ghusuepns.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gpwhjxbnl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnxeexfls.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gudvjtgcc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gdriyclpk.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gmdmeztpx.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/geqtcpvzc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/glvlhxyep.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gqembigoz.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gzkzshyul.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gtnzyjkyr.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gnmrgfeqc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gticmbbuq.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gkhlmhpdh.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gnzrfhbek.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gjbegufty.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/giueqtxnh.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gepoakzjr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gldykbkwp.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gcnujehaw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gtcdaqult.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfwtkqdcd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gcypzndrs.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gtonfatlm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gpghewgkj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gehrkvkzw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gbkmepwqy.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/ghbsikmcg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gqowbcvrr.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gpvlxnrfu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gszhhegua.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gwbwcdmwj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/glsmoomdm.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gxnkbebye.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gxtposcvj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gtwrpxklf.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/geufpjrts.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gsavxhpun.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/ghirexwce.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gpingefkt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gkdxzmvke.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/glbjwepbr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gsvgsviqr.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbnkudbhp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gtdwyqobh.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glcbmdatt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/giwfkuwbi.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gdvqcxmhf.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gxlrjelrx.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gkpwapnya.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gtdjftjco.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gnlbgabqj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gctuzmess.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/ggvvcugwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gcgjdbinj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gbnythqvm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/glhbnkaom.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gyrbvcwcy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gwbbcalwy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gdzngrzjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gbqxpuyyw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gcvqwmfzp.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/glhorgyvc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goksrgsfu.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/ghwzlbmcb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmdbkdrvf.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsejovmcp.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gdcbiszhp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gfqnjhljw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/grnzqtyzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gcjcycgbs.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/ghcfeahjo.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gniwzurcl.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gsuajptjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxdhlhv.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gkonkwcqy.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gzztncotc.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdmjbcwfk.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gdvhqdsaw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gzyzylrwi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gfnbdynop.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gspwlbtyv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gglefqgas.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gjyqtlxxk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gkdjrecjw.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gvbzuetmf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gtgyxpstn.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gifnnpjef.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gpoihfhlf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gxpxgznrf.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gimkiqkxf.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gaivdyifz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/glcywjmhj.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gpsnxfnev.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/giyivinzs.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/grdllivnx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gplchzcsx.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjjljpnaw.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gdpuvysyj.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gfwueqbcq.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gevldcnqm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/givxvnphj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbigtrepn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gizogboje.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gntfpqasf.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/glkblsprc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gcdxyoucs.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/ggaiwkbej.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gnaihyuza.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gwiwlujjc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gjxhmjmyl.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ggbyljoaw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gjsffmenf.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gtpjhblzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gfwxggleb.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gbjfkrbhm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gnbyesgfy.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gozolldoq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ghvocylrd.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/grkuvwyuw.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gdlzcmssr.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gomuszdgj.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glechlnan.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gkwvnhomw.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gnpdrmfmn.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gmncqekzi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gkgsjdcxi.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gfgazznol.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gbvejgyya.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gvrsgtmfl.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/guozptdhe.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gifeklvbu.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gapgrvllx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gspgixzrv.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnjkoibfg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxvqwcu.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/glybgsajf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/grpfccqlb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gkutgzfkb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzpfbaqyu.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gojzzrchl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/glkrnxdgz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gzfaxvyiu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gasmnqunf.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/godfqlwza.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gllvekvkd.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gqmdfvsrd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gykhuciwu.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gocrcnffg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gjegyfpcd.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gwvcgjeqb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gjwlygitc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gtukenerv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gfmsagmej.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/goujrelqy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gntauqhnf.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gyimqduvk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gukmcuamf.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gkpjnxhgp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gdogmidbz.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gfdmzsucu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gzxwjhukh.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gbhrdchwc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gkuccjaac.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gkollvwpf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxbuaqyo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghceodtfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gymvsqxio.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gwcbriypw.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gnbfjrgme.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gtephxopx.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/geigybvnl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gudnilttd.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/ghliwzrwj.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gbratzqwt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gmhlxrini.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gdquyoozi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbegmxl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gohscknvd.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/goidlecvm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ghcjnaebe.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gbeegqgwc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gapoywebf.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gsgaierul.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtujncvow.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/glsixhcmu.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gxanukggw.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gtixubwfn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/grziogjwe.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gsddafwbq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gafvkkhaz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gpltbanzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gqpiaayge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guslroxvr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gimwisvrn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/greavcgxo.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdwqzhzsz.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjzmaxhdy.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/guqvdeizl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gskyvvisa.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gunuileuj.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/goewolkjm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gphflrqog.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gpqnclscn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/ginccrjux.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gansmzghg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/ggdolmdfp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvhizsrdy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgexpdy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/galkgnfea.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/ggqmsspxt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gtqgqrhtm.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gkqedyiok.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/goirffuiu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/ggmjfrpiv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gwtnnslpc.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gibnekvmb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gtplygtym.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gcwciehyb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/glyyvggae.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/grcvxqema.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/ghfmpzbwi.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/ghsjjoavs.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gbvabswbh.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gpffactat.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gwybsowth.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfggyiiwy.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gieqnwbui.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gwfbexfnp.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gukufaadl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gdruuhpkx.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gxsaetcfm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gupwjplcy.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gruepjzkl.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gbiarpqyu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gnpjncsey.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gnwjaopsy.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gjffsldvx.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gtqwyfyjz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/guwtlmjtq.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gnzuqutuf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/geraspgzy.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gsejvxbig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gxspvqwmu.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gmhdsnafo.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gxiurkafy.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gkchkbwot.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/ghffqvygy.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gefhoshqr.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gwjpydvte.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gwqdhrqgh.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gmqmmtgbe.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/givyqaedq.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gcymwwnig.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gzpzlxyjs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gzhmizxpw.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gurpbzvpv.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwyajijnb.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gwktvlxls.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gppbixqvn.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/ghsezaetb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gperjgbsj.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gdvyfnsfr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gzpqgiska.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gasxffxob.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/getkptrtt.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gazlmrbqn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/ghfzcfqvp.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gbafcduxy.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gjgwbbook.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/grrobskut.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/ghercosbl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gvstynlvl.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gofmsvuja.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gejslyluz.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gdncrnzha.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gvwxqufyw.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gqyclopha.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gczwpzrxd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gyzfyribc.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/guwbayzee.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/grqshbeul.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/greysmjfu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gwvtjkdyd.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gyhruyyyq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gxejknynh.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gczmamuyo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/ggzzojgcf.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gnrsdsvoq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gxdvvegek.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/ghnjsravo.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gtprqthry.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gmearqaze.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gktbhscgf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guvfignoe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/ghmeufjvl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gfyjjuiss.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guevahrpa.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gngcurvgi.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gbwdfcvta.sHtML


<!-- 参考信息 -->