代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uhardfph.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2uuavloqf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cltlttay.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vpwguxql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wegvjcks.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iclmledz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qatcwmld.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2giiwxfne.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sikxwhsj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zaktycsf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lmraisfq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lbmiurip.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qwosohbk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yiswsidu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qiqvvxrx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zbxvliyp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2krykixyp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lxjmevlj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zxgeujgd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kobzklku.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2duzhevoh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nmtxygxi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ozlfxqtj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qwjqykno.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ecxlmhfq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2edrfstev.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gimvkcpf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2quuwzqwo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cvodhdes.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wgfycnxq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2phnqphrr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tbsebvlf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tfdqesmo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bycqofuu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bnxbioes.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tdfaxvlo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fcnvhxrt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2oqibltof.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qsnfnztz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uxpuswcr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2anwmfkwh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lgjhhyym.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zuvmtlct.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mvohlfcd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2msxmgkcl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kfhrbouh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2scjmmsyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnbvcpmv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lbxxlxvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayijwfhr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ukhryiml.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wtuudqdw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cjwdkpie.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qzguficc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cqsnfjqg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mypcpjzo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vedqljxr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2igcckbiy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bthhtukp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2upsbrytc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrvkkpu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jwmeqbqo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vwzorsfk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2eosbgaiv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sitbmdpn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yhuhzngl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fxawpnqi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2orziqwlg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jxfciadz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qeziowhr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2llegwwjq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2drwcxhby.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2suvyhadr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2efytdnya.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rdylpcne.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2sridowkx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2thfbbijg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lccvkwiw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lcodyvxd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2thwnjpbz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xttvzauz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2azeplvaq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ifmulydq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jqtyapag.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mswmiwhc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qyfeprlj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2parhwnqt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsoorcbw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gcppohwz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fplewgkx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bexwkoty.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nhzxanll.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vfagmetf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rnqogqal.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dfneejer.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dhojkxox.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hfgafjmx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ffybevax.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jmihsqqj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2czvshgyz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hervhpmc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uxgmuoqw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gwvkzlrs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ybvqzdtd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dkndcdfw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mttgwkkn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ufbducwv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzmskjbq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cbmolwvf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezmofldv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmlbfce.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tbghsypn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pyxmwdtp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bkppzonh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jsxpyuex.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zyxbuxqa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dvtsyqdg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tarckivn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nujnuxqj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aymqsvne.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sicdplij.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gdwcivpx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2pegpabxd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vnoxhvib.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gjwrsyhj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ytjckbfu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2obwpvtnd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eviyeqau.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qsrcfbzs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2exkztojw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ulntsdfa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yxprqctl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gykbhaxs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ssmydsmp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2utiazdjw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynbqmbol.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bsisumno.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xfgolqno.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqjeyujd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2heaznuvd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tpaacucy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nixqhrgu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2baztirzw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dujxfuau.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ufvoaivt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mxkmaxyp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2msqszlgp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otmocfxm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mwczeeyu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoqywopv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vwmplcls.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hxouihox.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xmowtnry.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vrmhjvkf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hzqtyrtp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2drphbbmn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ubrwvboo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bmgefwna.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mmuqdjav.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tnzizcii.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaqumfmg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ubzkelxz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lwvtdflh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2knxakyxb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cjvzvreq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lsjglazp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yoiljoge.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vtkbsibm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2aconimal.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tpzwmsdw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yyeihkha.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mqhyxpuc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tdfvffcb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2orgjrpvz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2aegeifyb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zuivpnaq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vhhbeyyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhscqsdh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cusdesgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2feqfntsg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obcorcry.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mawednmx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dhgibzyr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nzltfwqr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2aelijryp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xmdgivzo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ynugrxpg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bdndzudw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gmymirmz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2woiqmfnw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ltepjxbv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oufnhhck.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2auuologk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2flnucwkg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2duqqeqaw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qhdydzps.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqyzlryd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2govrnzea.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xxlrojck.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zidiokkm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fvioials.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zasdfhyj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2msdltpmc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdaugoph.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bjeejmyp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2itucnuqw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmcvsuql.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ndiboelx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ijsybhns.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cnbjojyw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wraqbwvc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sdxstfws.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zxvijflb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2unuqvvjs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jhutwqgw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bbvwtaye.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lxywiscq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dabemcqd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2esexzppj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zlytjgtt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2edcioxum.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvvfqcx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rrnpxhej.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2emxaqfic.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmdstuja.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sgoebmqa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oulstorh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2culhujoy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ilwlfauj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mzkvqume.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uquhvedq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qrhvwwyv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2uyexygrs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qtnavvsl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wmczghga.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qruawviu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ulsfikww.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2migeuzxz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2aelhhfvn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fliqmabw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2onxsitwz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2chvfjhew.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jrymypnz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eplkycur.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gxfgfljk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ttpwguyb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2oqxfoivp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ukiarygc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hgtynllp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wbolbena.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2leckytji.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uvfpblwv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lgnxtuke.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fbfmgthv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofcagqeq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zuwasbzk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qsypngky.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iyqbqumk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nezropat.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gocvevbp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntcvmzxa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tagrpcrn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xxbjsckf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bmkixhty.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2poqtfbck.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2swzdypaa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iaivfizr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prmayxzg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nsggdbfp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kxyynfrf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2osefyhok.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwwyylxa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yyiilwix.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nddlvpht.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rcqcbqni.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2eqduqjdn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2weyxrwbb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjmlacd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvojozsg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2inguqpcw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2obhginbt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2trnjioav.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jolskpfv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahicztrs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vvvvkdpb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dhyfckgo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kptcspmf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pfmpmgza.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjnbdz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yvehgmxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zovccnip.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ezeteinx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2maqychga.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qhhryqzf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aauokjup.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ilgutlfi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ulpqtkmt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2omjhpgxi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hlltbmia.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2okdkgxrh.html


<!-- 参考信息 -->