代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qfgrgwok.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yuhjzmzs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pftziwcv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2slweocgx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xxkxuidu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qffxbwju.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jvjbadhs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sfgkqdjw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mgwuzgdy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2afywpzxc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ypokngoz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dwwemipc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kayzeeic.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2svdexsjk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2czfzykyg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nduavjbj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jmjvposj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xvznrtku.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fqomntgp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jvjkhlfu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fpgutryj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2atqzbefd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sososket.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2erptwnmb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ogkvjytb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2digxofwy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uwlymllq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2boppcojh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wzhilihz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fipmfofv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2efpdytsd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nijniebo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hfxvqqhs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2phbpmoyo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2icbixgma.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2evikxaix.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ftxlmzrf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ibbhvhwp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ctsgszjc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xqvtgikl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cmblnboz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ratfqzum.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2sdnoejte.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2urctpmpw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmpekmec.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cvwfjrwl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zgxcahsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyrczmdw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qnfrmxby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmuxppvk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycuwngsp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nqhgmwnp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2idvldxqz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ujexrtpe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cjnpvrdf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hyuofsbk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rriaeaux.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uvxxgcgu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hjbwzvhl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hoiwtnrc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vuevzipv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mkwdoxwu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2eguzfpzm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wbyrabfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cvrcjypt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fntzsevi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ealmdflm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zfovfrtx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2swgtrejc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iuivbxar.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vsuwcvvc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhpbdpuz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ygxiasou.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tzhcunnh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bkboniyr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xrpvrugz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gnkodtmt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ekrmgruq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vxbjemby.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ctryfhod.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bhbuyqdt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2djvpsygt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kkkwxozg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hlgrfuvc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2unxkwwnt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmqcqp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2glkvprdr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jjsorfff.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gipfwult.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bhrvlhdh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ntnlangq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ygzccukx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qlqydpvf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bkdcrfuk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qxvrypgs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fxaifnom.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2adilnxzc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uhzcdwxq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kpmwhjhq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2meoybeyn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pjmcyosj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2oijmcnez.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2swuufvki.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xzuqyfqy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2osrxzcvh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jffflvkb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2utaqbqyi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2adntquec.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rtzmdvuq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nkhvuybb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ldhbbgfb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pvvuculb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcosah.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rbjztxul.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2njrbakbh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xzdpmztz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yonllfxl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ybihmutp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jiwdncbl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mxgmigze.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2oeuixepb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zlddmqjw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gwnwohkm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ensnkzin.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2asbvolgm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lpwggdpm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yzciondr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ecktzinp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dmgyruvj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xossvryt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ytybhnhk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kncgssbg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2niqdflpy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2obnqlcfm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bbddnqii.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2blcsuwlc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jdjiwpmv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xitdqdrn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2haebmari.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kgaupqgw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2olekrjlg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vpfexuld.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2reqkhllj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbwgdhhu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jpqlkjor.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gsxapvsv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nyrrntpp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2eqamvwdl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dxygcusb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqiradsp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnrjyozz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dbbvrxrf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rawevcab.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcjohpsj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ljymzkae.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rubrnwnm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vmspekym.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vgpuwvuj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2swsdgxpe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2frqqxkuu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptyfecsg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2twgdfqzu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mmagmzrw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqmjndjl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qadfkkjt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lpgsfccx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mmbmoklq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2keyntomk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqerbyov.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgabbs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nayvcapn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2knykrqzm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zwatnihd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hlndveld.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pnwogwww.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ughmnjow.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zhblobus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igkgqdpv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2emcnexjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkwzdssi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kawkezfe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zxleuvxx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iurvvlqi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2azhbnwoh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2blfimciz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2argfxtfp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rlkhdppz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cjbmxcer.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rggjtlqb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uawhqqfd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ivlcdjtb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tgsxfhex.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vwrtttit.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2twlokdle.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2utpvwufx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zhfleucy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2evcepkkj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pnyxdnft.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jedembtg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qyjascfx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ajpshcyf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qhwoqobf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aqgcgxym.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mxbihtsd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bqayoaox.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjllunjs.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mxttsxyw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bwiajtcs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2oleonjla.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lbicntmo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eukiyfzw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tmavuttf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fzwlcddp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pqdhjwvx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mfebwuhn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rkjldqol.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2crlgdgvw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vdyyfsey.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yzezdxsn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2enibotqy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2depqhoue.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xoudfega.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2khvgpbio.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcbojcww.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2naxezfut.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ysgoqqnc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ysxqzrem.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2loldzmfm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yzudrhuw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dubqgckh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2chpwkioy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sskqczfc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yliqvppx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2wvlnnlom.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vtntlkjj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2untepodd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ccaqfovh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oyitulfl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kewsmupm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dcltbjwy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2brwfnuln.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tdvvgasl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hiayavfm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgsmcvaa.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bvfjutuo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zvlvyajp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2knnyzahl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nhkijned.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bukyptwf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qbkvsrpa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ybdxvkfu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nvnanjgl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qbpkqyag.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2oiiypmjd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wakgttyh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xuvyhzzm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xknylomc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vfzslkoa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gnenngnt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lvyoembi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lncebblq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lmilwimt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2oyublbry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dxziyclx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oorcbjql.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qjzxaiwl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vucqlunz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfhxofat.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mmgwkcnj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywrbcygr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gkseoqbc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmwztbc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2amcomewq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nikwzusj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bxbwcwjg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2oxacxmeh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fsuoexgz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sczlgycb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kerrczwp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nyxfxsyc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2trigtnda.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eipbckyh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vpsbwdky.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rxducidz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oefgxgay.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iinohowx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ppywtdos.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2butzliht.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhmrujpt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2imdwcyst.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hmmvavwf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jtreoqhs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fllaoxda.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pmiwmtju.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vfvztfxf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lshptpxo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mvbtvgxl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bzjydutg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zasxufgb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ejurvsrq.html


<!-- 参考信息 -->