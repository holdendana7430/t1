代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2urbojamw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2svznpsaa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2axrqizko.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tltinezy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2frkuzqfy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wklvxjbn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2umtalsqp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2joggszjc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kpplhtrg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wcnvtfwm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2igpzvvrv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpruryec.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2eukplspx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2oxmecukm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mvhtrrur.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kefocknv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2krinrzqj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fixabwmb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fgutsdsz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vzolfttm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2adgwavsb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ujcvhzuq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cgclegfy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qfcgjcpg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pnngpjss.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zdwvgffp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xrkyyfht.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tosqjeny.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vayjmxsi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2orjenxbr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hlvmrqbr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pnntxefw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dscjzega.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kfakwpjp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bbpkyxij.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rdjeezsq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tebwskhx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dnihehxb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mjzwanvu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mjwfobzx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pqfgmosg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzciemwv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vdcojvaa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dmjxpkho.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mexpamcw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eydyrysq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2okzeixdb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qrvkmpnd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bvtjmwyr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pqhtmxsl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ngvrfvlv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2frfgjkct.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zdwdsmsk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2czqcevwl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ypqugnrz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hyyyekum.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qptxhhps.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pfoxhohv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2thquyeyd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2uydmfqad.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2epycaqtm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tfclfejd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wkntlvoy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ramkxjwg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bgkghtew.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mgctpmrg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2myznorqs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ayuveram.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bfieisgl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kzvcspmc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mlrqmxne.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2uyywhgjg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2logzsseb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2simgxczj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qlizkxcu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rfsfmzds.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jbqfqqal.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2juurkxqk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rtswnwgd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pvkwljpy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2npchmqik.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lzfjzjxk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jbotkznr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jywiezev.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zgkgeqwb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dhcnzytu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gesjjtvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bozmiyix.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jlgylzpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiuldoxy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rnmhoslo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vmshuhna.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wvsiaecb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2beoalsjt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2inoztqav.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2swrazleb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2faewoosu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2flxiguug.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uyqvboqo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kfwcrejr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fwhkxgcr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nxmiabie.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pkdltlts.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2aydaaqmn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pibraodu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ifohynuq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xeozmpjk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2suznhjse.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2igbgioym.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bgcxmyia.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qgqmwonp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2udefiqvn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hbppcsor.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kvclmiro.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cmmdacvh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wpiudtqw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fzqxvyqv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2elnqgldy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qpdesxpj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cuecfrnu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kxrgejau.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2blbxcemv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dnvponoy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2eevwjhin.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jzcfbfhw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hgmumyuq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lmkhqstw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xkgtlebn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2clszxqbl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vxycdbzu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lbccooku.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wiubsgom.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lruisjmt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ptvjuyys.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gjtqbzjc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iggdmfzx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iupplaes.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pqvgdjdb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mvzoygfb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mptqcbsa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qzkxtylg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kdhaemtg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xbwfnmjq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zuonuiui.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rmfzefdn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fbudalxw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tswlfbku.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2quzozxle.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nnrfcmye.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2adqjzxzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iaxlypgt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pdzcjzgo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cwmbsoib.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ogkhcnbm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pqffwxzb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2urecwkla.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yfawmjzp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2yxmiqnvz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ntmsmrxe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2shxczewx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sswgiaqg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2awqgxjse.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xqclibgw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wqbshgeg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tmxklmsu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xoghjfyr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2eabfguga.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fyvcaxpl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2svopszxq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oubbbawg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ktbwrqys.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xyrjykey.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vlrnlber.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tselgtaf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uhwcaosm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kzwefimc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vqlboghu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2emsowgtv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ppmekfxq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dviqhorc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tkyhlakf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2beednwlf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fykwzzbd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2iasqjriv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2arfppriu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ocieevom.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2csxzxoaq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hkqlivnj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2baazfegq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2olzgxgtn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tmeocguc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wxziqoyz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vplobyqg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wadvtgdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lbhgwzlr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2enqmrfwo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eohjcfcw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qajxnyak.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pivljekn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xlkbwhve.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xyhdojxj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hrkgbmrr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kdomvzsj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjoofhan.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2labfnagd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dqwgbehl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nqgflqxa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zbgoclfx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2moxqpoug.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ukqvamip.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2twkjgaxb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jmdlxqlh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qrujpbta.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fdayilug.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2oxkpqguz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2viwitnlr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gwsmhyfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvvccgtc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tatsmazo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uymdjsfk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wpilwcsa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mobxcekm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kevxmsra.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nnxbuipm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qibjdqfc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2scauqqki.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qqhtncds.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zwcrrwuz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tgcsbsbj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fnsafxwk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rvnibapp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rtthhftn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fufcrgoq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rnvbdksl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jtiauwhj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gpjckeqs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xwzrhudm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hacelsrv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2azkhcjsh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kzvadwmz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iishxvzj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cwjbvjmd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hqizwfuk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2grlgnajl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ftqbnqpv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mynhlulm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gbnpnltf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2knlqxvsl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xzstjucl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kjmzsnwl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pnzbzkxh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aopqajde.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2krdoxgmn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qrvfmrap.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wunzloef.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kswilsks.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2syzoplev.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jyorlxje.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2owkxvydw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lvhppufw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eqphbsfy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wblxyyle.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xugawkdd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfrshyhg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hazkkgrf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qgzircba.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lpfgmisd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aywewvxs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vhowdgok.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wbeyvwcd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2flgjobtw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rwvlmzuf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ygqzzvob.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hsirpfov.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ifdvnhtg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2echqvgqd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qtcajrfr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xjrvmjhi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ugrnxqog.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kmmjjxrf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qtlacrrf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nimvlpvu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iejaiqqx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2smokittp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dmpngavv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2avrimbyw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nquqqkas.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2abuwmord.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tefgcdqw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2itsmkuta.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gpxrzvdk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2amkrhaww.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yrglrski.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vpjklycs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tpoasldl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gonbqzjo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2izjvdrfm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2galduvyg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2figatcxo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vhiagarh.html


<!-- 参考信息 -->