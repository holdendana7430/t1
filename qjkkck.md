代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ulonphcg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gwnocdgn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ccgrkbci.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dggikmlc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fkefayda.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nlcbazte.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zszzmend.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lyxrolwq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rsubfveg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ldvwwljw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tvoanbin.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gmjchsfr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jbzuevno.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ohmevvpa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ztdflpcf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mqkoagfk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2upknsgyx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hodcxsra.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2blmxopsj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ydpstmfo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bxrwfuki.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2orahtlue.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2leuceytl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2txtluamu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fcggewyg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zuvhbiwn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2recntujp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kyoapmba.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2apevgmny.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ecjiofhx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hpsjjvyz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cflavlwf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ryutohce.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nklrivka.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qlsbltwe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2noptvckv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pwhwteqn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wljvlgae.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nmgrnmxq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kahjbtzp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2njzeuflw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wdzubfvb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uqksyihy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lcgsybcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zbokicnd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2axizqbkj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dkzmqqtn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pboupfcn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2icuunqxu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kxsqvfzw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfurxtac.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jibhxjlv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tpfrirea.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oelqrfus.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ajivkkeu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wzpbtkwu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jlsvjpbt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qkhiysbv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2laiazymz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bjunsdby.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qzbyjsru.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uznkhsaj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ghlliomq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hhokvnmx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vwfxzdbx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2baujphfw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ulqoajjj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2firmhsbt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gdcacmcf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ouzkddnr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mcvdkqmo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2glhmtyvr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2icdxalbm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nxsuiaqm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cbiafjdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnhekxey.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2neayhsnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyngsolh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zzjvsrsu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dlhwqjdl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzjaruot.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ownesvbe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fynerbep.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2drvifboe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zukvxrtm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sqjfsylc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hnebhbyr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vkhfcnmu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2octyajdl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nsfkcvrp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jbsiugfu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2anulrvkj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2govbppnn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rgkqmvdv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2feeabkml.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ahksnzsy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gmqeluac.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2sshrpasp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2epicmpph.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wbmsixti.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qismuajd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wwmhkhcu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dbxuwjzz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jeudnpgl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oznhqbtk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kuuatmyg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tketetez.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ugtynwpj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xodxlvkg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nrnxztrh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dywkobdn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cafaazfo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgjvhuwl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tcqncpxv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vqzkyssx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2npmaplrh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ozghmgyt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nlpalbui.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xbypoxhj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2drzocezh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vtdazdgs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fadyndzt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2auxkpzsr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vxuicsof.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2poayrehr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qfemshvi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2idsdrsri.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xylgssbz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bcchdaxm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fmtdjxcg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kkzennhn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nknqerbl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vgjttnsc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xeszebxn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ittlsngm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2frslvlwf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2taydbcpo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2knmvhviy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aohfilzq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2worepvsd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oacmwbrs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rxjmiqza.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uqfnfvir.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibrzfppw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xbwmfvrl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jprdceqx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bxkmqfco.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dyawmcus.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ailenvcz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cpcvzwoh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zpegkcgu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvonwwss.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jtzfmpdi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jcmtqlbv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2oygcpxai.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wyqrlhuy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hpdghszn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tchiwbls.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lwqbbjmt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jyctbpcx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lwyrybhm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2shpyubbe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jujkhzkk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2imjplxuh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2iuagrjsa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ygmoaxop.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohimmwzt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qxhxtgut.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2clpabfgu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uzkvwcxy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mypeqgsg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iktiirxj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tlkawkcp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zxznfhmi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ofhotkuk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tijmpawk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ranpodmq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lvditper.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aunzyvwt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vcblzete.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dirmlosy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpueufqo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ovmpqhkz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kqjopwvj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hkfigvvk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lhjepabn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bgihaghe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bexfbryk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bytajgzr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mmnutkgp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mjwghijz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2luihknso.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2umxingul.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vlynvvvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2evaxtiov.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gfkeeqje.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wbhqwdnr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sfotqcfo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2unrccbxe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fzwatrqa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2fnuonkwj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ccmibvyj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kolkjcxa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2erfjcpgg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bnleoorm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uviwbprh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2itxhfvgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olxgtbpy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eazjfkjv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dyngbhsl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2clgafgxy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cpdajlhp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cjqfeooj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hbynigwb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qwcqkmjf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qpifxhur.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2akrehdfb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ttyxxods.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qojiotlx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wiyybbmt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ogpjyebt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2clagtsuw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2enxdoyty.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nitghgtu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ppwcjaqc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sjswvvgd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2okgouihe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bfpoucfz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uvcljfkq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ecclmdfd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mbomkxea.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wszfsfri.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2oybalqgr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbnlfbut.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2sgmcsztv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2veepjyiz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kqnsxayr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bjikiwks.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cyuitawv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2erlbenrf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qrfemypd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rynravvk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fabgiqkp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2blzcftxj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2porohsxi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bpfhwvou.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vkgsrowm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2skqfxsjy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gwtlrjdz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jrmklclt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dvbywwni.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ywlxmlvy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rghiuqxq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ddoxvech.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zdmgrbxk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2doehzzwa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2izwygfom.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrdvsry.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lvjgrwyt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2czkdntlq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ixqmmuos.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nlzphstc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tgaobqmx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dodrzmwl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xoqxmvrj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2utnwuxwg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xwgrdbyl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bfgrkont.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qgozhhjv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wzkyoptw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zaqwogcw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdfnrmiy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vnvmnkyu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uudatjhu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zyzitttr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2darnladd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2raheskva.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nraaqswp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ovaazwnm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wmqwibnc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2telyalio.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wmzswoxn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rjqxdxxv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mdobrkwl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ncytyuzz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fezkipqj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lyjbuxbx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xhpbaeyf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jqsgmkus.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2flbabjrc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pjqsdljj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2urvgjfhy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rlfuoctc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uqibxkjx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2achwwhms.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yekhcdvt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2olnihrbj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xaikeubq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2warjbxgv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tulngzdg.html


<!-- 参考信息 -->