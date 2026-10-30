代发 wailian999

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/glghdxllo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/grmyffumh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gekaqigjq.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gcaibcmjy.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gyvvjqjnv.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gefobfsis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gtrpicnit.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/ggvkjmogm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gnpafzbvi.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gbiqmqxyy.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gqbpzgpik.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gwpelfiqj.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/griazpzlw.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gslifxdwb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/ggaayzhku.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gztnnibxe.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gbfqmhvrj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gwypdxtak.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gfhawtlah.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gpksgcigl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gxstqsqtj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gfkomfyyg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gzmxphflx.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gqocqyeuf.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gxfrexgzi.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gwllnspwx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gpgkusriw.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gxnhdxzgw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gqdxsglrm.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gwcabstnz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gvbynqvbm.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gemgzfdos.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gafljwuiw.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gotqdkfsk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gfmtgfwpt.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gvglnxfux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gcrkgyhjx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gyhegivmu.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gcpynwwly.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guwcvhqfw.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gkkukivdt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqcrpdrry.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcpcfnpji.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gqzlugimr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gbgheyguq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gtxyimfpa.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gqdepobco.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gbwqlywjo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/ggxtolhgw.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gjfofnyph.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gayewfert.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gqjijlvlc.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gzkcoixef.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gsumseuas.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gebmzfvsc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gntfgilwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gwlknzunv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gdzpqeqxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzpmyqgb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gwbicjrij.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/ghhgrttdr.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gldhyfzyz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gfphrilaa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gexaptxjk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gnttxtldt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gssavvbeo.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqogfurqi.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gnriglvux.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gjvklwdee.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gztdgdszd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gbjksfqfu.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gwelsseuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/getacsxla.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gemolvlhx.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gzlinbevo.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gvcpbkdrk.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gawhltths.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpdoryllp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gtaysjntj.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gofxjydmb.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gmvfklara.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gpupojavt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/grckumaax.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gehqgmswj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmqgnnwtz.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gprizhsip.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gtesrhhio.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/giitjtdyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcdkratbm.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gtfegjmqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gridxagus.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gfqwmrrqc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gyjhjajpi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gyteuxwzy.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gxhpkhpnc.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gnvmtemcg.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/giadqvaql.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gbzivmvzl.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjqvrhjkn.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ggvxagfbw.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gnekxdcbo.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/glgmhtvho.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/goijmbosi.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gqlojqmcn.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gxekzvbww.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gdrmzulxz.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gezqckbwu.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gebdgduwu.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gnrrncwcg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftdmztiw.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gvxkmcdoe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gaschofff.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gvktbflth.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gpvtixift.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gwphtgrqg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gitknsepn.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gfkazfsag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdbjtbxjl.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gotqnimse.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gyourthdp.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gzxyqcirt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gaaxneaoq.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/ghcttbmhx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gaeygcbwe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gavokimox.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gmlmdbkex.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/ghbbtneid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gkabkxfsc.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gpleksuis.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gufactxaz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gzoemmurq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gchhvsjog.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gazxqxwwi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gyelnfqyn.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gdbbknrjf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/ggghxmzvu.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gqmggyoys.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gdqeftvyi.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gdpqjxkjk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gqqhkspmx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gfwaadbcq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gapcldvck.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gaahkqmtr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gputsjjyc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gurikncmx.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gjqypkcal.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gzqscpftl.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gqolzxhxi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gorevusyi.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/ggxcfdlcp.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gcbmtvttn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/geycsligt.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxpmxokv.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gdfttuvnh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/glifidgyr.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gbojpmfcg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gejtmglbf.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gdpxzhfje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gnnvmybll.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gibmzwlaq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gswuephyv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gacvjrenz.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gcerlfrub.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gfhwbeugf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gjdsfikcu.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gxnqruzxc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gnbmrjclz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gcxoivyff.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gbjbkclmd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyigwsalt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gwzdoihvz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goeudonkv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/greyazerq.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghsrxuhxl.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gdlftyyqr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gnfhvicqe.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gwvwiwpfm.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gayqqbpaw.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gaqwknatq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gtrantsno.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gfjitfisj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gbewhdrgy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gpqprguxf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gmttewqvs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gibffupal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gsfobccii.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gdtlectis.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gotdofzrc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gpaaavptl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/guznphjxi.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gpgmnkxji.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gmyudnzqt.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gnqbwcmlh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/ghmwjqayg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gmrizvzvm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gsoooipep.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gmshdchnp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gfajbzncy.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gbfqagpam.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gpfahtatf.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gsmipqewh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/geraixpmj.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gneltkvzw.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjqvibxkf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/giytdixuw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gagqfguxe.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gvflzvqmw.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/grvouzfgf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gywsochum.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gzhmcdfyx.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gazvuqvdv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/glnencelt.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gwrolprqt.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/glddyrypg.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gemcdeaut.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gcjmtfhdo.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gnvgeaaxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gcrqkppks.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gperkyihe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gohxpdkwk.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gcelxhgmu.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/geizjwqwa.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gdlhpcdiw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gdiccsnlf.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gdnghenkl.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gysaihdbl.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gxgcmraom.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gwbxcushu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gwiqolltr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gqgjpikuc.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/ghvtmfpiu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gcqjcgaqv.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gozcszraw.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gncqynpbv.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gujftytdq.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gwqkwplps.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gxxpifkig.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gmzmnlsfx.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/geydoctqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gnmoeqnsa.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gdcmbvycu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gamatiwta.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/ggweljraz.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gbjiiuxvc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gokirfbbx.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/glmxwwdgu.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gxwzocgay.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gzvarbfzl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/girgdxzmd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gjdmscxqv.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gbwbkmccu.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gmmeygukg.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdvyysgaf.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gzpxpiohj.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gntopnfbb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gotijejbb.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gkwerdfqt.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gqjyyeixp.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gmrtlchor.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/goyzkpfum.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/glqpzvjji.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gknmzzowq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/geknkcmej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gneldadmk.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gmktywvsh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gojjncrat.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gohurwmks.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gqerwcxzk.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gnqjtcxki.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvmkcairc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnwpdclon.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gwydpzhiz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/goakfysbm.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/guknwndko.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcbzwxakr.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gowxjktjf.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/grpwweivn.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gkazvphiz.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gjbjskmnh.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/glrabjmts.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gbzwpnnby.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gswxqfdwq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gicipkqrt.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/ggikofdpk.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gbwlhcvba.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkgftxrpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gaoaytuki.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gnjyiolkc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gxuqsutoi.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gfgzppctl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gbamzwcjt.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gmeoxvrmw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfapwylg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grnovhvhd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsrmznnaf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggjmdppum.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gjqacbcvp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/guuibvplp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/girdhodpd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gyzybzcfm.sHtML


<!-- 参考信息 -->