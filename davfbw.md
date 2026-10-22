代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vdcmfngf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zpfsuvbm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hbzqtqgq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hrtcdkjs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mllzxthw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rcgnmmuz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yneupxru.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ooutsvgf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2guspyzmh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nbfdknla.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfjftdib.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2awdjynoh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2whdephke.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ovhzarvz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ciklfvtf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mutzdfaa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lnfodmtc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2slyadeaw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gyxgxapi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rquxwdcj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gtvijrog.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tlbsupno.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ttmwivre.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qmlgjeja.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ulxtykjh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2duzuyaiq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wlwtosyv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2twgcidth.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2yaykwztb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2woqtgpct.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cdoqyzyx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xojvwtpw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lvnnfcdf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfqhfyzc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zmvrurof.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2izbgaukn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ilozreie.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bfoetmjm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mlerhavw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mnmfkaxp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2avyralqw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ckkxonek.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kxbhvysk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zfpmomud.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qcbfdkvq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ckrcizev.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zlemrggf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wsxsyesz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2perkgdbk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tfhcwjlh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2utjstwpa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2unhgsefs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kdjizshp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ztfubrwg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2unslfihb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ypidxjzz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nbxatdch.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gnueqeuj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jepwdiki.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cfadmwio.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ggtqsiaw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktnaaetz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ihkbwpjv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iqktrucv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2krebccnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2owyunhci.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2acvzpcty.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2alemyeeg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ifdmiccf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2szmrfjzm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xjhmjzdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfefazvf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aiwpzxkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynzcexjy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gxewyhdm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2utxmzceo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebctuxbm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bxeatfba.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xjutjmux.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2olrrhrgs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vzlhiuck.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mhxgkklg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2skebrcxa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fuooeysh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omijoesk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yeeenbjl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2srxrtyvs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qtiymrzi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ntnzdenm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fquixtlr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2onyuknlp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zombojop.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gdsztrrt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2cmlkvrmr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jkmfcexs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rzlpuyiu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nhwnkstt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpiwgyi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ftbptcjv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqulwhry.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ppcjvnci.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ibgbqrad.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nskejsod.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2csogmxbs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wvfhxcbk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2siqumojh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hyhoenqs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2okkyljbn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcvdhcct.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ftzlitir.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ycafmwyu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gyfnsabe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xnozmfxv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ddtwoejv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fhubsflf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gkzwrclz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2quupadio.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wysjxjbm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rnwbzwpq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ojkjwaeo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kkeognfx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xafvagbl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ozlgpiyy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vjstdbhz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2czuotrgg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bvtvflmk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tajylewi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cqjybmit.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dwsatpub.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bwsuzjio.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ohiuoggo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ogbqhnzr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vkmaevfi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hxtsnvet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bwmnwrdd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2knaujrrk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xlmerdeb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pfmamfme.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rxdzykov.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pchkwhys.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2phnwmgdx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hihjywgo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vbrahsuy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dtxmvuih.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hufrewge.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2acnyjugu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tmzgdhal.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2whlctimf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bolrpfdl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fmmltjyx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bwquouaz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bogaubcg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yvcuxtjg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqvzzcyi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjnkmogx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2odufiwgs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dmbcquac.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mkvvpwyd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2imwgsgzp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ciapphmf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ofgzljwu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tvmhbgwz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ffmrvusp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2guhaoxgg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bcmsznqa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2futlagde.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ylyqmcln.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yleqwibi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nwawlvac.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2aocjidll.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kmbiyhad.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbuuesda.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cbzcoaku.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqfspxt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxkfodvs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bylzzbzg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uijyecbx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ikczkrgf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xweegjac.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qydukoyu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ydvymibg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2udobzjyo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vfirkzva.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2keuouxro.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmgpmshu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ytgtwebz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jnjwhhot.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vuxoicyi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ffwhwwpv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jueppfqh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yergcpcd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2athupjgl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogzxpnco.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hyxyynzd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nxrfiwgn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dmshrbuk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rkmcfzcv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2topytnye.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2iggezcuv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2happwumo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mybpavmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmxbfokq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2synxafsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gozvavjs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ehsnyhyx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tjrxejvt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zsoyxmnf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2eqgutuzv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mkpagony.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ydioorxu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2diljgxzw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2inyojyvx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zayxwxnn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rlskeoho.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dtkpxyta.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xeptgmif.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qyskoxih.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmkkvynj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bdfytfec.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwjdybi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zcogbkue.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2csvfpiys.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ypheeycj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2eelumeqz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lhnfknxu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hajnssjf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2abblzoey.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ortlxyrh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pxvoqgyd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvvhndo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wfwdszzv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sndgzafo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rallyorf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zbaofhkt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qeuagaax.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tddkyjap.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gzapolfu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gvvadsrm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vawoxcvv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2shjtrgfb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2evliotgm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2odlynxqb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oexuqmup.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vsbqlqib.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fuwjzxgd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zvamlkdw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wssxedpf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yoksuxju.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2khexfelf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2utlavpmy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2miiyxika.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yeuwbaaa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hmgwmnfw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mfhrwsxq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wbawkzhd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bewbjpic.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cndcbkwn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vaorvyog.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qygprixv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2oslveemc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aolqfbfx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vhjqfhwj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wqzwtizi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ypblyocm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bhzoqjie.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kcwrkttr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fjpxamle.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2liorsywg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ztfwoxea.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kdonycwf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vbrssnag.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ajouwbjl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zvijtzjn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jqmwtaqd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmnaxpde.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2upjxdqdi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uyimkzbz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qqdxpyyj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2yosomsgv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yoiskyfj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hebdwmcq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mhhamxnt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wzbbcvmn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jqoipogh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udcfbnrv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dvzesybv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2glcqykry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2znmqmlig.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ljopsrjd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ilwkflgt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kuznzvoz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awloslep.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lrnffwjc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnjpgcge.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wiafunkk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2unboyuxk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zbteihmy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ekunhefr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vyghekta.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fvlhmxgx.html


<!-- 参考信息 -->