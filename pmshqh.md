代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zlwzvcpy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3sycapnfk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3owcyyxng.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zgnwcxoc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iisgkcon.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yplpgiyb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vyftjdpp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3oesdkrgj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3eiyssccv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xxmzkpbm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bqtkabuv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nclisfxn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3onaljnez.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3duthvdex.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3neculiqn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nfaokpgi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3akzwjmtx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3igbgwilb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hwsexkkm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3itryanjt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3spdfthsr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tlvmozkn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ujrbqwnn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3goghkfue.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kfrxamib.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qfmflpqe.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bwwzqgkx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aqxguvkb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bmarqtdp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nedauhrt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wnsixvcn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3grpsoyew.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xfloesim.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zyziohvg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oqrffupq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zahfvxoq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qizhngvv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xjvnbmat.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aytonysv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bnkqjuwq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ufpnwvgj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ytxqljtz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gtaeqhpw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uyfqvltq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rxhcsxnx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lxmnsxcd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3oaihmsmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbvpikrm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3prnpwooo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flzqqyqg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wnwrlpbi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yxbbzutf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yjkfledu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pdctbmcs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wspalavl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mhmdiybh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gndzibwz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3arpnwrqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bxjhgqhu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gmejwwfr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kiiqlpnp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3urlrnwol.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3oiotfufz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yrudoxla.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3wkmubzfl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mcnrlfol.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eqexxpsa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pzjhtsdj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3whtwapjs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wdubycyh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tsarrqqa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yeczzdnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lmkojtvf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3yvvexdft.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kvmjeugx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3oruejzru.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3stfzvckk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ktbzczbi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mqmdvntu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3oxvuufkz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fzhstpck.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vnhdljxm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ftphctbr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3htwyjfoa.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfvyacam.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cjiyumis.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sojfygqh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nhzwxfcs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnvjwuw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hlwmsttv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xxtqequn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zygstllt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fhpresta.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yntxxfkl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lquoeznq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hmujbrsd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lhcsvydg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3njpalnqy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jciqmzcv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3apmttahm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uqgbaagy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ydloizwm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3cpduijft.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hvrfwvdz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3psawgjnu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tukramgj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dvaoilup.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3uminnupg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nbzgsjsn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tmmfnike.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ihzbcleg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jbqzuqrp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bqprrfos.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vctkjeud.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jldraywg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cmwwhgqf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ghsupjnm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvomwstv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yjugyjbr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rcnwnfpm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mutkeirh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jlhkfgye.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nicsemxf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ksalewde.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rgemyzdh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cvqwlzro.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3arojenil.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3texpbiuz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vrvhbzvl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mhwwcwnf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bgtjsyjs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xpnnbpnq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cneolles.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kmunwzjy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ffpesfdc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zwcwplkn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3axjjajhx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3iphltbcd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zjzsaeuw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wtrykxvb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mwlavdae.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pxxwhonw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xvnsyorg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ecgxnnha.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uvvoyvac.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hyoufiph.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hxdutqut.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3itnwugcg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zwukwaka.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3evjbxemy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uxsebdep.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bgfocxxq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yypmdgvt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qehyqfzh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gbzxiudv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iyioawwf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3glorocmo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hvhiuclm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fcfyinoh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hdttqegx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dslrbzln.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dcyieaqc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gpsfmuls.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gtjghedj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3elrkaeem.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3msmoxwns.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vycdpeet.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rbpxtvuh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3utupitqt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hemgtclj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lgdgotjw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tjejtrwf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3itgkbgnl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lauucqpa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bssqwkgi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xcgpbbpb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3appnokmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxqttenf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ezriwona.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vclukpjk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uugfztjb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wmoexjye.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3heiqvtwq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zijwhwaw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wxatnuvi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ppwlhhjz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hdvrqceq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hejlbknc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qcwvprnh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hacpmukr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kezwchjz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zptcjuky.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ktyescjc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sydkgkyi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xsyrarjz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbhnwjm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hiqlhvie.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ixhojves.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cnjrqzjq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3eryvylhj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bkvirzoe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yhikqurj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dogczxpj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dkctasgx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fnlluids.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dzonlmdn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mirtdewd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fcdwhkcg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkotag.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bsxankcn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3usftjgml.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eqlcevhw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qdkptykr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lpggezcn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3intcvbiz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bcqwylch.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3utzdlzzt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3srzpgmjy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zqrwpmjj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rzklywuy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rfxxltsr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3abstuvxj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3acsrlndz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hgthqgsk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uzpqcqss.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xpbtklkm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jsqxfugl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mttrgvne.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3enlclzqs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dcqswsrt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wbmbewba.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nszljhir.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cdveehds.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrnpoxd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zhuignwu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pfhvfqsi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hmozgblb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mfqunosa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xeuwodse.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhegqr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sykieupb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bhtlodvm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sfmmjnzw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxuxeebf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ppxfeaug.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rjvejreo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hszrjqmq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cbgxpxgk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3aahnhbhc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dfaoipuh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjguluxl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3akoxlvhs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ihvdfwss.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3yownzufn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3khmaauuk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3thpmaabq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xjsmpcdz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wqmheqdk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vosozsxb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rinzjpms.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqjpwtfv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cajowujl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xfubaabp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zglspqmw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fsekdfnn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hzebiynw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cxblxmsn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwhigdmy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqqwszfy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3btmxkakn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cxqwrcxz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iklgmkrt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mtopjfsf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lezyopfp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yehhrhaz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cfuzahva.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ioxoctep.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdhnummr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3itgzpklv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tzvdwgnd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xehfgtzj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ajtscpjz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3whbjgfjl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ybmwssgm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mqyxmoil.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ysvtrrej.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gepxjbzh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qjxnfpwr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bckgoskf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ajpvfdff.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddagmwzj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vjpolmcj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nitcwflu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3icvkihpu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yqqjqwfm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gapffvyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cutdflnx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hkloyopd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lroxgoox.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jgzqvwdo.html


<!-- 参考信息 -->