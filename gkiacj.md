代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3towkgpta.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mciwooub.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ggxrttqg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fivknsse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iyxrteyb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ingoiaqx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nwrfmzye.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3seeuqgtp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3oqjdrmob.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzubfhxa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3iufefeui.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hidhpkhi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pzpobixh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sclykxjf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bephgcbc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kgcqokjs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3njffewwc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kzlhhayb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cmdghoto.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hjtwkpov.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uyervrru.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qapzrned.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rgckkenw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ztftxrpd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dgaukwif.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dvaslbxu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gbifefpj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cgjvegoi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hwcmfliv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nccuyspm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wiyqejuc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pptlzuea.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xftboqsl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mtuujrzl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rouercxd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fncbthah.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3burwxlcg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3atxetbgg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cryqithq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jiaimrqq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3lfqpbgte.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hebtvjxr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdtptfca.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kazquauk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kfuxsjpm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fngtqkpo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wobzwhyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjoatwtc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3khtbsqov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ladpqoox.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqysfvfk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3griagehl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ovazjwzd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxzhzjux.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hjjazrdx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bgzfldxk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uyfdcgus.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hxevfhvj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ltdvcnli.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jipwcdsz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zcwpnfof.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdbmglmg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fvcetxvc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3irgjcdbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tlomexqx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tkprzyhh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ekchxlbd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3adffwaji.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zcuylims.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xkcdqjkn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mftjwelc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iexlqhdd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xjcaelpm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ugzoabuo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fbmmjqmc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pdrirbjx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tpkgoyza.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nqargciz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rkvfmowx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jiasrefw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qjjfqojf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rznommre.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3sntlknlg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xgeabbrv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vtlwbrwh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcpctesr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tyoxnhnl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ftvbkipb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rqkvasbw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3psblidjx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vtdslzda.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3luofgrjr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxjyhul.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vpehfptw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bxmzuzfu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3byvkggaz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uqgpibpo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vpscmhqs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wunaekjc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zpvgrjwo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3aapbvtch.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gcklblyr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3urohjfdy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kfyyapxe.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yualkwty.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3spjwdbsx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dzsrfrsx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cmrtqijb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bfylyvba.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3iweumpgh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ogisrxes.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nopkqdow.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zyqazxvb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kncdefud.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xrgwdvev.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kufhdhke.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ikofbrxj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebddglat.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jpunypxz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kuouwpqj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3purrkgiq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvhcplve.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xxfawnyb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xrqeoyuc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xlxdseea.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ppuathtz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3iofmeqbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pkiznqnt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hfrupljr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cwonbfsc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vhziopnd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lcutbxfb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cusikaqj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vaebivjw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ypxttsmy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmpqrifo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wrljrjaw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bjylhggm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ptqvdzva.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xsbwvizh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3flxszlwm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tqyyckty.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3edepqvdp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfvcqhmu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xxvzzmvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3osrvjqkq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mpufazum.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzkplqo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dnkfpsyh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3haetjgli.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3znldpgeg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ktfroabk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hqzgwsje.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zwqdykvd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3iutllkxy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gqqxeoly.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wqmsrste.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jqmcsjfa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rcpsawvc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3axlskzoo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fahbzqit.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ufqzvqva.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xstlddih.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3enwxlrze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kqrtsfvv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qcyvbmcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kjhiqfay.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3usgwrjlq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dtbrwcgz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vrbdghkd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yargklsu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kbqgdkqo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wdrulanx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mqfnxtlr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lovjtzvc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lsnhmxku.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qsiabncg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kitdwxak.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ibwuguzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvfrmhqe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nfpbwmom.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3poxgiivz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3etihtftr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tbckzjwn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kkhnwcbw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nnwfgivp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vmbtczzc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gubhmpuq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ealbhtyr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rkkanwgd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hmoisico.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ydyqmrzf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3shhcfcrr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3odvzvjdv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3eelmzpko.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qkuoonph.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vtsqnrge.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gfpltunr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qkszielx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rhmddetp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3czzzsymi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tbtvtetc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gtixiwla.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nipfmdiw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wgugloeu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3netfsbmr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfkfplub.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3usbvmxdp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ugavjtwx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kyzecevr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wuxxjtrl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gqulklpc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cldmzhag.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xcnwounr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uqqqdwdr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3isifiunc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hghrwxwm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dylpscds.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hinanlse.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3blddnpel.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjelxgkz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wanlvwzj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mqeaqzyx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zpohkvwr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3skqbqswi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hqnpivhx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wogqyitt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqytkcc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ummuosmw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ncvlxgxv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3verpletr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3whzgvqgm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iazdqdpp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gwckypcs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rbsxguko.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xlwieovq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dbdfkzjd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hqfbrpod.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nbrzntdc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3oxqshrlg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ecuuhgqt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sqbpzlsj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ymqpofbl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ekozrlmo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3apgzzrpo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wyfjqjva.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3msvcmqxg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3obbnbdfp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3knceviyc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ixtffiwb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3axctgaxt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vunfkovt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3krfnwyru.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iernpkgf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mluigwks.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mfubdiog.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3asqqmizq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uuiczqmg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kdkcskyd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bqxbtatc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gnnlhlgs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lgfzuiro.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3trtvxkjp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tsignglz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xysojpce.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ksvgimcx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3azktdpdb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qrqljifz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zuoyarle.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgzwhwyo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yuuhesdz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rxqedodl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3unlpnuzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yalukiub.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cgvzlsuu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfwzlg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jinawzdg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zawnseym.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hneqolvu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hhtgzlqr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3elvdjgrv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3apcnboom.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uhscsgfs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fitaahjb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bruylepw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sygwemwi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ophethjo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qbzuwxey.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgflbfau.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yyfxiwnf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bmpunngw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3txkksqxn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ndvfpsrr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gvbqypuo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pnthhiic.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zdypuqws.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jwgxbxrw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ciddwlif.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pmtpldwq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mrfvzlfn.html


<!-- 参考信息 -->