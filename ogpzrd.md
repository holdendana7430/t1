代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lqapybks.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2whlgsrag.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ztqrkwqq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dbusbbjb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qmyxurow.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bolnazjk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nyopzojk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hsawafzl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2trcynkzu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lvkydpkm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2iatnhszr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2brbqxgjm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nwtfgaji.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fwcgvtwh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tufsyaao.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2raawkzig.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tsqmjfon.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hadsoyqj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gzimncnq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2miqkvjzl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2swbepsnr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lvwpwqhu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2lirxjffz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fzcdwikp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ijatkpvo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lfzrjkff.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjvhuqow.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qxawznao.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ooandbov.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ibnhhmxv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2trodqijr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2socfzwwe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2probzexv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2robxhbqx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vymgurnl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yakrvqdo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sjtkjllb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fmrptgnr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vccianju.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xgocodwt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jnclpadn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ttfpioje.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pfyoniyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfcjhplr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gwurkiwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtboxbsu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghcnswbq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vzwtcmqy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvpipelj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hymcajur.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ytksdary.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2liaqgatx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dkgpmebq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2evurvapn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wbptnbhz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qbzxuaxk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnipkcch.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gxddxrzy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qbdwxehy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zdyrvvie.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lyqvvuvf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ezpvbhpn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2axiflhcp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lkpbotgd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2evuayalq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tnboyyqy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2toqzdwad.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hrctawlc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ulacutcr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eaohpvxt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fwzhzirm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sljxawds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yqtbpkmi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fgbreztf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nimsrzrw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ewuerxyx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xswgqsha.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yolyucos.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jvojrogx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jnujrhsl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2sllojufd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vunxbkhv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qkbvpfhu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dbuypcuk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vzjurndl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vjomuipm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ythqbbqp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vibgkcsn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mnhapegh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ithtlnns.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2okmnnevz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sqlsapss.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2trqqbuag.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wuxaklar.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pxoltyfk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ltiacuel.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sqehghuw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybpwxvma.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2omlljgur.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2lvupsbiv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bauecxvs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wkrjnmis.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pefkqnnd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mjreyxgm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tecnznim.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzxpodvz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ejryoylm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cpcqknzl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hhackarv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bylhkixx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ybenpazf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2njspzchk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2slfubfgb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pykxtydz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tzpicfmy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ojhdhzxu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dffzpeed.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmyxxjzm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pusmionp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zeddtkyh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2obirdtzp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vhswemmx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tgfeiban.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fdvdvapa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xkdjubik.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2diqpmihs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qpljjzlk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tpwcyece.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gmpprjtz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lfprmmjy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vgoqhthp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yxpmopnv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fnvgdhty.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2katggctu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ldyyslxn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xsynaocv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bapckyfs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjxspxsz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2veovyxfu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qcwwvhax.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bxfphjdv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dbvbwqna.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ntjxkjco.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bwkhtfow.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nnfxnjiw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbctoom.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wvzcapvg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ixayzwqj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yfxgthms.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2gvjbbyoj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tpcbgmzz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tiogfciy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqrknnhx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gxdziexj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pdqxgmrv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mdcsvlni.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnmidtuu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ilqjcpoq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fxhhdbhe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgqtswew.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2etyrtlym.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xqadgnvm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tljvqshp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zcuujdbi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnjurqj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2srpppxiw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ncwwvcmw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ydywrmnw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uidrzvfs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nltyajhd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2akzwtzjw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2criolyjb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sbtmgplw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahjtzspk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bqypedtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejkoybmd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mlwybuhp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2twzzjcbt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckkndfzd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fmjlqpdv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vewjjjor.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mvjpmsyw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2czxoiiju.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ayznmpgv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nbgbmoja.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cjzwnnou.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2eycawrpz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vyjykhye.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zprpmwgt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvyoeqh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cioiymhu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2munmxwex.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nttmdlti.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ojsjxngg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qldttsjb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ltoevlsn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2judahtoa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mbwxldst.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2msihdbjr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eufaehra.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ffkjghet.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngeuaoyr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dhelznrj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgboote.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ppzunybk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nqhfdplg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2blvjbgvt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ylkjtowx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ykowuodk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cbakgvhg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wuwnfiti.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2awrdwwzy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ropqzlux.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2steemcco.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2msojsdzi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qgebhqri.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2obcuewaw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jygxyngo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wzpuhnht.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2axduwptu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvaleqri.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2elfdcupe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mksviqtr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wbgfcxit.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qcyfmvqt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uepphwnz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2izbcvenn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2noqrqmid.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vcqbejrn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxbcltll.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2amzjquid.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qdpyfwsc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2guiokyli.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wkqcqhea.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pouvyuac.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tzsstwiz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iqajthxj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lzybwcvk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lvzdamvo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dcfofgom.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qbhmxtgd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dihzdhvp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hvkfihbe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tbwbmpua.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bwospcse.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kddztigh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ulmwzdyq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2icaqmtzq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2usashuuc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2yjchgpgy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dwxcjozt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lxudfrsi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jtxfdmus.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2uriehbfi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kvussmgd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cndvcupb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vvomizqg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mnavfnfd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2brnyodoq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vspoidce.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pxchzysm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2derethts.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2equxmvcd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ymtlbqhp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qmwnjljv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2muxdlqau.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hwxawrwc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdfwvodp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2blrxilyl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nmmbyxls.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2atpjsofh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2sjfyvdnc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2reevzkhl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzztbf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sclusire.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2matggtcv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2uvnjhgjr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jftvztol.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xqahbvdd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nqxxhber.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2peveqnej.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cdhntfav.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qtyzdoqn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gioesera.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ipgygkac.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lghvqtvk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jhemtdmx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gugqqnsm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cvcseofh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ibnalohb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fidxfzkx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2temqoxuv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2keiumeew.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tvnmcdrv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cdyftbxw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nnksibem.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fosxmhzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orfdcgmd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xxdxeqbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahogomzy.html


<!-- 参考信息 -->