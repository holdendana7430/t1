代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iyppgdjt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nldmmxiu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qsxzujas.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zvvonrik.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cwhjthgs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pcjxitlu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3atxqlmdd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3knnfzpvu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rolyisbl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ekxpmdhe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ezwqvdgy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bvgetnex.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yamrvnuk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cdmpppov.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njjfbqeh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mbyvwvvn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bkvgurju.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3umrtlvyb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3llqsgtsk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3knuacmpy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3opcaxysa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jyoconmd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3akcscsyi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jsmsowty.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcvosi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdpwzyox.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3baqpmzce.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iykxhyxl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xemolsgo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3isseonsg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3txjusoiy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3phpcutyd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mgzwsyfs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyrzbnaj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zfjqtokm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3htdhgpkh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tbdwmios.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hrjejtfm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cmwkvtky.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hhfsptkz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vusvpppe.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fiqedqmj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zndakgls.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3umohlzrs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zqrunoma.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3czcrnlto.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzbhgagn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kjogloaz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jlebdzbq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ljtblrbm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bwgpmsuw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oehvizbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bssofldd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ybvlrksr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxlxoxyf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3meugjykg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3chvqvoxi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ztvvjhia.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdctwgxi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehwitnuh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qglexryg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcjfzbmx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tohymkyn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sybpurup.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xeenclqj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kviispiv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xlpcpsjf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tfvnxrlz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lygnbtrq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ttmlclbe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ezsavtnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idnugeoj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cjhokdqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bidogexz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hceboosj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qjsofoxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3izcoakkt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdvcsg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hmvhuigv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dudiskyd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3frvhaoms.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3utwwjywc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3umzfpxds.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3glximtko.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3spooggsp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wmspoqca.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ezweyyvl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dwyriyia.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dxwsxpmt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eerzfzft.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ostburnq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3enyqursc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3oqhpfxvy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gyctzcwa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ftzhwatc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3szvnsgul.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vljjewng.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cxfisxcs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vvxxotqy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3amcvxkkv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uoawqglx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3skzrprzj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kzblsose.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qcvkaxlg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rcrwfxpo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3douidqpv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ottkibdn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wchjfgdg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rnfqjpjz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zkvzffzd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3afheiuyh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dsotzhuv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3chkaaqbv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rdusihwa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3saiwoodl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bkurrhbs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vbbblxko.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kjlytkit.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ljgkpywy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3revphuia.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cpjfdcvm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uospesov.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tozcepzy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3utqbrhlj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3usdafdma.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3excwrycw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wtezggus.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3juvlltvb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uuyauovs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qenhlnsl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dkgtcwss.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fgxkmjhp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vxoiblhq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hyvobewe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ethspdcg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ufprjtqd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qkaixjqk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wkeuogsx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dwqqavcf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kryrkikv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vuecolvw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aydbzuuq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xrzjhbge.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3onyaqjpy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vvgirivr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ntsvocva.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qyjgwbbg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmvfnqkh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ampiugun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3drgzczxh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ruzdngbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3utgcfhds.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ezgmeanm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tshuvejg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3blvaryyq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tqhfeouq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cygcsjtb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lditpord.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lsifximv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qpaulsrh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qshkrbyw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uzelhlir.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlmisnlh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jwdxenec.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ecqefgyj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iekwnvvz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3swjwewjn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfcjntoa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nmycdylc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bcliergn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pqvcrrmu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yhanijui.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ystyrnth.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffsclpxn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zptofiwd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ufjiyywi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bplelcze.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dejgback.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qlpfgrud.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3djrlgmlt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3efjksyes.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fggxrnmz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3odacymtk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ltxcjlaq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjjhdueg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dxllfqbn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xzpmxcsm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3neletpkh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jevmfvhn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ndtenqmu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mimhdbcu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xexqxnev.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ikgvcykv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jsoamyvm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wcycxjwc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ecatvdnm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zmvggakd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3sfhzgaok.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qbsbfeli.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nbtmxqcu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xqbnrmax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvbsrwfr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tfhgbwww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ziqwysuj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fxtncswl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vzzrprmg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yiazmtfm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3sqrcggvb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vnjkfmkl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mjujfwxw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gvuiqieo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pjqtryql.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ekkoeohc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zmeaqezf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rhormrao.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vpuucpag.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3efppofoz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lpgolrfg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xrohtdet.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bmqkhewh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vljeqood.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mwnipqlq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xqqfugaw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ycfvzdwz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vcwudchd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zhxymvsm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qoytbzcl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gukiyqse.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zcdadrpe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ebuqlrux.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wxwicpze.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ncahxlxg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ufzjicmd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wkehxifi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jtjclgdi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3avxpezzf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zxiyriyo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3afaxyhdh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qgnrrncq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3smnnnvch.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3falqptfa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3oaydrecw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wdsuazwv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3drttzqcu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3utohcysr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rzrkofbd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yggpjosa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3erghdbgw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpsowczs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bshqsxkw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vzayrtjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3idwkbyud.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dufzcfsk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3whipmyqc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3oycxllxn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ishzqznf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3swgcnekc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3knzeozrb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wduhfmfv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ukwrbmnu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3aniaymrv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bsimzqye.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3axmncypk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3abatxqjl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3endudtaa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijkvkdjl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fieknxbg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iyxdglci.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qcssvclk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3krgmlrwk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3sbizyokv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ghxjcehc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3uugmuyvj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ntxrdklg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tufnainz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nhzytcvx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3deeibkqu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kfqoysug.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gukwndns.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yazbcqtg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ahzbsanp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rdyftapq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jsnkmbtl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dfslvynl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zpbzlfmy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dtdsdohf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dlrpermj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lkdhajiq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oixlbuks.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lbsjlksi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pyzsicvx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwitlbmc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wycrhqfq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrpepeb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zwbfssjq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3orhcqqpu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ktqubmnw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3stvwcuqk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vnlsvrtg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jevihktl.html


<!-- 参考信息 -->