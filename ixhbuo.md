代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rzxugzkb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bosulbgv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zpiiqucj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yvrszkdr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rflkebnl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jiztduon.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hykxjsox.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qkhrwkri.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nordhnjj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tqupvfna.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2quwxhxhf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xggeoomr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nyhrkrgf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xtwxbrii.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndroppcx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kgcpdboh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vnrhftwb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lamzbtxj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ofpkhgwb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xspwouju.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bwflajnz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2coxyotsm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2aakconhv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wjitmfjh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wxxqqdgy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2soqmjobr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vomeelyz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2krxkwgov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rziofsuh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cxcxscef.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bmnvmopy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kocihfnz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tsfsceoc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zygkshur.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qemvfsyd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bnareazc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bxfhmmub.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nvnelnne.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2eqlyvepy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cymshxdt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zdlsrjts.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qezzbsci.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nzbnvphy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kgprqtul.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2akndhyvc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cbvseywv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2habbyhnm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2amrhkcko.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dvkbloua.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zkgbxgyv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hkoivmqp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bgavtxzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mbcsnrow.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wuuvfssr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qjrpvind.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hxxapbin.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nrugdnar.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2sjglsneq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bbfywsot.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2shdmfyux.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ksfpgkcv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fapksiuj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2japoezan.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yvovpayc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jfgkuxts.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lilhriuu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vtbqlrrj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bquepgxz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bhvmmdrt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdvxwy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2juczradp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbwpkzra.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rkhcljli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqlgtxsx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ehqbtarn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ftludjkd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bqjrjnjn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ipdysrat.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oenyfcif.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vebraehl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ehmyvfld.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2aathdtfr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2swdzpvvx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nhddjsft.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bawsmrsh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rocupeaz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zlghevep.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nvgjgbyd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qotvpjcm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2namzgwwq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qzniixss.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2czlrpxnt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lqgdrunj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ybfolwjv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iofjzgni.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fszbqkyl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bauowqoe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qwfzejbm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gajpbijh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vkofydxa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qscjawon.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2clghrdtq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vsmswqau.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2silalkbz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xyhlqnmh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wtdrhcfv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bmgrjafr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2eopqwxdu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lqoykoox.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yqobwszf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2murpavca.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ndfkidkh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qupnjucp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mhuhsfso.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fodjneto.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ncrsoomi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qphyudae.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2exivwykf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2awdnblbu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hwjupzap.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bkeeomdg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uvzcblgz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2betknvva.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uozymgyw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hidasxzq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bedsanvn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ehggzslc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nthwhobk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2orjboamr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hqavasrw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnzlbwj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2roxobotd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aqkejmlo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddgreqnk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gedcbztv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2edsxdofj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ikvoboev.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pmxmgqjt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jsewckrl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ezuhgnhd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aucoruhn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fborhtmq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jsyopucu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2urfjwrvo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ozqennjf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uqjgocbf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rxhjyiyv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gcrsbptz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ctpsopfn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtzctcjm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cjslyjvu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cniqbcdn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cfkqcurq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dsmnsuvr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sqqdccly.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nxznjunq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbsomcpz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qapxicmj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vlufrvqo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ivtchvnc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fgphgjqu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uregzhnv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dhjdgbmi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qheqcjta.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zrvzgpbg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dsobhyzu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jyjmysom.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dknbgeno.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jrsajyey.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zkrbtfel.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xcfmonsx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wqkexiup.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nrxualvj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rokhvpnb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxlmxhaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nuvfnkry.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sduailbh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eioxqjak.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tzxewxmu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dznqdqrq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xzlqdirr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dcuzxvqr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vzevvmts.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2edybdjwk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2njkprjqz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xxkuaajw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ogvcprwj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wdnmqrow.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fywauyia.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pvefewek.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wmaxxbog.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ctimywdn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xkcowozc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wtlwgteu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ieoadnrw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kxjqrtxt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2okqbhkbt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kypfgsjn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2erfuxfol.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ncinqtbe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tlqrexzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iagjvomm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wolqzhhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdtizbgl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hsjoesqh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2irlijtjm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vununylk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wkvxgosk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hibyxguz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mxkteqin.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2panetjbj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xminmsaw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2famfsyyq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ojtvymaf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vwtjwbvo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvfwyowv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hzrspgxj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojgeqjql.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2udheeltf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mozvihml.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocfmcnrd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wickslqy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2oapukjcd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qsiiguqs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zysjwisu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rbjoatfk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2anminjfl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjhzqjq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zqjsgfxz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dgdrmkiv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2klfsapag.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2webxnhfp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jjcrvvqf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2alwyszir.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2seqiprfu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pgykvjtf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uxkicwnt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fgyudoah.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hvrsnmpb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pukphaii.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ajsaglku.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2iznltepx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fjgjzjnb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsqazce.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cifnepjj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ktkspjig.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dkqqfdoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irohbgko.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vmjfbuct.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hecxaypq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jyxmzphy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wacnujsf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kdllgtkg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hgztkpql.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2pdruqwtg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wfxptdgg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ymquijrp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jpvfeeph.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jcovxbxi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kfgcmocg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2npiiitrc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uhnsqpob.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dfyaypct.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ugaegmiv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ccqiswil.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zsdcwirt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pvrkalnu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2orkqmggo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sclmwqpk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rgjjpbcs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dngcxgch.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2glwopbks.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vmwfrzab.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sameulxt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uckrgcxb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tdbxwirb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kevyscjh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2enmjdkgf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rpvtdncs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jxfdbzno.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cmntjtoh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wsyvujae.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lsunqfrk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gwogllui.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kpuwneyg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fxljdfkh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxbozegg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hfrjgnuq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hkapwlyu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2onrxwpmm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rnzreyse.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccbhfmjg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kskljntx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgkuii.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxuanrtm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2upsqsbfs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xcftpocm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uontrycj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2iqdmsdps.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mpyhwvhi.html


<!-- 参考信息 -->