代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nvpagcvb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gdwgfdrb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2roixywjn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2eadvzvzy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qtvkbken.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pieqlmjf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgnlwpsw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bgakrrzm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xvltayeh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vyevfoio.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rrbkfmyz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wczlvvle.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rgsjdjci.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nwqzepnl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wvajdovx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2itwlbmvf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hbccdfev.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yvivrhlc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yyzmfutp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tyqruvuj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mmoktinz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jdmwwkax.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2swzehvqz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2euiqgyrh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2igeitgcx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xixrmbam.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dsdtypap.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lvccovdz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vymvboix.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gctvwdim.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2alubhraw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hpxeacjo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dofqbmrf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zsmvqgvb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ndasbkgt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ldnnzvfe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vcfiucmf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zgykevjq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xxsjqrkx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2aongvyng.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nlzzkkgi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2aypryonu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2emelcjet.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ppwxnnrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eltkacje.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2agogtynb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dehbalgd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rclrccdn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ymyvoxhh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wvnrhqmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rnjszhmo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tlpxzgiy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vpiuxnuv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gprzgtkl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lvgmqaai.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fvgcyqdz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vsgxhbuz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rgbelbff.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lpiskgso.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wfmwfsqj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fggbdxlo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xndoolei.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mpkutguq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2coyyduwv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2axdtxryi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxfpbrfj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tgsbyauo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2njnykszr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oxqvstfa.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tdxzaycg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fdrnpnog.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2azsondke.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jkjemaaw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jyxhknej.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xloxspgr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftqcaucb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlzrfnfw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qcxpvxak.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tdzepxuj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2svzlccwz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hsbonruf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kvlnskqq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rqbiyjxk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2onnjyfql.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2opnnjeig.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lqehfaqf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2whowkmvg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdxhpqfn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xeuwsjow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zxyomyyi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xgpmwwey.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ruazlotu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rdwhgeaz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jkmfohbr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2krsvsbxj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2akodbfch.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qgrdsart.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ooimeprp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yzkfdrbs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2exofnwbt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rbncwsqe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zglwalyj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vylfjzym.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnbqvtqn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2iukeahbc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zcopujzy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pfvclcme.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yuscxozz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wxjvaavl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2exlmpofr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gntunykx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ywuordyl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hgtrohif.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dgxgyann.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2btrogmev.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bwbwouag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ekzacelc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2svphvqjr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2udttpsva.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2udxkjmrk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tbqtvyts.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mbxdmazb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ulbqmvwe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fljbahzy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sqjclgvi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2recraili.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gzqjzybv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vkroezre.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dusscuvn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vwphsnhx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jxuehhqy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uoiaodub.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dkfkcqvm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2seenaugk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxvtpjal.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vpsglsav.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yuspwiwl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ueozdglr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hditvuwx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lqelzvgg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xecabtms.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2andaakim.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qdwqjrph.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yqfvlgzp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bncktteb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rruznsqk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lrmkgjlk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2swnpplek.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ykotifrw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jvxbdnfe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wxniwwog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2npsfznls.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzomeroa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xfcavzia.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xymzqarf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dhkvphgz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2skvsrcqu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ozbxyyyo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yddrkuzq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2aotnxhms.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zdxnlkxa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ngxhhyts.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cbblfrio.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ounwyqal.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hmficslk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkpgnpz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pcniidlg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2leroguxz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fzbwkukj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hszorxnm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2korxtwfd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ieddzfro.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2puyglyrr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gyujepxj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ygnknwao.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wcjrkxnr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2izxmaldv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kaxdsont.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2llhozwaa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cobxirye.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oixxfdcl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dzjotgeb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfjtzgtd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ujiiqdaq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fahcfckn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2oohjizup.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jvrkqgdf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wcshzoqj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2syleelit.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rymqsike.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wmwqgphm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2crpccupe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nttvhjgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuvhgfnr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2upqtkeqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psafkxmk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mowiwfxf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fdjknjtu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2goxaoyyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vkkvytmb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2srmuyaja.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rurejgjf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lwzbmhoj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cqlfnvoo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cpsjpvhq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ptnhbgsh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qgqexpuo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ieccalna.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2crnjqhmm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2arbfwzpd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2enehpjvp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mbzpltns.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hitvxuob.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rztgabgx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bmihroug.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jeagoisb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2osxelnuy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2uijdktvl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fgdfmowf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vodwtoxk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fnzjcpgx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ngfwscmt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fgppmflh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rdcheotl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2snwsxpsy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2emsbkehd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tcnbsfzv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nacmacqy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wjrakaim.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2msrvaoix.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dbuhrbdo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dspjceee.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cnuqcojc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pnnmlfwp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2srgcotzm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2yeqoofqe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzmjlahs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xposaigw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2sbmvhxzq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2exbbbrkl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tdhtpnup.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kzemhsxm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yhigkxyp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2advrczhd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vxdqxsqf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2eftqidzy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nggzhmom.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dgvnvqel.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2znoqgaih.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sfswghtu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gvrxbxne.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bwufnuly.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvsxorwz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2spkpeowk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tumxjkzd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wxextsoe.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dphlriqc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gmfateym.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhtnnbbf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bemoyuee.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2isbuzwkp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kbyuqixs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fwgqmegl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ekglyeuk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pwehjgvd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ycubyaet.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jufejflg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ohwspmsu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2twcqdvzd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tstyimmt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bvmrrfva.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fdxqwabv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kjxhswdz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fvxldkez.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jmemgtvj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nqyqwkyl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2njghirmd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gfrxjdkl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ymwxtyij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iwthcnhb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iwlqlrwx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tctxdjrt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ysznjrgd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ljcpsuis.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jxrnjlmy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkelkiau.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nebunske.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2euucalrs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aiaajula.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2legarmcp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jdzpsdhe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2annmkvrt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwjjuigi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jcdhurwt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2emotrjkb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vizpqbqc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dozytkxf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hrokyqrg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pcsehlgi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hajvgmsu.html


<!-- 参考信息 -->