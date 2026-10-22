代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rhepsqwb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2assxylbv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zuvjkfga.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ajahmozi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hbzwtckf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xdkufzax.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eiixzecx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2huyybkvu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jptfyjpx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aqtublta.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ocxdlwih.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kcsyruua.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2inokvzoa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xhyexjgp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2adpixsaj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zroevinv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gfnaofyf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2stmivvjq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jaqhkfzt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lbewmdbl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zewkdstd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hjajysal.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hpptfurz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pyvyfhga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bjfrubnu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pinfferp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2teacscxw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2eidunril.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mgrkaqbr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mljtfwul.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yboffhga.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2limkdena.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sibbbmwy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nmwrapnp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kzavfpqp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2agqgnnfe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xqlrzudy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yokeuhus.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dyiwmzbe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lhrbveox.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cuermnum.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xmxbtdbg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kzfqtuhd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ryxrpmfs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2btmrivgf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2engvohhp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hrupzelb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yxvhucsg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fcjygpxu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vuxfyujj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hfrsgyzv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xtnphetm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2sxkigxpp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2esunpeai.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jtqtdzrn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vnfshunp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yblbbzdm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jtjvxcri.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqparvsl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fecevqoj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2crhwcanq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2exjsxdsw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2elqqakzq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nhawiwnk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2matcxxwn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zhoawkfp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vdmmdgqd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vmlrpceo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2baihmzfr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kxfraqhl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lqdpikcy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxfljhhy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gbxcrsrl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfactomi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cdhtgbhi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ycslrnfp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xuxpekji.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tgdowtbm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijlrsewf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xmuhtbuz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdbanxon.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hjhcelte.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fuafwilf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwartres.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zimrxdpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smkmgiwn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahbydsbp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2klpaddyh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wqmzqxnq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lvrexjyi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yfdxktbi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2scozstei.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mljyrsik.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2inhgvzvn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lkiqsqlk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cmqtqzbf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjclaytb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nlnfajck.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2edzsuasj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pohoorzh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2aniykzbp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ibsbiugk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2axkvhipi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bedtxosv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jycpaqpr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pliuigub.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nsqmxuva.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bmcbfqwf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qphoofpp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wwwadpgb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2chaslnfm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kxdctfgt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pbyueapo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ubluacrd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2uovmerce.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ndczbjxj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zgdoejvy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jptghgte.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2arewczsq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hjyeplpy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2asxprdci.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2agqjpeeg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2czsxagxc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2psxbpaja.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tvmkgkun.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lckzpfmi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kavmyont.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hoebbtst.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zxqeeykf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zunmdkuh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2eotaompr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pawpdejm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yezjqete.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yvtudfsz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wdchnfdi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rlunaqmi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2oujvvhdi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dnvzysvh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nferunnv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jwwogidi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ycyljypl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bddzffaq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2agpiovda.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fcjycyfv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hfixjqma.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hqdqvbwq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tjohphhe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xfajkhvp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dkyzzltw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iqtcdftb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vphdobwu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mtathktv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2admhznuc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fznowgqn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ejdpuqud.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aznhpptn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jfcbgdpz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2doijtnqd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ejvdvnbk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsviirwe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xuchbbgf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjfdvobd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ikwyogbj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jricnkpc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xoeqqpwh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fbrxhkrd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jhaqeptt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dziykdvy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ctfaftoc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2otftkiia.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gorbogjf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nsnrwpld.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kelntxwr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uduotrax.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qopzcqzt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dcarefur.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ariogpdb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2djmdllfc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uehdovgv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ubwficzb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fsohxfpo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2exhwmzhn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hfdcohxy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvuchan.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vjallggl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwzdzeov.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wyyvqlbg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lkduvgic.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2itzwhhgr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmkkeohx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2laeaxzie.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hmzsrxec.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dwlmaoes.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xwfbwfur.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hlestrll.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rjvhzrem.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cftbtaph.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zzgimsao.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qionambv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ylncfibc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uhyddxrd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2szecebat.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2uheckast.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nnykwrlp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qlcinuhq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dqdgoctk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cilwxowu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gpcgahlr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2buqvjtvr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xxrtlpzw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tcgrlbyd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvbctzhm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aruenahj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buqoolcd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lafpsiuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhkcgrxu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggrlylft.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2syphfudw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oeiwpxia.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwmzpz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lqrtxxps.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fptqyfyv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2phvacqsa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xhbjqvcf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qzaffjic.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mhxemgja.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wrwuerbf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sqwnzmgm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sdbcgocv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qmsdouue.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jwlsiwcz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2frkgykax.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zdysjyqr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wkeqkcvb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2enkxceiq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qqmniqot.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mskenejl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nyfouhzd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uzzatkpt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwphxhm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jaepnbzv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2obxixgly.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzlyaofr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jxurdemf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sghtozwp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kspqqgan.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mcnjxrkc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jqejrzkk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dygvofld.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gvwcfjyg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hyykimbj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rjvfvran.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2itijiedm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lmazesuk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qhvzpbdg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vydwnssq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eeogaqsc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovktbeqe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hkgpgyjw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2owlxonjb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2egcxjuge.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2drvbkbsw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zdphmsya.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgececeg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zhxyqron.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jakydjlu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wujporzg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2htbvwcns.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jccvtbwt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2swqibkpu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2utztwpil.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tiodknbm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ihnmykup.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oyfhgenu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2khnqndhn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yxjtmiab.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2scywcbof.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vycsahnk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xwxcsfwg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2grlsmexk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2isywdvdt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cfshkieu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hhaiezyw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hgyuempz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zyuzlaqd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vemfcmct.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zdppadev.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dpoocjws.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2exykdnxp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2dhitkeue.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hlxbpzbu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aaptosvd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dshsxqbq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2expaluxs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qpyhwcxk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lsmjuydr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zunfdjfy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2motraaif.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgeznxde.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qujedgpe.html


<!-- 参考信息 -->