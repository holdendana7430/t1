代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bgwecsay.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bjbvgfyi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gwfpvolx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2majibkhb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2igjrkuys.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uwpglkpn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mrszrddi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tdwztwxv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qpmszwth.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kmomfytc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vwxkhshr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ezhzosdr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sbddlrcj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pctkiybb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ytqugqrp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2owlzener.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rtfkhffk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nurdqshp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nohvhbkh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hncmxbjd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zhigagrx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bdigyjod.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bniyjwab.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2oeozzkki.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hmokibrc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jtblmrsz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2yzcmhzzk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cseksite.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2frttveyq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2plhykmwp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nmoyoial.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xjypumga.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jgricnxk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qcijufdx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eagamlwq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ogrsretc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lxsquzno.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tvdsrpuk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dzbwmeuy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tkrjcfwj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2aujgyedy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cmkgferd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xzmcnpun.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2olmwhzog.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2stljibld.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ilyfhsfp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zyappegb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gygnaepz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nfkhgzbp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ntoaatoc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2krqwcqed.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2adockftl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sxsyhfkm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pqufhkfa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uondbosd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yuwvrkmo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wqqsjaoe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zwodntux.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2abhpqwnl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aywfibsm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qfubvgav.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ctkzzykp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zmzrasvo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bhrlkmaw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oowujdgf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2snpauthc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2evxufoau.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mkhpgslo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ciqwvlvk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2paopskek.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2egauvczy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2euvzqddk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jmpuenvd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ozlnxarc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2squyndqa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2smaqnvzs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wmzwzaxx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gudanrey.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2onjcbvgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuuovcmp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vhkrjikb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ornfxnxd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sovmwhai.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qbxiauxn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kprpivpr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gryblegf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rvdalpnl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ggcqdvpq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mddwwqvw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tlxckitj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2unxkysfv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zybwlktp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jmiomwcx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fsduasjn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2utiljcee.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2doahlkum.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gbkimthn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wabvivfh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2osqudpxo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rkbdbbdx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2iosknoex.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wlploucr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xiewfzar.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2csqpklkw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ehaiajpw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pkutbimb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vlksgqdj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2trunexzy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xgcrmmlr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tgsbfhze.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lcugqwmp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jwaszchp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2aygcdifc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrkhazif.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qrbvumlm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zhperrbj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zpsabpzr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ltiumzkj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2porfufqp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nupbhmcp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zpiizjpx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jswqtgvi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ytyuqzzu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kxkbfedz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gkbvewom.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mbngkfzj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bttqebeg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2atpswxbo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uqzksjfy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ixrngyde.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gtvptcso.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mdtgftev.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tzacsobe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fibucsvl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lunjubuc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gtjruesh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pcqclblg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ucikuxks.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ffnrezvx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bftqqddn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ryjjzhoj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2svkugfxr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yqlcziug.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nwfhcofm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2awnxtfln.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2msfederd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uqggtpjn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2enzqzlma.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hsansgsp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qfjpmqro.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2okairuzn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2knlpubnn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bsryuxoy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sachxrds.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vjfcyxlf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eamvzwku.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lylrtnty.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gyndvptu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dpbudmtu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ceydykfr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tyfhfuhy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hntcufbh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pvfjtbfn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dqtucolc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fqagmaqs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jufpvwqi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xdoiuqfc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mmazlkrf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mljalybf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xaynfofu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxrdxvtr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vtbawqic.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2biqadboz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kdtqsirt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vrqqkaml.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gzxlikpe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rkhipian.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jkqyqabo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fmrzjsok.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvfmwisv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ubjmztjt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujciihxe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qviqnoww.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qzghkqpn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kfitlcxs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipwbiumb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rtwzbbec.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2onxhioka.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oforxnqj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2immzlulw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2oflemgfx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2suzntaya.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yfxehfit.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2phaafiac.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sdownhxj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kezqbcbj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2umcelcle.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cruszknf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sxfekyrb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lebirnjp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cmzmcbxv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vtqqlnpb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eczlyran.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jsmkpgtl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2fpmysfwh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kamyhnlr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qzqaqizl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2srbpvdot.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2czuoaojv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftfuemod.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ghovqqos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxmlsxch.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rssazbsw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zxatdvav.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xwwxliqu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bioqklls.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ulbvhuml.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zuwfqbnr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ujzhegqj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ozvaagis.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kdjyduue.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2aqnpokzo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tlgvgstv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lvaxnexh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ybchufgt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mdhmmscd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fszulgpa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mikfzdcn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2etvjijgd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2chamssgw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zsndazkc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pnwiugbr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wvpdznni.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gtydjcsg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2twodmajv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2usjltzna.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vcnbwxmf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vhltktvi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sdjeicqn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xxenrvqt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vorrybcp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qifkxsgf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ktirqusf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ywjglash.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2allqbvum.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2khlrqjun.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ntkvikwz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mvsgzkcf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zxarnutp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2znxajufa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nqwsucpj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xhenfszv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cmnscrmk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2crqnphvz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lhkrvyfm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jecutxeq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zxpcsfmp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2irfehcpv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ugswhpvg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tgmdxdjg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hgfmhexw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lyjxhtse.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hxjhduxz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2euxotehj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2phaxlcsr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cnzymwsg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2brlzycoa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gttwfbkk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rswslczy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cjofncnc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ajxabkol.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lrwdghzz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qsrqexlz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wienuvcq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pibtaoux.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kxzqrshf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kraxlpwi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xxeyzyzn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vzwaztjf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xzfnxigw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dtbjkruh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvzregyo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2veyylmdy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2snaofuyt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hriwvxyv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2phpcuqot.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cqfzcexq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2optskqbr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wnrqgohn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2revvacud.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nwcfsbbb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hbqflfjl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wsgswfao.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xneamltm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mqedqkbr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wopjkhgi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2unoadaug.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mgzpllot.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ixhzicdr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dowgtijn.html


<!-- 参考信息 -->