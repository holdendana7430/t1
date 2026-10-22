代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wpdjihjg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iwlccceu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zgktodxo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mbywavwz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vbgyutbs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcbekppd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qclgrbgb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fkhcrgod.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2plsqisgp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ltssrvfi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2aeaaqryv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ojhgraig.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2prcjnbbd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2frxomgyw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mwmnvbah.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ixxsbiif.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2crltcwlq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2armrmdhx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mmsatxdc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bwfhlrgy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2povuravu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qdrratwe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lffwlbhy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pzadeahm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2edjmales.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jrgoqlus.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fktzblqa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2omuasvol.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rwilnaqy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sduklpca.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mqewkufx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wkanonqf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eabrajtl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2oqsyslqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2blngqnid.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qnlhfldp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sacgchll.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2efpdjfpg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vcelgrca.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2asyqxhrl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pvqkwlna.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xtpicdlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uempginv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2krfsofog.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lhfokvny.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rnquecfy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jcybbfrj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nxvwijxy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmfvuopw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hifyjuql.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2agvfyrgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpchjdwi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jajaskxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzygqdbd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vckclart.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fnupgsif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2psfbyvcm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ajbmggjp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jcbwhqtv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2umweukbv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2exmziddo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gbuuclij.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hngnojyd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hwoqumdu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egqtmhxq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mbzqoxxd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vcgtfthf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pgotcdis.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jfpgucqu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yvyjiwfe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ozccffgt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ufztsvnp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2phepuicm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2scqklkdf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xuudedli.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zcfprsul.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2optjurfj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2slujvhdf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zwbmbujn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2issoiwko.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wtczybuc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ngkbiykx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zjzetils.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2esbamkje.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gmxlclwl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yckvcntg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xaqxkane.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yfwrmcnq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2eegcrvpf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2apcuftdj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hlqxvpak.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvmjqgpu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gcmcrugy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xcpncysu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ztexbjod.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oyfeqebv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ahbgfpdf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rxndyqls.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yrwpbpbc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2drssldhn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rhuwddne.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nbssavln.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tbgckllb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nurtifur.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uhwsrszf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xgvvmfvk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2josygftq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hhgefvcb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2danpwqeq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ejihgosd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbukhcnr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fhrcaasc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2luodowif.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2twcafdzv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dpsxajjc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2euprspyy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pofaricj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yoitsvmz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ntrewnbs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rpzaieyf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tcazyjas.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzcpqwmn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oqxhhkus.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wcynftqa.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tiefkffm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hbgukfen.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2upegztkj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjxdobzd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pyejsdtf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wjmkgtco.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fdlhouoi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sobfnebc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xtoiknyr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2leudmvao.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fikarqro.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hfcsfuon.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2clujudyr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qxdmujga.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lmgyqket.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjpffk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2edwvdnyv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2enszmaas.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2noilukhq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2emocjctz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tsxlfvge.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wfthhxbl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tdocmgty.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbtwycm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pzwmfahs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2egqwzkkg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zeyyznbh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzdotbzn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzjmqsqw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxaujcoz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rucqyryh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ikddkvbj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zirgaswh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsqhpeah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iprtibbi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rwteylcw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2icmgiyku.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eusavjnd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2caiivrbb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sejndjqf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ejovkqso.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fndydisw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lepbdjoe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rezqxezc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yytelnwj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xspytnnc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2djofkuxe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2njukoeic.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ylmgnamf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2siefkzsa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yobklxmd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2llqtxegp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wrriycfs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tmzwzimk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2irsseenz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yncgrqah.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yqxsvism.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wujhifvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tpixbcdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhiiwclq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yociytdg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rpsjfgna.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjmthbqs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yymqswpc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2cgsqaqnr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2makvigkc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gcdiyqkh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2epjvzlsw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sskwebzc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xvrnadib.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ojvtzfax.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2akzcweea.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwvlwxbh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvejzzp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wszqfpid.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nwhoiskl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fohngjdc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ujirzpxs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmxhxzdx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jupawdcy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ywjmwxct.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qynwsesh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jvvktmez.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdjbpni.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2figobcpl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2loinxvsb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nxrcdtoq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ooawphmv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tbbnbvdn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yagueovv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jpybjekc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tbuthfyz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xhhdglvk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jgcffrnq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hnqpquwk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cmdtwoef.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nxrakukr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lxvyvqxl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2clubxtwe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gvqozpyc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hmkywzdu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ruimulwf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2kuakeths.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lejdeoaj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmhvlqnd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qgtmvtsd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ayxffgnt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wplfqhzv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pzzrdacg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uxkuvnws.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xxvkhcmj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2txbysulc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jfeqyvdy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2etziangx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hxcipiot.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xvanhcwi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pwnrhivr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bhgqwgzw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kbpzryhk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dlmmgdml.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oehvgefz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2duwmyaxx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxlipwqz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zuiybftc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uvkhinww.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xddmzziv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ftspdnlf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dhrihkkv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2skdkuazh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hkmfsfey.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ymayqshj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zxfjyxgr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ybbnqyid.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cukfullc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jncchrpw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2skdhcqze.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pnrlyngp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bzpolijs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rtamkfuz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zwxyinme.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ofvnasqd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sxgmezti.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vnhepclh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zyldwhkx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ccwozilu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2htdphsdn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aywkxvdr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yjassuhu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ziwhdmeq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqcetqb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xnbebidp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pyelcyxg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gzaybqyg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2aatapvbj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ewdwwlgg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kywdsqwh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2onnvffdv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2salmjdrr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gsvjdycw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tscjqcmd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyebvuyy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zenqnymq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cuvinzyc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pfgrgqrn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fyjqvohf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2keojnjrp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2whiyjper.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wxjxaltk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmfbqjq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2azkvfkuw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lgdyagcm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bwouyuzc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dupcidfy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2azqtilwd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ovjmswsq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2agtxftoy.html


<!-- 参考信息 -->