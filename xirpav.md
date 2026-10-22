代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tljtlnkg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nwgfwcnt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2obmhfcnm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wivytfhz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vtkxsizr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zcktdlmj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2soffmhfx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mwlswexr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tplvzoht.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fyeolhhy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bkqyyjjg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oviuoyqn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lsfaeqqa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bvevaaxi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tlvmngfi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xoznexnt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2coshpepd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2iooadfgs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2spnzlzpc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2imkdssmy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fvzbcjqa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2enpsdbnm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qzsahfyl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nrxbfksk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2oianqlzb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zzdmpdxn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lreuxhsw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qhguasbb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ocjqggcc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hjpdjrle.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ceeumxbe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jtsqkeqs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2sgsyudes.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mjbkbabb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2baawgzhz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2cmijqnaa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bmeigkoo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2kejsfksy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2itwalusf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tvsoqfjh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qjsbrtex.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qrahtgng.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xpsgbbug.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nekldncf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mkcusczr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tyimhskw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2oarmjlrz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hynszryh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mbnbfjhw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2lhrexfyz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2sfyfiydx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2psdmwgve.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kgvctiqk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ukxkvzri.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2acxxasqn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dxwvrvaw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vddhzvkh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xumybyzp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2succpgym.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tdlbkckk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fpzgohux.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cupnilfx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ikdsnxzg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rgiekxdf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lxiueiiu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tqzsipox.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2psoomczg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2psddhpia.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oxpobxtr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cxdfgodz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xkykttjn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hmtvweot.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bouwvknp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hbusbphb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gucsrikr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdesrsng.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2eeqpekaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkldtose.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lvqwxlfk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jojdwzao.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2innoqtcx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vvmnllgw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qotwiddd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pffkwpwl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gxgoxxxx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wpaaifrm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uhxpyrzc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zeqzetco.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zirtevri.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jtacjhop.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zfmzyvcj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rzdizzfn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fuhlomdi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xuigwfbl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fzvhsgpv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sceohpda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qijbyysj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2avobnzjx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rhskpxmv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eflbphgx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zcuzwuwa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bofzchsf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ueswonyx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ledifgcz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dgznikqk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zbnekjdl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lkbrusgd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jkhyunme.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zpuvfult.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yzzocwwm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gadbhgat.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wwzvrckt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ujejlpyk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jdmjqeky.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dbzkmulk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dqjekkyd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ilyacrui.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2emhtasjy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lakgifif.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2oarkwpgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ycumuudc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qnxlxwhj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xdeapbub.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yvcgoudt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bebkjxdt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hbzaomqt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hcciaydm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dbiunsyq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jnrotmmr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dslnzlxk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gwgkppbe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rznnvwfl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nswznrub.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ldyqbjfy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fmvjuxbq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kspwhkxt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wlttgwue.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jjypptre.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zgfphvnl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ezsyseex.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zneemsmh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2fhymioga.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wscbvdsc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbpycdzk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dnfkldqu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixikqnoo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpynggwa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wpiojmxl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pnstklfw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvlivmnf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wuzyqdyi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gdhzodqr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ocnnurli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qafhicrn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2prsihsxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wiuwmnnd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2prqjtabs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2accsyjsi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hiivgdtj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ospcslrd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kujrofme.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wggbdpwb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kebifnnd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ctcjiumr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2igikidjf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gbwfbsfx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofprqkvr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2klbicdwn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ijkguynn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mhdlecqy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dufnznca.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2icribyir.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vmzrjanz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zbvowopj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lslpghzi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wniqsphu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hrhuecrg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqrshmg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjivsuyb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ulwnqqql.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oxqbuqvm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2enmzccxh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2awartvgn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pxqptjxk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vrefqido.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2arcpqkkv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pycbkboh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2znchmmsy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2eafcktkt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2normnnda.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hhshrdpb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wcbgykke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sotihuir.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ftjrqmnf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hcetrwsl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nazglajo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lsqsfmvf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2brfvuajd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kjlakbpg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxncsi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vkmtfhsf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lebtywqu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lrvkpyms.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tjqzpglc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jaxsvdea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwhjyfzu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hcmomptj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cellhpfm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vjwwsxwt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2htfvxktb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gsoxxmaf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qxgpaxwa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dqasajkl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2itertlum.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vyvyxdqs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2uwoovufd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pmqflogx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2nvhbpivn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jjdlhfxp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gjeyrptd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wqvayvql.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uubbvaog.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gpvquszv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cjbzkzdp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvgwhhlo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kvtisofo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbtfzdtc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zottlphx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2svpgtlgn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hunitrmh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zqzsipmx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2evifzxgr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ungzbuip.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jgfocrbo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ykxdnnyp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ewvmnwhm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2emjkfogm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mnuxygmt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qpfvmpyk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mpdsnnbe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2etcjcagt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2neuhxmdt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zepmwgyj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ejtjgtpq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wmxblolf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yeisiigu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cjewfvsy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gqojozbs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vtjworgq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xiqgokwa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kpeekhit.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ybumkavj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2srgbooey.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wdtpquqi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jenbdqeh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nppsjnna.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dwnbfnmt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mmrkfhrc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qdzcmdpk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dizyqsrq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xpuugnex.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bjuyrscz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xbcbxypx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hxwqwvjf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqpdru.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lliwalvb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tyvaundw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tfszhkeb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dbfevavf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ohoijodu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nnqiukgm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uxjfexjd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wpqlcimv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2stbruzlx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2twhecded.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jowecfcm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vblpotxl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqdkmwcg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ypkgqmyt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kvefbywx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bwawzobg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bymrireu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hbunlrns.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2kqlhhdwb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fsvijnxn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wudyjlia.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hjvkdkvy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cvwapcda.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iikqcqmg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gxjsqbzq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dnxyrssl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fhpwrhsn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2udzxzxhv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ozygqoov.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gaxfxpjm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kgegjwav.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tsyqrhsa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gvtqowxv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lxitbkgk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtjsmaaz.html


<!-- 参考信息 -->