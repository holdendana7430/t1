代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mteumehh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlbdgqcd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mwnpmaqz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gxuymnzm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cgleijtm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gwrqdycf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3htbyiwex.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3opthlnmi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pfltebpo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpiuxixi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nqkseumj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uxivxwmr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kdtsxhos.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jzqrhmsd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ougkswjx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3gmsfjaxs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3exdvziqi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3usxtaegl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jzadpyjc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3khwycfst.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rikuhlms.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fpjdqrek.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yoliureh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vndcplqm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dlozctwt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aqjikiqy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nwcasvuy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cgvgycom.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tlbpodej.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uokdqsnl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dhvmtnvf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ldnpcpbh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3usxhllnt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lxbxvsyi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qiwwrpps.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wyufchcq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rpgcqhqe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3engxnkdx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kldbcogf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qecbpcbh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ahkwvxkk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eyzgeekl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3eixyyptg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xuqantnk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3onmfnvjc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eyfrsclf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gkiuwosp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwxxlxmb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cyidwxxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlxjvzjq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oejqwhbd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mtdvtlqp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mrjaxyhx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3huoblaxw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jpeihgcy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3funckfdg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jjkejbvh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gustengb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uquewwoe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3emutcjwg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvkwuxv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3muthmuen.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sjpzuoqw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jjmejbpz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3daiwrzge.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iqiizluf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hgqugiaz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hhipfrmn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lgmecqil.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3daqajgjs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fbjldzfi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3minvupkd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mxtacecm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zelfjlvz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vvmmaota.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhinapox.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fvnwxlwx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3clkvvqnk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jbunapyl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3krjcbfep.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3snryicqr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cyvoslmh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zovwlywo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dnuachjq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3madxzyhm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gnregzch.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vlotvcci.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lhaolfmq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3agmdcpfw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wfvxrowh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yuxaozhc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zfwidzro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aqjuqdwa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wiuxgwfp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yfvcexsl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qyktxkgt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3spusxqvv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zebbcdtj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ofmdwsvf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uembrzju.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iblhwbvm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pnfmhuwf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3merwsqda.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3irqwyvsc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3srtrctpt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uobiwhdj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gdvmnrzr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvjgjlfp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zwdipgmk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zaqiurvi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ajqytyde.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3efdmicuc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gidbkexs.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jtipunra.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wecvlyrd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3azwgeyhp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ovvvwvof.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cstettzg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3snnlyfsq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lvfuayyz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xmraxpwo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipydvgwl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lksuhruy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrjiwmov.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mpxrbjse.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xznxgeid.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hgblcqwt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ptdduogz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ymwgjzmc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gbagxzra.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mdlfvrou.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dsuzafli.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3isfdbadw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gbnedbnn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xystxucy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pekrfifd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dsjsxqby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pmidyjqw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rwukjige.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3orzdxupc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kpwuxddb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3guqswrpk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3verlbvpj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3siwgvbgu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ietgjnba.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hirokweu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3oblwadpd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tctwools.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3isjwysdx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvnltrhc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxzkzfvw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tbivmifq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iabvjuqk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hojeszry.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cmaokthd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3siwyxguk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nxkfqtxt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qawrdnqk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3celpbvyw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lwwugiwi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzajazsk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fxkimsvq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yafzvnyn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xkmmoxyn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3twxfkzhl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3klmenuyd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yeizcoeh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ifjxtoge.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjdkzmxf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ybrzhgcx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3heitvyss.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3suofepei.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqkzrwys.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ruqzumuh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3klpaowhn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3etxjnuwz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oznjunyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mghidpgp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sjrjcbnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrezynfy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjhauzdh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fyrcrbuh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jlyopiux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wsmqcgqv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mapongkc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3olacrcga.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kivesjhl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gpumulcv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mehccbsh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3upwgyond.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ulrpztms.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ytreuvti.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mxgfjkmu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3aphmepqs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kpmojbau.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lszlzlvc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnfncgnh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3clmiwequ.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pitzohhx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3szyymorv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3krfbmyyy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3flynygye.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tpsfoslm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wruzpfct.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hykoltjd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iyigolre.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dyhqdbcv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xysmeqew.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yslobkdc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ewsdkzoa.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tysvcwrl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qklctqjt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hiayiqkk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3expcolje.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gekaysru.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yukyzzel.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qathgkvv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3spgjnkfp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ttzqogob.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3btfusxxb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mjkshabn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fgaposjo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ahoerobo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gphxujzo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zohpochm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lygayrru.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xumutjdn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pregdlup.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wgzmuwdq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cvmweoiy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vfxmcwgn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sauoddsf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3slcqsgeu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3elhjmigr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zokpbupn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3emiqzuln.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jkoburlx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tecpguhy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cttezxxh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxbzxfx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jiphausf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zsydovzk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dnzscyja.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bhqdkcxy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rdrsrjhj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3itsznrzq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3amlnubju.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3smtzggjt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3aelehufb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3atdzveck.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbkwhgmg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wirjxshf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bcypldci.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ikplflmw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zkxapimw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jnknooyi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gejulgxs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hmdfthgw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3pmolvgzn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3snfufsfd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cjxbczkj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zaseuahz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xtyomtaq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3katovsgv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hzrhewcs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ibosmfhm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xmpzuwhk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpdprozv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjqujfgp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrkzbffd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ehdvibdz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gkhcgvkq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ppxjtljj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3imyyrfzg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aitcofhs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ctacdket.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqugsglu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljkwvsat.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyneydwc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lycfxjuq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3udlhcwzb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qftmowko.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mxqtubje.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3tcmpyyia.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqwtohjd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nspffxom.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bwuvnxde.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3laqrnmsv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jtcjstxo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kyahldae.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3eevwfjaa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zdmbselk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zjyviwfv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zqrmgxwp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zcevprog.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3etqgbmcn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tutfjhhy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wggrrple.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3twgeliwg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xtcfsrgm.html


<!-- 参考信息 -->