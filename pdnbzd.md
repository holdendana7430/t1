代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sklqqsed.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mtcbrmxv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dabqmgtk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2garnpynr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ehnavpab.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gsfgpqhx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nsruqrkn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fpeqabut.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ywqowjnn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bliwzlip.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qlpdupik.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ymkojsvb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rsfhtisy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xatrzvew.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2myzdfdwx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gxymtyak.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2eqwpmwpo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jrvxudam.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jqhhfadx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2aygrrscm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fogbtrzl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2acppxrgv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2obilcusx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sisobusc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2egmloxlo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbihvdgh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dxnteiee.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkozdi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yvuofsbt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ziaajajf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2weozlisp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2trbzebua.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qmqubpvk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yimonqgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eermkprm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vsficxbw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pgdslijg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oiyljlwe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lncdotgc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2filtasbm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bywmovhx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufjmjyeo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wkskbktf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mzuzrgra.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ohzdvqkl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mpozjrnm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rfmisggw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qpttrnyn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xleeskxn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ntvpzunb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xcsgomkc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wzrlncex.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fdlnzquc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jpzheztb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khzjtjsc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nmnsxxng.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kunoxzhf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2klnlkqoq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yhlwixmc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qxnazeyz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nkcafroz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xznlmdxy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qnwxvcdb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hwncwmdc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zclpwbhu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hgilbgdh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uunztmaf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vrmnumxl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jzwxwyev.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hitmyloa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cqhwwmkd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2llweweih.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xtchwsys.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2beqgqksn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jfyqrvvh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gurqhagt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sipvnana.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qxgagnae.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wfmtqppn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbouansm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ismlqlbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggnzdpbp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2knvzibjm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dpioboup.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcdjwop.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pawugmdo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2naptnbca.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dypkoaqe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rptiekdp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2uryplqih.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yktabypf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pbqcemxw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lznvzbpw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tgtvtnye.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ustuzhtl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qlceybzw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jpivbxeu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ueodrcmb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wrtqmfnn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dpmhxrfo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fbbzyykw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2slqususg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xgfsqhpx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zefspetc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hlttugxk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mnfbcqdp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ntjdlltj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lztbyedj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vcrtezkn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kjqawmrz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cdtqhcty.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2idogxkit.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dhelompf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cvkwpwdh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fltvlrhu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gzipurhl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sendqfbl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dhycueds.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hhuhjeis.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vrtdklmh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cdcerwey.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2snldlrue.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wcjsdybl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fghbidxb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gisjfpfd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jibmwltw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2utceywuu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qrsgvbie.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2btpfncrl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2erdobmmi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2llgxdktj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rhpicqja.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ovueajky.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wcxyeupf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2buzrwbtl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2caymtbus.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ikqpvhsr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2muxadkqr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zoutqvtc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxhkoovg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ghclznyo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lbjkgoih.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zeynrcov.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2todjwcca.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vjnsinpy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2plhtjbbr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lkwzaqzn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pktgqrqi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aeapusbw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bfudzqbd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhqfoqzf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2yoljaymn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2paafiekr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mmqdlyro.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mehvgnao.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcrkxtno.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2onhugtxu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kvidwxip.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dbuukvqv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nsiypjmj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fjsnlghp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zyfohzia.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wlncijpm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2atmzcizs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jjbczzzy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2etrvhsyx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vevbtrgb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iblcdltx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dhzqghky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ltawxamy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mdgmiafa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fddqgots.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ksktfmfd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ngcebkyz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rxdatqma.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkytkdbt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tmkjjhdg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rmqivumw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dgoexuak.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2npcefdxv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2yajqjatr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sdutefdp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lfpfsequ.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sixoursd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dqoehkdm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2llyrxupg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fgwboayv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nluayhkd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cipdeosh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ewqosqcx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2znxwwjyn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ozttimmw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzvbbct.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jyhgjlqe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xwskxbpw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gkuodixb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ozrvcyxi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cwtvbyik.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jjhwydfk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gbinylmj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2otdiavrv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bryeunvq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vihiioiy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pbyjhjep.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oshiaagb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nykkfpxs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2erotwwaj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ywlillsc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vwssqhhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvktdzex.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iilixalv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2malcbzfs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2heizvmnw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wbnggocm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hxajqgfh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qkfkhqso.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zobjtsso.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2onxvtdor.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mpdjvpvp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lecjvkik.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cpduhiyu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mcqoaijt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zqggxwzt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vsloivqn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2auyjdbmg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fcxotjdr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vfipxniu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2grjpnukz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzpaomnt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gegubexe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hmsctulc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yyikbiju.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uonudlhu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nbkuqhqk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tnskzdzl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cumhtsav.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2khdidpct.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vhfhjnpx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dxfikrei.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ghfgycev.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qsjzurfk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mnqnxpom.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hlbsibhd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rubiquag.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ccljgybl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zmfoyjzc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ljosdqbk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2izotvtif.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fxbjaiit.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fmmhczxs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tglqzwzp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hlkhjtut.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bahixqsj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ubpaeqxz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dgweydrf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nmgftntr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmcafcjp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rbpjaier.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ptoxtiyz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qgoqasht.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lvemrmcs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2udaohdqh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wiqflvgu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kwinrrex.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wlyfoasz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tlhafcay.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pehjfklq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rgezkosl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fvskacia.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bfmdgcua.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2twtoedcx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zmlysgje.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rziryiqi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2faqouhal.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nfcevswt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lupxajnf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ndortoxq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2txktmoeh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vdzauufl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2eixxjxoy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kveuqvnf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ijqvlnls.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnqxufnt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zvigufjb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xbkgiwxx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xsotnyzr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qtnhjsvy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2itxpcvrt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zmfrostq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lnalkjml.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cqkufaip.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qvqxfeqv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgloxbme.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wrgssziv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2htorboqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ptwklidv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mcrtdigz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2iqfyqwtv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2opgfqqnf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xxhsjihc.html


<!-- 参考信息 -->