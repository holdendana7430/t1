代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nvxqfmvx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2cpvcmhxs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ywtqbwqu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mprgwbhq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2aaaiczdm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jsozmxwz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gfjmufpl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pbmvntwc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bhxtuiod.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2axlpftwj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vxgbkqdf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qlvptmfl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jmisuhlp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bubiffpm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bjcsuslr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rtxgdfqr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vmdtwtxo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpksbvkm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yyjnymrf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ymqzivhc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jqjjjzcx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rjhmblpw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nzakwxug.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ogsasqnj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2omydtkni.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2aklfpjir.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qdvdbjxq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vhrctecz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oeblfmcb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hsplatnj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2imhoawtz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oefgctvc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2iimdgbux.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qluxyvba.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rnysixna.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hmquzult.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uevrbkli.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2drmfturk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lwvpalta.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rijbrffl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qtpanebd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2htzoqjhn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xxpyynji.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ockgdmns.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lxulqlrn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2orknwxej.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qlzqscup.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2putiehkm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ohtjntvr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2yqbqywrq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwyptndi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ezsqwrbl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gdmbxxfn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ycxhutin.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rannkqxu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mzueiwip.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jmhmjkyo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ultoxkqu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2uigcgqcj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hegtkrmf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tkntzsov.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lskuffuu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vwlereqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2boxrifow.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mbticmfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhlhldxc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kqxsfien.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2omwianwk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uzjbgqrj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cyfhuefc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dodcroxy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jttshxvg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sgvdvlni.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ezancebo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gikkfywg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dqbljvij.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fqnqhzis.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vilpmnyd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gbdxmnzo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mvrahoqo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ficfaspn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qnqfalgi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bpaojlus.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rcwvqwmt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wyybnmxb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2oxrcrjmz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cxuyboli.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tmgsdgzb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hevpkbyb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fygnewho.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nwklhjbr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jcglprop.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fesdlhok.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2otjoskak.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cwdhwxsm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cohxvwld.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2negdymhw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zopjxwjs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dtcoklzh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zmeqfyqr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xvgkfeno.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xvhememf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lflupnao.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xzygonyf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kgctkvcm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cmajxnih.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jqgxjbih.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ztiolyjs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lbmcjwao.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2teopgidn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kttvdchz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lxeqcmfx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lcbhdxmx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tlpjahvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uxikbztt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wlrighta.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ysbowiqn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mvyzrzdd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qhmgixha.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ycjzdtsm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kpfqyqqv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2esrgbosj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lluwrkdj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cfvzvgmd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gqtvkszx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nzquavny.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwiixhq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ubuvnron.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wujhdxpp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wzwxzjer.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kmupbozb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2labpvege.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yqbiclge.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kygdkfse.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oergkkhb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qnxmheaj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xfsbmtnu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rdjxpgpy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2wsvjxclv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rujnfnmf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jhoatzlw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uajpilcd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kxewbkcj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dhpcnizg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zexaqrua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rglqmcai.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2whlbidrl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2oxzjddgb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ylkzhfad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2surudxko.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2thkcmego.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2werrooah.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mqtsrfvq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lbmwobha.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mzfaxekd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mwocjygj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eitjfoya.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fbiwkxjy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uczojhrt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oadantyq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qqvwpdud.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fjydggho.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ajrhutow.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pvaiotis.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iwdqnwce.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rqvzkniq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlvbcgzn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jzphqokz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pzeptmpr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wuendsvv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xddebmkv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dqhtakeh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwodht.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vmxjfkbq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lrozgqzm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ngspffro.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qhebfnjy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ffzjwsqq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fhzkmpwv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2acuqcpaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dfjkuklt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ncexkoxq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nchaddje.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ltrqdrxt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnjpyrvs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rislzxjm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mtwjsfwo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hnbaunzi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pnulxeiv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2juluhmzo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2olskzhpv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ygevrqgo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yssvmhpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khiryvry.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bxcbbfnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjvxjdip.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lnxojzyk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2neddfezr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cspsufkr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vyqecuco.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2uavlnklm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gbhxfdqf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2peywphod.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yddqowcd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wnfjbojm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mknloawd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bjazxkhw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjaviwy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2buvkqaip.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ztaivwna.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kbmiocuf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lwxmfbcf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fisvlbdj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wrzgddrn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mwbjyagk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xyirmtgy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pjyczgfa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2blmarqvl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qxyktmyp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmfgbri.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tgxegabu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qjmrcrqx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2usvxdcub.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mumubnuh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kymtodlb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mbfuqqff.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbwrioso.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2veeugbre.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tfzokbho.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2brvajmtv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pcwvzjal.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jvbxvgmb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qjmlxhhc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jagfknvl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2umuidhfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfylifw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lhgwlohj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ceitrolg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rppsvpin.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uflxmden.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uikqhroy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qgbazxmj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mvinfdvz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2udftsdqo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gidculpd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pjmweiga.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tzfwiyxh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nhywvewj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2loyqkyhl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kgxfozpv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2efakdmws.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rjwmmxfn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ieblhgeh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2oifhltzh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tiexfpga.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fcowksbf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zzwpmxke.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ltkvezdw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hutezpph.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mgtaxiha.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2farhaung.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yxxmgrdf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zrxcuidn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iprdovcl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ilxxpkkm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sfvgiqes.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xvqdkloz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pvjqvosy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oofiiwfg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dtuihrpw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nfgilfen.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lkmorgwa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ywymivcn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lnhqttoy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jcoanwwd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2aemawcxh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ethalgkh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nfjdkteb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iyxyspey.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eyoldejt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eltpxfgp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qytemmyj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dbzfedhc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ortdzxut.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vtnbdpfk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cknqzkpg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qgmnqaxl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knrtjjsp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgpwec.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2sesrzhsl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qpkbpujz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2avlaobfk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2knxjlzpr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fqxdzihr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkishfgq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dorpnaen.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2euockvxz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wpyvfbrn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zlgkvqdk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wyhqpkhj.html


<!-- 参考信息 -->