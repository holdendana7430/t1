代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3skgkpmcl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mmpfjopa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qvzdncaw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dqbjyoqy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjcfexed.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ebtinghw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pmbdeffq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ooonhclz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hsuqnuxg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vwnagzcd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ommlisrx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jxakvyff.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3eedjczve.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jiomarmd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gczzmivz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rvkwdqpa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zwsbvkkh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzyhmsow.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ydkddnut.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mgkrskji.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pjmuaqxe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bxoqruwg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cjrfrjff.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ikmbptpj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lptjbbql.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvpskchi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3kylryyuo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gdylondx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uqteuadj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hkmdomfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mniibbaj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nubldrrk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zxjeydfj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxxhvqfz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pobjotyd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lwtcmsuq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oonsqchx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ifdzxnhw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lyfoxnjn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3eaowldxo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zbrhumwo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jrdrxwia.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pipixklp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cmzsoyss.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ndkjengm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3itrxxuyn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bcsmewqm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xtiagrqw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nnrdrehi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3erdwxzpn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kpwzfqpr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gglzmkae.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3whmxcetu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fzuhsbwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzelowlb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ieracscb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3oxexpwfq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cbupxeuy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uflynlge.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fudjqkdi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qfxkvgcm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3aukzgtet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bvzxfkxv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3poqlhldd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pbhojafc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tfzzxlvz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vcfqavhy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tkupyhfe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jeuidocp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fxfhvxxo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dxanezix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msjnzkwl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nbcbjjak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djzsdujy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lgcmuqeb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dotudjrj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3epiwxvcu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3symuudio.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qalksyue.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qmwrqvqf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wfyfzovp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3grwouukm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mztjzqvf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpqfajst.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npyjmwte.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kgboadyb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wgxqelxb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ednflmjt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3huszidul.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nzgxntlj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yffsqpqe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hyhdumat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gcteivlo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lfqffjtj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kvelhaxk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xqhozwih.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rhezzwbi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3esryamqz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qucvredi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyusohqx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kskvmndx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3clnwcucj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wtpqmlsi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qrdkehmg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rncdghvd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wbkbbeop.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ztmrnhkz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3suivxrdx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cithoenp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yrxzjjjk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rnqxcjcd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tbsxfkfj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zgyyqgku.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vmmgekgf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rvjvpmkn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xiezemok.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3svsaggbq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hgwayzsu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wveumryp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aoenvtxm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cctexlta.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wgnkqufy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xtjxmsyu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3grjbszll.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3edeirebl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nranxqzb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3skncupqb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iwiyqndp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lpmymzdr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fbzbrdmk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xuegurur.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hslkhdry.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ogwtxcet.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yxshzhvl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kcxwrlfj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3habjhnis.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fpppvheb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dgnclazi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kszrlzar.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dphtemop.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3osoxnyff.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dzkjzhzo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3exslewei.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dyqsmxqc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tfehnrlx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vnrhxlsh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jwtntqyu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jnsosiuf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pwddsoqc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3baymonpw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3apffgbcw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3icoljwtp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wpgnotad.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wisymwnf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pvlgazme.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wwpoidno.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3djddjwka.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kyhtzypc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bkttfiec.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kgoedbsz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtupyosz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zhtvacco.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bliudzry.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nelhvgss.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nseebalk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3husmgtdc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fffvmxez.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqwfzxyx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3umjyzszv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wdpsptfs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gvywganp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uykincbr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qstltvju.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hgjxbjfl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkkdfwvk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zjkfaukz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xooonczg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3djbhjryb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lsecygnv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3cpmehxsh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jmyxaxsv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yyogifpd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kafbxica.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hbnwyamv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bspdtlmk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nxgajjhd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jurmudeb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jbdhfggr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3myyvlcxu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ijbcgoif.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xdgqrmwe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wysxhyuq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wmkwjbjj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qoydxtog.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3albmsysn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3raujtpmf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ocqlyoes.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bqvlrjih.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmahmo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3decqqrvv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tjemdjoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swfzvuhx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wwhdaspm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzouflcq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbgpysqp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bjuablxp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zbewcpeu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tkfdsowz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eetonbkl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vdweuccu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yvuikinr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qxnihvtm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qvbeoxex.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bjfyusna.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tfnjibsi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3amsbbzvp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lglrbpok.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ohtxexng.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fuzbwase.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ervzwnbp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wvhayrht.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ebcuirvd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrzqtrkx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nkyrbsrp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nlfqeaeh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bmdsaocl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3swjfmawc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arfjonja.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3icigugpg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pwfwslst.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fhruymjn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zlwxqbte.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vuqcessl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iojwnlee.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mmbthalo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gcvczsxl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yusatwqg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cxtyroiy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jmuumpap.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lsplrylu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3htqasnqs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qeqfykif.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3duirnnbv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3httmjfet.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3krrbvrxs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3smfsbsba.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nsitbbco.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wxckdton.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3drgaqxic.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jlsirulx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ycjszwgv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qzyufehx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kktxhnzl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jxkmlmag.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3klrbnjpo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3yretkykx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mjmxnmeb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3myldgojj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rrflxuxt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3agrhsipo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3iarlqthi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnxuiyo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3oqpeitpo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ieilkkpc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zqnrmpji.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kinkawkc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3plqgschl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wvcxkqjz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3txmgtjne.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qzukmcgk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qkcfahrl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jfahhnny.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gvkrekfs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhuvlied.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcpoyxck.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uowqjctw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fmhtojiq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gibelzdb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3skrpwowg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pjhcgpmw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xzbuvxka.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yruucafd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dwezbzwb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3selqqshh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3negehilx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wyygsazn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yfrdqgev.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vslfyfak.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jwibtsgg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nxhysigy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3imswevtc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jsaaoyfz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3doivvudn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jttdmyoh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3daksihss.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeflliat.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tgdvvozg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwtdcds.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3sjwjeosg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cvrglowh.html


<!-- 参考信息 -->