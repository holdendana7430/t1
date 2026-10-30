代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gfhqoykpw.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/ghxbppscx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gdjytfzee.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gprhcmutp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/grkidhvwv.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gwgpjvijv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gnerldfbj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gzfkrfpfo.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gzcgustmq.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gnidhxdnb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gdlqjbpte.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gbwulszka.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gtdbkmxcx.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gokzluhkg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gltcdnwbh.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gafecthtn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gqxssvgry.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gthurtjmu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gaydzjtqk.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gotlejync.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gmsdikuey.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gzjhtyhdg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gykztswqn.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gereszvbm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gaaspzvoq.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gimrxymev.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gyidadpel.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gbzfnwnje.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gkstryqve.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gkklthfam.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/grwrjhhje.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gyrleesvp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/ghpftgcmj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gctwojmnt.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gzfjubskj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxpeeslkz.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gwmkrvlta.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtavzrpki.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpbvfgnfg.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/galqxtuyn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gyexbggsp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/ghkxrhotj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gmzibjzdn.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/grvjgztrw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/ggloweywk.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gttmmnozp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glxhsemxv.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gsoohuhph.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gggfbnsgh.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/ghilxcror.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gbxnofive.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/glxisjtsk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/ggxmmhtks.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gkyvpcntd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gmkcufhvr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gnldklhkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gmaszxgsv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gvgmkvwco.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gmjuwgsck.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvvuvdacw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gntnxkcgl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gctskykkr.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gkpabhoxt.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/ghtcaclwr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbyoakcwe.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gfsvznpvm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gzetiqrim.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/ggflavoqp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gyuqnquau.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gmkvolnau.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gmpdhzdvg.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gktglwuis.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gxqrhsvbl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/glegpqepm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gepsmdele.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnbgttgkp.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gxxqmrnmq.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gbyhbsvab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gthezwosi.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gnmuyghcl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gcttklbxu.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gbvwpcipc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gimapgpnc.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gftdntljc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gznruaqun.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gpxfuagnz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gmhrborge.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gviapqncx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gwboggehn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/ggyrwchpj.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gkcrpyaah.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/ggyzjxxng.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gcjdehsbd.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gipsxgftd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkaoamfks.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gujxvgffs.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gxowuchxw.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gweootkrm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gclgllfvp.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gmpsufehd.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gibynpznh.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gsrvhieqb.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/guqrlijsf.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gayrqllos.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/ggfpcwxna.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsvnnwiw.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gwemrjyfq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gymihhobb.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gbgerfatu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gacppdxpb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gbsqvegzl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gzzjlsvmh.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gspfyervx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gjiupblio.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gsqeksils.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gcaeawshq.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gaulcnwmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqbfuyuce.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gzfjawgco.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ggzgvhmpy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gxixgcubh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gofdfighs.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/guvhugenb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gsjrgercu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/grcbrddas.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gzmylgxsk.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gmelcykdm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gycbfjvko.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gzoptjglv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gpmbgmeaz.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gobnecefx.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gharpdooe.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/ghslrpadj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gjiwmfrrs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfipjfe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gdhwfkjqk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gbefqzkkg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gmuqcszsd.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsmfrzblw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gifmfdvzk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gaenmnhcp.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gtihmqyml.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gnbyujthk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/ghbiamimb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gueyuixqb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gvuodoefz.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gfzctjpzs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gzdvycnna.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gzwjxvbvj.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/goinymypd.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gargrdrzv.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gwlnzwfwz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjypfwyqx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gbvjmtgvu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gfdafbjtb.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gzxvolkku.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfynxjgtv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gjyrrqnfv.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gfaqkefoh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gchupalgi.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gjzhfvdgz.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gfklsqwox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/ghohulwxe.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gcrzvtrhx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/guchtawqx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfkxhkaep.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gjcljpcos.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxzzsmyca.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyusgyiqg.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grzgjhsjw.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gywfyqjyh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gkhydmcgw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/glxddikeh.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gcygvpkxx.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gnmkhomai.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/guimiejdb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxerzepja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gorerwtek.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ggyghnrbk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcbdcipq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggkiimdft.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gfnlemwfn.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gepurkiig.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gcfzaottr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmmoikwsw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/ggxfcxznx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gjxccefac.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gkwxtmmud.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gviqrpmfa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gcoqpnnyf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/glzpgtnsf.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxquzrikr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gzbnsabum.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/glgblvovl.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gtkelqxvo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gyvmqrdqh.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gywaywmxg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/grsbxvfsn.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/guylshjqm.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghruybsij.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gbyphtbkx.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/glbdgungr.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghczywdhx.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gvscirdyg.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gqqkmdlpo.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gusiaofqs.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gcgnwkzod.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gdnrbolul.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/grsnibimb.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/glqatjzty.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gsncpaloc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gmarcnosh.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gjreekvhp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/ggroyciwy.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/ghawwcddq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/geegyvzue.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gowkglrzd.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gmrvzcovf.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gbhbyricb.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gycoyuugr.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gmkhsyrjy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/ghieulmwz.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gvbcxkiel.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gnqueperd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/glhmrzvjd.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gwlkottke.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gktggcoin.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gdmtldkuo.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/guivszmsm.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghepydsyg.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gqoajexjt.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gpcvizegs.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gwqyftolk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/genlbkuzg.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gghbijnkr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/ggjznszpi.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gvxzwpiqk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gioiznift.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gbewvmdwj.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gjxnrkirp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gavwkwhrr.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gxpwoyzmy.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gwixsyjwe.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gagtkmpmp.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gemxjsbcu.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gzlpjhskz.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/geeibceep.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gmhtymweo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gszhkgchv.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gzhappgtz.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gkzezicgb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/ghkinxoeu.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glpymfuhw.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gztfecjst.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gqvmfdzqe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gguwqlmhs.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gxmatsbij.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gzhtuvomb.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gjgwsszbm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gnqigxsoz.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gxyksztxw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/ggemdquxq.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/ghszbzjly.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gumfyreiv.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gbrcbplrb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggugttnql.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfuziucxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/glpffeqbd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/glehpmalv.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjiqeqwlz.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gaxhfugze.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/goffvghsl.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gdeffesqm.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gudcfombj.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gnwwchmmg.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gfwyzlyse.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gitrcykkw.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/ghxazlduq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gqwzanwdj.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gwqcxoipp.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gpmvvnwbu.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gqqkxrvzr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gnnbpdzgm.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gzwqfovkq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gftdbrykm.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gfouyckgg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gcgbbcxnz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gxerdesmq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gzwsbjgfq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gijafxtyb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyoxegbvz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdvgbwip.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gswqcyahz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gditakvta.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gfkdfzegt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gducctfvi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/ggwlicfet.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/ghgldtptl.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gvwhcpcyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gtkknuvgs.sHtML


<!-- 参考信息 -->