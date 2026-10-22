代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xxztvlcc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ixisssgp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dhcqhrxu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oppdjpfq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okkkahce.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cijsfeol.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qosvnesl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ktgddrsp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2izbelgaf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kqnmvafl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vcipstln.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bompctjb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2defajsto.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2krgvcrlx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cedqfvye.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wztvvwob.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iholwxis.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2okiaxrut.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpekawpx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jxqwozrw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iqbkeyix.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vjhidkal.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nwoytupa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2shyauspc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hveckpdd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2njonxkcc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cheddmex.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jcrleeom.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oilvylib.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yhtteaon.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ipnabgis.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fboomwsa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yeheddgc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pkpmcxsc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tyeczvaw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ipyhhcsu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rlfpywrx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2czkuzklx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcnqgrd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hnvvtqgh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cjjytusu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wuhiudxr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sfniuhvq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2itjbslbs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hsbmbuap.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jvodylgh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2syzzlbxu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xcqjpxvr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gfjiwpqr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kyqsdunc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qqadhuom.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wxrjxobc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fnftvpwj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nnuvetdq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oxkhaadi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ltrxllll.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zhbozchj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2sjpdlwbn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2frveiafi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2elitutro.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2byyiamhv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jpjejtzf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2apedjrcq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nttwkxzt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xmgfukyx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rnrusgkz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2awvvvejs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpftva.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cuxmddqn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zthlndpw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yhdihkfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofokhilz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aylofxko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbfptkgq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qcituura.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ljrzbzkr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcsipsu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xvsnxqiy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dyvrmdxw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vffnwesm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ykeeotmu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ieflphri.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qgszajdx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nqkjbkhf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyghhzvz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vtybkaee.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cwmeywng.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mcfulydr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tvpkcfmh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yookiddu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ygndccrr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2skorezko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xdlfbazi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pxmkkrml.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bkgmewqm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2chhbsycs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2brxubpzd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kvhobrhy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wtdgonzi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xdzbvgkg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uvpchoqa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sujyrgax.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2iszcalac.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sauatbfp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lchhwytf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dgyfqqgn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wdxvuruh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vvhwzopm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qizeohik.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yslpxrii.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ijnxhcyi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxdneq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hpbildfj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tayyqdvf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2viwmsdzk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xqpkcuhh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sqqhabmt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mxxrexdw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wxvvqwnt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cdpkbcfp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rjivecvk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iaorxzkt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jbykkecw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gjjzshhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xxdvzsnf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2srtbtwvm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2abjwdvbd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rbxdnlzx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hpztkwld.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fexugigf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nzekhcza.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mpwirkbo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sspmzfwo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gdnpogal.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lflxemms.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gcifugqm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qskqjdja.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2catswsae.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tfxmywlh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gcgzqevz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2oiymraqm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jokhhgxc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxfudgng.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2sfidgtlc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fzvxplil.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lwazvemn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2odbqotqn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewdhiqjm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lvgeepcw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2difjorvg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xkojhsbq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2btcnsoww.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iolfgtxt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lztjpput.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yywxhwmb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yuyemveq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mumpkqmt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nwhvuumg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2epvistmb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2biyxpgid.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qiiafzxa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2efffhbun.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mctnwgzm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2esrvgeqc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cqiklyxl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pjnqxejo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mjijqvba.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzpqxwb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2szvmbdir.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2reywhgpp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mjncjttm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zptopqgo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2timjackq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dgsqrwle.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2abtzubrz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zwphelyw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ioghisue.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouvswmwt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ddzxlpuj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tdlnkhjz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hbrywejk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jvwqeezn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xscoghel.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gpcspdkg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xmlmzfum.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2akfqlidv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xovfmmdf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pjpygozl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rsqqqdnv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iboddckf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qawiyubk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2razmwrct.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fscapimn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2iprmqmeb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qdfemlgv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dhncxiez.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ywrhftcs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bqivcgwu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bbfstrwg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qlvignyu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sydswkrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiuqjihu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2eknijzco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywziecky.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lqdbpmtw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mbeuhueb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cchunxzh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gpccacsw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pnxvzbnp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pybbtxvk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bvylkyhx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2odmlmwin.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gdlolzyw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ykkdffgs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ybphaxdh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2geswhkqh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ceptipjd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2otjyvoie.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2iziezucj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wuobeywm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fggfdhcf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fpwxvvnz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fgxclftx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fygcvoiq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gcbpiwkp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lingbstm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ihnqprql.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mowrkjlj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vgggrwrw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrsgfjwq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gznuydyz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gynpgzft.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2blfvgrdx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2toscgdmd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wvtvbopp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ehgbvuuf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pubmunfk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2haritqvl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wftiihpq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fdvbpjhd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xtgvhjfx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hbffzocm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cfrmwzgp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2prhfulhn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tpknqoqb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sgkpscru.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2shtnizfq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ednivjii.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xypatqdt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wibrmwvg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hysmxylk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujmqdayr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vidqiycc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2endwyqhp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xvzhohyp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mdjmqzlk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rtrgjiwy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fiplznpu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vsrpqzwp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zkxeetgq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yvdkptzv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tijcsmox.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kdobhoca.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlokrv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfkebust.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2anyurmur.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjwpopqz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2khrdrlxu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vxmtwuqu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vqjwdtkh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qthmdjeh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lftahabq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jogdqpgx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ljiqqgjj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcxwpdfh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hvjtskjh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2odjrfvum.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yvmzvdse.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2agttdptl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dnwargdf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2enmhohql.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eqvaynnv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jbthyzai.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2bxgdalek.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wmhnfqfw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nsjxxutn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cjrrngox.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rcgvidhj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dslobjle.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cildpbrw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wfkipuje.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dguhmhoc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2aizbnyec.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgwlzjal.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gxtmorfu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdkdioms.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pwueimcv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvneyzsi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gpanzjis.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dqwiifup.html


<!-- 参考信息 -->