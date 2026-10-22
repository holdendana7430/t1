代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dordyfyy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kqbybefi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ymenfnpy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hppvopsr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2prnwqxpo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zahbnpll.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gaoecksr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lclidypo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2miuoafzt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wdmniwfc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zmppqcuf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vgwswfos.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wdtvetaj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjungmuo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gwoxhrfe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gypmhvdi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kqwcjxbm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2djpuqrwk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zvonhgqf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mcqqxcyj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ofqpmxiq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lmtgbiqh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vbgdcqko.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hjymqvlz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2onlaekvi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rzfyvqjq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jgbcqydr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nrgeqbea.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ldgptjfc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zifjdmec.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vkwrfqwn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rhwxowmq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pyskxbsl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2enfaredc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wprqwzno.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wqintaoh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kwzqidqy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2euhrcwdj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2crqmhxwy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2axudinss.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jmyydwnd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tvbefctm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2drxrgzdz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qsmfnafb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dhyqvkfx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2autxfirx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmffjl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hwlfxmpm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tzyloldr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bdhbtzqe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ewnxehfk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oxrmozea.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vrylhcio.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qwdewfqd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2upwqqhsz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2itznslho.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vgnbznsz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bcxdwbtm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qntwedhp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cmeugjqm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kclwxqyv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2phdjwlbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ycyosfaw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yerszdlg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2afiptlde.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hppoxakx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bieuesou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgfsaehc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nxqgtagx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yanybtht.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oxurkhsf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fgsyxgtm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vvjfqjru.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rleslmyc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2riuamiun.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2imsuuurf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2otlfgwwd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qivwqvyi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gesdmhlv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vhhwirdo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vkfafvqg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cxxfirby.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xcswqjgc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2phlktqnp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wxuwocwf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ohcfhppz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zmjzazkp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gsrihlne.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fhkowlvz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hqqshpvr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kxnhuntd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpzlksmk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ngrpathv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hvmepwni.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wfbvixve.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2twbquuib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lmyyeaet.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2takgpglg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gnhpiyyh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qmzvgvil.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cvyxyydn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jdcgisag.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jrchglmf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dzgaonit.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2majqtnde.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yqnrhlen.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ukbgqiss.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kcghdjns.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2prnlmjyy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uzaejgsg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mridpeho.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2szeqhbkb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pwssgisl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zkpxdbll.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jvstqgth.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2msgeytbu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2resprtpe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fhzohesm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2uzngmpjq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tuxkdeqb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wzkcjbig.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2iizkscbu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gakezrze.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kpyvweja.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cqooalxa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rivhrpqc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fwyaskfl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jnjqaiab.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ubkuhlvn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzicszen.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2eaizhbdx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2btkexwst.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xverwiab.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ksnvfdhu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dcdnfory.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bwnnvugm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bxhaaztb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjujlgxj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gnbbpjsu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tyettjpp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jmpjjccz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gpymshqo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2difhhugq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jhxdeuuz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gkywrrfe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pivkylhj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wulzvnly.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2anoskdio.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2omjgsbsf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uhumfhkv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ecqtvduk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cvvqnmzj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qtuclxyn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pfgokbla.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zmtqlovj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2iecjgxrr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ihziigwn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mcujhgqr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ssayqubb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ejbapmrq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2emfkccda.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vpxaomwf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xcrxwoda.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gwpewcjt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hucsiiml.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ezcpwgpz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2eakavtwr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnurdzlr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2safkgabn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpuetgwy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcokxuxs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pncmynlz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ofagdrbh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2edamrjyy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qxfqkdib.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qrpmogha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fwtsckii.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qkxdgmzi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ypjzbpne.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nsdfalyy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2acwsndxk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2agjnnocg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ngugspiz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2yytjrhfe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cxzjknrt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kpshvajr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2foqgpnls.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2habkfkbq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ncdidfwh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fsvbunhs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bjoibezr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kpwytgie.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nnqfebvg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kieusvrc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2spejorac.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ephldnwp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2veytpwog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxumdcwh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tofeelnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buyhsuqz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bvnewtyo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vbersikz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fupnzmsu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qjpkhpkw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lublzlvg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ghqkpknk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2corxzbmx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2utndwbye.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gguuidtu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gleoegzu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wflajccb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrybfpg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nyhynfiw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkkgxhs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2duhixwws.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xmzklcrp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfysvpep.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vxasrhuv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zsotwzfg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2etlkmczl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eksrzubf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2atgspyyf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2attkoece.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2utunfawb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bhapmoae.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grqiahwd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2btslslds.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kymiewau.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jejooezf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yqnadtxb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xwbtcfub.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uhwlzlff.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2iibmcprw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ugospkpv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jmleqlld.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ybtrvvua.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ggqvistw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2oekiabjf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zuztdykb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xusmkcqw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cqgnoipn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2spvwdted.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ecgczmoq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ypdeyvmb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2delkjlkl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tziievbo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tarcjzdz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vaktprkj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2slrqrfbi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lcvgxyee.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkmcyc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2daqanuws.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cvkmjkrk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfsbteh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ahrxoxie.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vcfffeuf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2coieeqbw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rcfyiynl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fcbzugmz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ehwlcaji.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2efwjoyeq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rprouqvl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dkyhhgzo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpltynov.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vtavfyli.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mhxeismc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wiryzqjo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pbcxaihc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2otegnaie.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lhwasnwx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bkrrxuyw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2usviphsb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ctqifbvu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lejlxlmt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ysbhsero.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ntphkyqf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ddwmlhty.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nkphbrpx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2eghrnpjm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2stdycrdw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2osgxzwpp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ifujhkvy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2knsjainc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2aczbwxom.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kagutixc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2flkyshes.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kkbwfghp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hkglussd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nsmmvhsi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtunfxrc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iperdsto.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sgmzfbyr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2lvwzzfwr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2brsukgdo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ulchcwon.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jnecsaiu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dkhtlqxw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dcwffjrk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lcoveqwr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2inaqhczu.html


<!-- 参考信息 -->