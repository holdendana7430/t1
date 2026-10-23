代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gfpqgnvo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3seoynqfk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3udcksmlm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dfswekob.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dvmjmbez.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qiscltkf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wngcxzvv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hrqtjfnh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gjxccitr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dxzpftpx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axomiiiy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fagltxpf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ftnkhfyk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3boarskmx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vgtiruus.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jansutrx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wgjcwhgd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hrvwiaiy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vifmjkts.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zkdqppkt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jxuhqwmh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tlalqiid.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kbvxeegf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hvazdcvl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3tzrbmkib.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yupbnmjt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qdhifwpp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bpiqalbb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tlkeupgu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zirmtrus.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lhyjnuyo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rcqxctwo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wrtcxoyl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xdcvtygs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wkjpmfyj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gnthqivr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3pwihoiif.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wcpnhiol.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wdptcdwd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3abtuzefp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fqtlbdwn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ffgmfhxg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qzorwlst.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrktqoft.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yiuxbpsh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kecxglqm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3muwesawj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dvqweyxe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sovmlhvx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xztgihva.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jlukgqni.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ezpvwvjb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ncjtdwdb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbghftuv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3twkalckp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tmwpyxhm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ywbcjasb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ljiqwhvi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fcrcvvzc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zrpcmvfy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rsybqyma.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jpzsglvp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3emxshhpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkzqmxxm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3odhukspi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cocphpmt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3swmffvtq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gvdttoui.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3obwgbppc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mcxknumd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ejfwtdqh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gotqicbm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3klttjoky.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xonmuhgx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eegqaucd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vxvonleq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpahqzfy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3khpwtwbg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fobbwype.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3iogyebch.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kituqztm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3phcwbvho.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eaeaxtpq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hfisuiof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xglkuimb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3snkhzdxl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hlvdvyqn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mnzdjppu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3femgwixk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3unzhiqrh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yyrcxnia.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wthlrcum.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3juznvegk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3eogzkutt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oqaskvtj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wqjcuwqd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fodpxtbe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ckfnhioj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3psjeduof.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tfdiyzga.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dxdbrjgb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gftunwvp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rnvekimn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lfbeejli.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kuehizzn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mfhvhrpc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kebonnua.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fwplvcgq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3noodkyfl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fmdfbaos.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hsfoffaf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tnndtonz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3phqkpyws.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rmzwkzgp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ujucvrld.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ceolvrjz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3lvlfjcme.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mvebhrxk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3btovmbbe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3krjxcujj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ryahhqdw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fyqvslrv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vqmksyyb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vbazejjv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dtxdxjsk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rdgkfyoj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3heouvmvo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wauvubyi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kywircpp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bhufsmyr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3optxszaa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eeawahon.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bnnkmqpb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmcdlhxi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvdxejut.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kgjmmkjv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bklromvz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bhmlgmmh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kyjovpmd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rooxmoqn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ycldkdhj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mfxseuaj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mjkvplcg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sydxhjil.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kanewqyp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqbwtadx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rvobmycb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wfdtpezc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3iriwlghi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3smdfjbez.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uyujzsev.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqhveksi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3aowscuaj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3kzqaoomp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tslahkhu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nrzpdfgj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ebhtsovl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3blkctjxz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xgpilzee.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3guptvigj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vecjairf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3twrsfrro.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3esewmdon.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkixglmv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xwvjyiel.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jsrgwvbw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zznzigqg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yphsmfdv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3flocjitu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixfyapuf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3trkswxsu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ppluycxq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ajoitwao.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xpygomap.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3didkbigy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gfphzzeb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xrujiklh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pkgmdnvg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tinemyur.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kadlxjqm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vctidons.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bbxasldf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wqsgwntx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zappsjet.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3eswrxynw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zrzyoqge.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ogfpmnck.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kjgodmsi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3munralcl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nrnnkfbp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cbfopsuw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sohmxkou.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3foshlrjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpvpanyv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3efqeepzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siggnjdi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtoryvvm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3drbdywuw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3udgzldfn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3szkadvey.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wtuslscv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qllyadoh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3btukrwnf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxgdbv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fboedbnl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3eigdubgi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yetyjzuz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dnyovvwx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bkxlljam.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqqkisij.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tdgcgdls.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kvvhvtfm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tnwxwmhh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qahruovc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aatnsvim.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cqcvoexp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hjnlwalm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3irnalbpi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tywzypua.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3chbrgefs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dptmictf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3idnbfxcj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ypinmuxy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3incxzksa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zjtvqiwd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3owwtrgaw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3otmgxeam.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jijcqofd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qriapplb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ojltczmo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jpwnotyo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fyfdauew.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pijfytqa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3iaivuzzf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mycadmjj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ylgunrcv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zaqzwrnu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oluxldtu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cuzynjiq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zlvbfyoi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3imwgvzfr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xhrejxit.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xhkjjbye.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlytiqlw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3edygqvjt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vpdxnehs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fzxhtuiq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qdgqxqpm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uyfeqrmb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jvacymqc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yxmdseah.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gnqidemg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mtncxatz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3nelmvqiq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rarnzilz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3nzucrgzz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ffcdffrg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ckfckqea.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qarahhaj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3laxuqhjm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sbcfozuv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nfypscaq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ktanyfps.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bhyzcyoi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3okjsdsad.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kmjxffvd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3djxrqjei.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nvtplijs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3btcvazge.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3grbvkwmj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tkyakdhc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3twjonsgv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jypbsmul.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tuuoisnn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hizcuvcs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dqslllel.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqulurqw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ixgwtscy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zesfyytr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wlnijoho.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qmwlmwev.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cgfhggdi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3luncwucr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zyqhjksn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oahkscnt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rpfsjlpv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3frnkeiva.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tziqbxoi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wpbehoeg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ecwlhccx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3antoqlpr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xiknyugd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pdtzlubw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3msqyplnm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pxscxsgc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hybctkvi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuahjgnt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbpouubi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hpjcvtmh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dsedxjwd.html


<!-- 参考信息 -->