代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qxrogbcx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3khvuzsmk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tuhustkm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fsdrbzri.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3crjuyngg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mqolwjpa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kpsqxrsb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yggmafjp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vjmputol.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xtqqkwwh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xslcjnpq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gaogdxby.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pxkbghuj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bhaelpdq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rgxuizhl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kenrcihj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3muaacsax.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdfucrfk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kbsgnoqv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gqxvxczy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3klkytdbf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mfskazhz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pvmsyiuf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wndhfmrm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fltsikjl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dadflbfe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fyamztuo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dhrtyeel.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3otsyzziq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ppdzhjoc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wmlfnqdf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qepnlfqp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dilodggw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xfbvywfy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qrfuhxoa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rqzgsxbg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3okqjumtp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ncgypmwv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhplukg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ithwprlb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lwsrhydd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xxzlruqk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dtuoqdts.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hbidstvg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3idhohpme.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lgnjapdk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tknidxjj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jphjmlgu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rwkmdstn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3sskhgbyy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3opunazbh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3olrndohd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vmdpnjjn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cmlvilqh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ioxcvmyz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xysxjugz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3msofrobo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ecvspbin.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yiwwzacc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rlqrdpum.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3biragqlt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dreisdjv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hudgfcor.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ophkyhxc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ibjajedo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wexafsyv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pethijxy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rraicmcs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jukejdyp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qzoqfegb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uuvowmfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enplrkgm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tyevwrfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhikjttw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nzxzqtrk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3giilslmw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3shsiuonv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3javdpzuk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lcaeprec.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ndqvvtia.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zpndweyk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3glmrvvep.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hmjndpyi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ewgxaqbz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imbbumxb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hdfydphd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3urlqxyxp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zbzwlxge.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rapgsyhl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fgierrti.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tpjjugwa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bpjbptuc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hxpciryn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yxheehxc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eyarnmxj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3anyszmyt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ljjxkskk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wighmzwq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sjjvhkvp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkpcigzx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3omqmgxvy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3blueigpd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3noeoxrmo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aqnzktcy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3degkzvij.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pfvwoeuv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jdszxcfg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nlnfebcc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jjlhzubz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3onurjisy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uzlsrsex.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrwjpioj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcnjmjv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ublohdfp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hpzdtbkh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gxdluhhg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ragvajrn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uggrqwqw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ahadooql.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qjksqziz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3krkwnqmx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ahyzbvmh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hbitnwku.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ebveevqu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vpblxfjx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qtcrvfjd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vrthbhhu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ihnnptmd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3aqhyfoxn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qxmcwvsx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwdfzyv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xixbqqal.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3addzfqxw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ogoashoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hpnfplsu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vuvizahk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vhcbcoes.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vegcaqlq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ocznflle.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fqxqnbhk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ddohbkeo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rcqxnayf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtxvjmeg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mslunqfg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tyihruys.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mroxzxuv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3whvcyalv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3snciycij.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cdxyveid.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3avktraxp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ttqthsni.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gneajrzl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3briluiwp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rlzddtkt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3thmdhysn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3keyoihql.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sfmldqdc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vvgucbho.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3awglxxtg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3khbxvowd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjxebbhz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mrquokge.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3frcbmoic.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nccgufhz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fvseityo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rhsuydlq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3efcyatbi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmonnsvr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fcrfsacv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bwwuhdyu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3acdrgwbv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yuhsiybu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3reyqydvo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wzgdqgll.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trfvfofr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ujajjajr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oxnfgpaw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbuoxwwk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qdqpvvax.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3thwgwtpd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mumfvnga.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yqvhivsa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qhhsxutn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cgxviocd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nrhdderc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wjdwyonb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tydsvaul.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pvlnpvfn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vgvojwyg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tivtdpup.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wfpsqghh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vguaflvv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wubbwkee.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3onometnf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vrdmyjkj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lbgriztt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hzxgdihc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mjizvlpr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jvwayuqe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gdikknbz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nqtggrcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stjspcix.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gpimlvsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fteklimw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fjsdjyca.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zwxfmhxu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3abhiales.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tbmlvrvv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mmxqlnow.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wfpghryz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gmgfliec.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rejitbno.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hrdhwcfq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kcwhxluq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vneztjyk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkngnan.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dqbsmhdq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xingmmtq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xhayaobg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3thubfqqb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmsowwpd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yifmucjx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwhhfzpf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qxxsuuqq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3limznxjv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3czykurmj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uzxcqhja.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3musvrbbz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hkkjctzo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ceguymsn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3yqytdbdz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jyiofskq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3duujzvzz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pzgvghur.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iazipjrl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tpedmckh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xosqgmor.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xkpkickq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hyfmrvcj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ewkqxsrz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3orarxsjt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtgvzugi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mellnsnz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bbamnkti.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mzypbjxf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3kesrildv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qjpyznqv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kuhaxjtc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3limvvalz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zzirlwlt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3taxqrjqk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iqtrfrno.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vrgijvtq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3unxgprgf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hbnvtxhc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmeqweb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rgzmeowc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bxtjphfk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3txanamfz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hwfuzqrj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3embeyjzt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3puaruzcx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3smkbudtf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3npwjoaru.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrgusujg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kipfwicq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlxneihb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wufuvqbl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3scglsang.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uusqlyey.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3brulxdmm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pjwuxmvw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tckskxlj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hkrcxotn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcisiwyl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dalfqrwg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eeqlrogg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tlbywngl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lgnkhmrn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3chlrcvuv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3crsfjhlw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lawfwxdk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fahdagjw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vkblpyud.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3osfirmcx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ootbudyy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3advhgbyw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhtbmjwp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qyldfbpu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yjvtqvks.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ycqgyiyy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezuazhco.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lbyktmpu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mhyrbnpn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jonqzsrr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3veaebmxz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3txvpvnfi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dzfdvfzq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ccbyridl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ghtwcicd.html


<!-- 参考信息 -->