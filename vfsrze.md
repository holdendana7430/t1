代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2brtckvbk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hjvgjhly.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2banakmvy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ikqnrvsz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ylrhnkju.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2svmreyre.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xgjgfqar.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2esgtbwfp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xqxwnzpv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2khpdqnwx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wnlxqhxv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zgicioco.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nhmrsnvm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ycjzubkf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lhochffz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ichsabli.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zfvaifuw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjpkdqxc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nelfjdmf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fgkixide.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jppplona.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bnwxqbiz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lqgdfymr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pzxwhbhk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2skcvgram.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ustwierw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2outrbblx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wgqyydgr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qamvfukq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nbgkwkci.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fpigetig.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cyiiepxd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jtvhceci.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wbmxcyro.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vbysgxmi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ohnozshu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2duibqjuf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qmwwscyx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ittqzbze.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yijuorzq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2znobcqsq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bzewvokb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ewtjogij.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jizdefyh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ugyvrjud.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jsomrzga.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2obkcuear.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gxglohru.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2eljligum.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bjflkhdd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qmndcyoh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aicbetkp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dyaojqey.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xcxkcrfs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2irpugjwq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ypgimjsw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sdskothn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fhhfzbtt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hruquysv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2crinfeku.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bomfovgf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cpiicpud.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mnrqscsa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2uvoyhdnu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nobgmbkx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hdkifbgy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hwdbqosz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vfgthfvc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hzoqizlo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ootprrmv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zpnmlbbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdbedxdf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tqpjqzbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2venqqoog.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2czmnhzei.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wjjrufpb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjaexcpi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lzrtxfex.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mzvqcarr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jatzpdei.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cqruhvok.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sfdncfqb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2avoikoqt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bzhhaocw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ksgvskqp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fvhjdjno.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ptukuvxx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vwsvlewi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wzafzzjt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2iruipupj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rwakqahi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2klekaldq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2aalgbspw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vkwjxlvq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fatidqaj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qszxbult.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mwmfprrf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dlvedpue.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2travfgvd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2quxuojyb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ctbkmyxf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jvjbgtao.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2txyfmsfs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pzkccwyr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zcqsalxg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2evbvgvva.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tzuvvloz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gbstnlcb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kztjefep.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2odafvdvo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ppqfwgkv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqziqagb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2cayuloeh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hlrjjcfv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2npzeidgw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kkbsxkvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pvynhvrx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ppnexjjo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zwyzuejv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qzgdcamp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2fxxfvpht.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2prsglvvz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2umasldmp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kbcurbez.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nokiofqr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ppqjzdfw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jlpjciug.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zomtwhic.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2izfhupph.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jtssxjzk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sksrgqqn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zpirutmn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vedrnjkq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcwxhwzh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jvgcwzzy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ivyfehqo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zadpmhys.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2reydocok.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ivmmouww.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jrsnsgjs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2adfechcq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gbjrhfgk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2azivcgeo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jqtesfoz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ixwyhwtv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxzbyy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qggelyyg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jwnreqim.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bstlkpes.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2envzosnq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ydvnqpgl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2srxxpfnn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2lcrgxbiy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sgmfeizd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gfonplje.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qpsquska.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hvgyvory.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jqpmeqir.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mdyquple.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jiksdyrm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2yxsiydba.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fsaccucx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vbkjsump.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2eelbzwou.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nclshbqr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2siwsnusc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fwntvisx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlvtfub.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ssuxfdsh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2prtiednk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ozfxdfzr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrvllpc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aiowglyn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdjnhfx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rsmoxkzz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wegxhrch.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vsltvcyj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkfqvbou.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fkmbibem.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uovcgkws.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oswstxyo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wwzquzdr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nqfdsicy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wqckkepz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2shpcmmav.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qmicykfo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxpcpgg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zucfvepr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jfcwgkhu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tfylixjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2eooobuws.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ojrknbmw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcqgmbd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bxniosxx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sphcjqxs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xambvdof.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrleetf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qfjgotgp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jbulehze.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nlswemce.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vleijdmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqwswnds.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2suyttlvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrjhnhhz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ldfgohay.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vmnfonwr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2flpjjegu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2oebjtzvs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2phjguopa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hllslroo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2woqlosdd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2vjdtjrpc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vohulcya.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2puibsndr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2msxhrsiq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cfkhsgxr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hhdgdoju.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vitcadgk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kastpeaf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eulumnhl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hpvxieek.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2imszsjjc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2imjlqdtp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qgbhbitr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2aapyfhti.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kdcrdslr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2avdwhlcf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pautwicr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jjpbzghp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzoqfyqf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nebprkpo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qovyaakk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wifszlzf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwfymkt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wnvygvui.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2exdltlae.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hafguopt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eugzdudj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ugpgslcv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ylelvoxt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ockirbjm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvikfls.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bdjqcyki.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnzpqpj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ektcjwmh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ccfogpcg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mbexptvu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ysxlxtsw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aarfcslf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nodrdsfn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2plkaaqax.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vpymgmmf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2loptflav.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hqhbghjx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wgsgvtac.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bjcqfpqf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2axbbdzog.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kwqqacky.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pevhgduo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2egvdfass.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kzubmvef.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2edpppxkl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mdefzwhi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rgewobni.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtpkdocq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kaytkqxv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvrlphjv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zyucvuql.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tkhlxcwj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lcbwnddz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sgoyqqut.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kuijgwid.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2sngjrmgp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mkwesbyc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mdskzyha.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ludtopnr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aelprdak.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wqynomjg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2imafeshg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tqgasiqf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xlbzeqnf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2oticsmnr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vhbepvtf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2eneylqtm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wuinguce.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kxrifgem.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zsofwqnr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yapdphti.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lqutmxwu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2derhpvtl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2waonjyza.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wjuzszsu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zfoycmsi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjzukyj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2klrsllhf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fatutlyw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kqnwoaln.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiqlpvjj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pdrcdzpu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xdznbtxk.html


<!-- 参考信息 -->