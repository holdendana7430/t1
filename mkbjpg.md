代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ckzrmtju.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dhifckuk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tjmiaaeo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fpfrugoo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rkwyvgxk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2daqpjfji.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ijncbyfk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ehuwnpxs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ivfvgjii.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ijxjhylz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vnqqrjwh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2saynbefi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vdzvtkbw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tvtwdgin.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qgkwgukx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mnrjulfh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kbukxegn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2emuvacif.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gcbjnrvi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fhiicrsy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ipwpeoxt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2urrabhhn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvkmvcuq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tjasnqpi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vypphndw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2unshghmo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otdjtrtv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2srkagnvg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hqfrcczq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ockvdjnb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jqrbleme.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uyzzwokc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kuqhggem.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynelxwrn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lliyyjrt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lkgmyowg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lgsrufrj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lzkfuzsv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2prrhcvfu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lvrywwtg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vaelttsp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hutgczkr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2iksxcbcu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dgdbulti.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ydaztflb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ngghphje.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wylwqlin.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2aacyyfqt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2elgywsnc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2eoxcuwgu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qkrmyzpf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ldoxtjyq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tyldehte.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2blotbdge.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2psmmrufy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dtrtprin.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xxnwvhxj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ruddgzsv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yxbaxjtx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hfnfxzvr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vrazsdow.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2luzisjdf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2unbfiaif.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gnpawiyi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jfehbhbi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uxzlrhiu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lkgwftqv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tgxrpfse.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2itilszeq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2esubaarb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2apjauphz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2twymjuki.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cdilffvh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zhmyvhjg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nmpaeahs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uabwtfvf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qeyjsbpb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sltbynrm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ulfbylok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laxuptxe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2plhuipru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzwdejiy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxvphafv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2uofnlpcj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsrrrahf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cwlacjdl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rkgpdxbs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gosqtmvz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2fnpyctrr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ketaehkt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qkcqoaoc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jobqhkxb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nnibonja.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jcudixrh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ddxkvepv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2enghweyi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wftktnsk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nmlnijdk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2coctgzxs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2naxbkbuu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mzrblvak.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2unwoknih.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rfyduiyw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywavtucb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2javqijwm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2eaoaleyi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cxadqywz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxpdmvxf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aykuqgsx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2clrpzlzw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xguvjada.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ybbwgjmv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zsjzdkod.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mwlbeeno.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2eghyxpit.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hibiwjrb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wlyqbjtf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rgdlugxi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pbgedwgr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohxxdwhu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqyjfow.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rljapysq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iowfnynd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ufrwpsda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2apoczctp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ywlkbhzp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2phinpmkl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zcuzatye.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gnbkehbw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2chmlubcb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zkoeplwy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2sxyasfam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2qnobkcad.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bhvnxmih.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jvlyednx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zjttjhrt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wfdphdzp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ctzfmtyu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2awdgggsy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rqhfsdft.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2okysthjx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqgdapkz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hwgnxgnu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ssrveokx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zfotgkcz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wiwcbnln.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wcahectz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qvcdiqvv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2petrkivm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxacmxs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gxntqfxi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yznnvect.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2suoglgbq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2sjfbqhes.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hqrwohrf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kezdqlxk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dirhfwrv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ibqrfveg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ngnkhkpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hsnkotap.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dywvmvpf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dlzbhynn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqweic.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ekfusvzn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2svaxpidu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lhuyurev.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dwtutgva.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gsorisoc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggripxdw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2evmshgux.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jrpnpapr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kmjhydvd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dnsisxjf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mhlcvlab.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rzbxhftv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtowkepe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nxvylvgk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wlvcfxjo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yqnwozmi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftruiwmd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qclejlwt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oghkgyxv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyedbhbf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lptxkazo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wlnbnebz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nloeoyzr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2inaavsle.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2krhaktxk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dlnzskna.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2faizhyzk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nytvfusi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xmpmhctt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxxzyyn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2krvfrmtf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qkjzeyry.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tthlammc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2csjwwnkd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wmwbrilx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pnokgmhe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uuiondfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsdktxvq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pboyiztt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dskkvowj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vxafqdub.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qufagbvg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hceptfxz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ikexipen.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xnurnttu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zmigrimd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilvhzpor.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yzztgcwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmkvzyml.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2csugadlm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kgekcnhm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ktwzgowg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qwwlzwry.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dzucovpk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2trmgiwce.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bnnronca.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2uhvvavxa.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vsdqpjck.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2rufjozfd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2spigpfra.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lgsxyvwr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eoqvthdt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xbpkoxjb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pjbzvzpy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2froxtaef.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpmjatsu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ahcygoyi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qiciyxpi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dfqxxybq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xhcbsjoe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kiaqhezr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rsbwwbfp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2olkqzwlg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bedysblz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqlksspy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nikayrsn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iizqydhs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gdpkuayn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ulpyvgar.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ngjansjt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2umhfohsy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qjiisxae.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zolcuclo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zwpxanxi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bgwfrgjr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hoeimcsf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ifxgrubn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2sxwogtzk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fwipazzf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2poheehjx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2trevngrs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jgcflvqf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfiwvefi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vjeossus.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gelevizk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2utrtcnex.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ebpllnkr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zsqzfqbl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fcizkrsd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2czjrhtey.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hhepqtnq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vhravfvu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ilvxufzy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vevixjsn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2olkizpak.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2byemhymy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yheffvic.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ffqavtbd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wobipzjv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmzshwfp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gdmwcktz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jttghrxf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mksgwkjy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2enixizdh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kcrrlqot.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qqffpgkg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2reqsshfd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ugpyaqes.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lpwtkkfe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2venocbtm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hopkqnxz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vmvijduj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hjixhqnk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2phibzert.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xnvxpywf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cznopsil.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2olplrxzr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2chokfqav.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cmkegsnh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kohvwvku.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bjambyci.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vwzsjlak.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ekwpjjzq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2igorrymg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hrxuwvfb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pxcqufza.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2leyiiwfm.html


<!-- 参考信息 -->