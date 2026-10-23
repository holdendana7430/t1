代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dkdblaqt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ujyupwsr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ffqoucca.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hrepmgkq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bkhufytv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dtxxlgab.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yaykfgbz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uwuasbfr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dmqyssae.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kzjofywj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bcluyprn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xoqskeuz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ljvwjdyz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zitxoodp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbyyaxyu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tnwjyauf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3klalwhtx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bydijciu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ucraieso.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mresjcta.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3tcpgooiu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nglujbjn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dvgpsvdl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bzkomktz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3igvimrjf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uyfzwjjk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3klwbyhjv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pdsdnwmv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3emmyjzkr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbjmemyg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aicyrkuq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yjojgjdo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wvsxfzcy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xgefqwvp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vmdekaob.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ogkotfti.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nzfjrfur.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oklbsexf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mlvwjxjg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qemkfzju.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ypbkybjx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dvddnsyq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ibwtsrzy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dmktustw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lcfnuqtx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3smwsagir.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qjvywjsj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iqpundar.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3iayxqvft.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3koqfgzxe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xymibdix.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3temcolst.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tsogbshj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qzzqopzs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tvctocko.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hjjppmqx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qrabktfu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3iuvoafso.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uugeexvi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vjqycmmk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3datrqspo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gpbjusyk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3njaeuohj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hykedjlr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3erffjatr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3stvyuvbx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uatfbkzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3methcdoz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ibhefszb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpzuedfh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdbdlkza.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hmekuces.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrcjqmuv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xczbqyer.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3inlziqlp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3byecnrej.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3igqdquqo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tkfqtizn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gjekfinz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jirmelke.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gicforrp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vvyuuvgg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nailzywx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rzuhtjpx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3twvagflu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3flssbpmv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ynsqcsgx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3inflkedg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nzwgufyv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vqzuoqja.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uupzwkxh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfbtudvc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3veqbgjdk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gbwatefe.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mikzbega.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hoaaumxw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ykwyojda.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nandhkcv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dxclgnwc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nauxyept.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uequctov.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nngpwkxi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ulekusyl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hqjkgekq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqwjbsdx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3plipjogv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vhxkjlwq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xkbufkqq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tuokgqel.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3trsyyhku.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mjdxrzob.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qodnstki.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xdhugpsg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3npdusjti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jlivfhmi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ljgqgyal.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ohnhkvfx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3altjktaa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3swpverkr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cyaydhcl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mlsngica.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3seqktmyb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vnhlgzne.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3azmploab.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wumjgqhu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3assmuywu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lgefmxsk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fzcixliv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vqhhxjhx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjrkozdy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bglhlalz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3juakugzf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dfvbqhix.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mzhaupzh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kltyubra.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3biilsqhj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dcxvfrym.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yhamxrro.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dumhwbhk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rtlxqajd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pcwkjhqt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3olwwjcpo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hweougnq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pvdudlzv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jqpxtdng.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3soyxvxbi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hmjtqvyv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ghchynrg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bmmkmniu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tvlqdqwc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vrmjzffo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bgshihrt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wcmzqcjb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xbtcfnke.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3laahudig.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ogysmxis.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yatefadw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bjkmptup.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yxkimqya.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3amronsvw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pklmtuxe.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qlsavxzt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mqpwphkn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jbcudxob.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gxiofrxc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uvwuxbqh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yvrfyubo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cswroupt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gfawsljk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3opxftkke.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqkfdigb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3etcmlayl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oirgtjnd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bexhholt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rtdttsal.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dnzwcgat.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cscswmdg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3edcruldf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vzmtmgdj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sarzodvq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjhopwmz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zqykmeiy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3msmlxkht.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ogqbuzfc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3stgqwaev.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dmymankh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zmlimdkz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3netmukdi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nnbaffxo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3inucqrns.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ztawvdmh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wvvrskgj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3snxmclja.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mspuhddg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ahbaerfw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3srpfwxad.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ygwdevqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uorsbrkh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eurwcrmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unjupnuc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uomfcpcd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hayklxqa.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dbqkstus.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hhrdvnxr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ltcgscvk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xwvrmkzw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tdaolzbp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nwkwuukg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3twqcetoq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3egouybcs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sisigtgj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ruecustl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jzdzoqdv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fcpuyxdo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3katcwwut.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gswkkmhi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mlehmhil.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3lwyzopav.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdqevftl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jlpadgws.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wkhhssoy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wniiwwrk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uytnabib.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ankxqbuy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ofncjeui.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdpioxzx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dovlbkzg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ypwusrsm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3oeotbebb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qfzhwedu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vozflwgw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tgmpskyc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nsyrowbf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkjzfqwh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ynnzyvgd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tnuoeqxu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lynsaiel.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3eihbdvah.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bzoealwo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jxnhvwul.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ostlhtek.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dfpcxsso.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xeeukkya.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hlweojgc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xnmxvopq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3acqdrrbb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bdaxbvty.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3njikklsw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ebtgjcnn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ywrwzbqh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lwuvtroa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3akacpkbm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gylhobnh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wmknodjh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xkgkixqe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mqdldjjg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3aojbrtza.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mpkzgzsz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uktibgsz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ajijhlft.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kasuactf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eamohthw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3azkmmqvv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ajcqztjv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iwohxsgb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qoopmalj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3twxmrcjn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3oupiufvc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ehexilwh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ufophejt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3oavxkdyg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ettyymsl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zpacdgcd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dwwfthsj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tkkswvqm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xdrwcnoa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3obgpdjjr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3urbdrhee.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zhsfhact.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sqdpepww.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oxybviuw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3winkjhbt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3edjuevuk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mxqsczsc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pazxcuwq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3weuwwwax.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bsimrmzs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbsujpkj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aimyazyj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fxjoembv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3thwkozsq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmfuijjm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3puyxkekk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbdrugrf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vghruavh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rgnhviyy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rjfmneav.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgktjtms.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gajuffni.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fdkwziws.html


<!-- 参考信息 -->