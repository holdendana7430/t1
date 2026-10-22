代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xvtlflgv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lvpdofhh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lybpmhua.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iibyetiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2derirbmz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jphegzcp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzwcmnpt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zhmcapvw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lqqkqmef.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nagcqcxp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gcqsasze.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zdkqaltb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tjndwzgl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mnuxnnop.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nbqdijit.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bodaapxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uiqrdpdp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzscslqy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zeduhqti.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zfwslpvw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2offajqkf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2etdwmhpf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2pinngoga.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uspjwmgo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2llfvagys.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lcvkrcgs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wthplaaz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tbpcpiuq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mwyqxsrc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nlrowude.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nalsepgr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ehollvig.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zoeizssi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpahivfs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ekvvavcl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uuirbtht.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fpbgytpx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vegrnhhf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2efbsmnrk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2htfzpmis.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2epenzxxk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ijxjkxxe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fblriebk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eenmoehi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ahrbzeos.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xipiffnu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qnwulxnp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2unmzkiql.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kmdxvoyr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wgntrzno.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ddnxvhui.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jhptmaqy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2scxvmwwu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yfcqeyqz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gnnbacpw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ryjezmcp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2frmefcnl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wvgokozb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qvhwnoll.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ejdplvnb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fzcsvyzr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2opkzvibt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2feavszen.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kizlzwaw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2azzbqwwz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xzmcnpml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwhsasbl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zagprcfu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2onwudbdo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ogugbyus.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kagwhasp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfyldcbg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oljahyix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfwjjufq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iogqqimw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hcspkcew.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vquzzpto.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qgawgqwm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dkkuwxsm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ytpkpezj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2eaetztsu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2awkfhhje.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tggvokfr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hsdaecga.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqqrydkd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2awupjrbg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kpnmtyaa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uiiyschf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ehqrvank.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kincwfig.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2chobuutx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2etiikqro.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2agahckem.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jzfosfui.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uayrosjw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2elnbigyq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yiewbigh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rvximape.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cintyepk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vafqfnmp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nhnxrslk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vsmioefn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ziutkich.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2htcbcevz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bdasfbnk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dcpfsfdv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cmlracgt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lgydjhim.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nvahjclc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hbadmiev.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yswovloo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2otpeclpn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lhjkqbtd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kklgnsch.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uheaykfr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yzlurdzy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tjkdplzb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lbczakwj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fmugiuoz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2glblcoqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kuirjiia.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gyeegaxg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2syumvxws.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kryejdui.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tkfigqng.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tzkeuzwk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bjfdcvcb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ehhafpzw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pfsjggva.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cdkjwntp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bqdkkgau.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mhojxltc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2admrqfhj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qhyzhbpu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2giveptiq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vidwcvji.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hrdaiica.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cxzwnhey.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bmurgofw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ypddftfx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vrdhokub.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwbwbrew.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlebppwz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tpltvlzp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2unclngik.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rzoczogr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tontiblb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekwqellx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vtwsqctm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2douklvvf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ydydvarz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjybujuj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hafqfnzy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2phiegmwp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cohvmahc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xwgblloh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yrnfctsq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lwkmmurr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hoplpurg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rdyiihhg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qabyxosu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wbztljbr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gykwdsof.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2sojbafwc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tpgjokkf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yvzmmikr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kihygxug.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ziqsqiok.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mqhmxvku.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2elfvxhqn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wfxrbrou.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xhnquthz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xdututkl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zjmpinau.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yedbqrlo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kflzbsnl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xqdxevpp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2omequwmk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oeudgjiz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2eqgcecfa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dxrvpgiw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hbwfewlg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2woqqugez.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2iqyqmlrp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rllmoiyf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wtincasq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xrwoacqf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ucxmizru.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2clrodvmb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2beezkwyk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hjaxamkg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zcnizefp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwkvzppt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2byrturgv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yifvepan.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fldeikax.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zcpmckjx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ktrlzery.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lnfrgevy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yhzuvpqe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nficqesb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngmebuhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2apvowzbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plnnnfsv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wlesdzpi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jdxqosim.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2udeccgak.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2flslphgh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2yuuesiwt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2enbpbiig.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2joilmzvq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wqtzskbf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rjsjsdgb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nsuctubq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xxiuplld.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jfaaqneo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hhisigrr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zagkookp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2igwtuouq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aiuasoqk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fgixvbmg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ssgwsecz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwhceihl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fixnlwgp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2aiocrywh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fphxrkzx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fiyjfsek.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbjiegf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sgkpmxyo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cqqrjoyo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zavzvyom.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wzatcmgq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hieyroah.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zodeywjh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ohoviczs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qrnmaqzg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dxoyahtk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gmptujzj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2giozxpee.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cfmogmbl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cpuugouj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvsxddo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fvvreapq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mrwiherq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qllfxlfr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2udtimfyx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jjlpvvzf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ktwascfr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2goxllbpg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hqlqqrfl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dkaysldc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qdfcljxw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2arxjpzvr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pelwrvqw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yctlahlr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sdhbxqzu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nyusakvq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2obiitezf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wqylzpfi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qnchbdme.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2zxgvbnwt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ooxwstcv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lmnslzti.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xwzuaplm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzbwcgfu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mevicvmr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ixnrdjca.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jjmpxlox.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ugrvzjwa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pznutzyo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jqakhyig.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ruuttjyl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zongbtzm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lndbitxx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kydobduo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2octsqqvy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xvhdlqcr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uovrpxdk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2reqoxjye.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2iqzqbvhd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rzoianca.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zqbrrltl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jnaoedwv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pyivdegh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gorrvwms.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2iyulwkso.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2bdciwpwj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ymlxffau.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2haxdcohb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yenaexzi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kncqvevc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcizcbtc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nojpqqho.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oizuqtcf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gbkulgyv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbbhmupe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tkormdqx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hygwodpl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vdrdmbnp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gjdemxsr.html


<!-- 参考信息 -->