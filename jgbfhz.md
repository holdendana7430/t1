代发 wailian999

df -h;  du -sh *
来源：http://hz.pycfn.com/gtaqafdcbe.html

[R62] 找最占空间的文件
来源：http://hz.zhiwuduotai.top/gtjpuetjje.html

du -ah . | sort -rh | head -10
来源：http://hz.hongshengwenyu.top/gtiuoymcye.html

[R63] 内存与进程
来源：http://hz.yuanzhike.top/gtoqmjccrd.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtkoipexve.html

[R64] 结束进程
来源：http://hz.hongshengwenyu.top/gtxixpcfum.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gtxjkzgmar.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtmbmkeqeu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gogol.net.cn/gtpxptmysw.html

[R66] 定时任务
来源：http://hz.dashuyun.cn/gtpptjloug.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gttxwkysoe.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtcqmssdvr.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtvmybqmzj.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtdqwdihxp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xylfe.cn/gtutjyoprx.html

[R69] 生成随机密码
来源：http://hz.yongpay.top/gthagsopwi.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gtdayjgqzy.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtzdvccnam.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gthlhfwxhr.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtbrucgauq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.quarkkingdee.top/gtzvukgiev.html

[R72] 等待端口就绪
来源：http://hz.yueranfly.top/gtrcxrcugi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtqkmtflgz.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtmwdqssnt.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtsipzymmt.html

[R74] 批量重命名
来源：http://hz.jinyuanbaomall.cn/gtdlpejxgx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tianlin.xyz/gtfhcliags.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtodzzqpzs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtlyoywodb.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtawechfyq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtubsmyfku.html

[R77] 读取用户输入
来源：http://hz.zhongyouzk.top/gttgebuwdt.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtzlbanfbz.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtxmkydvyg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtvkzpqcnx.html

[R79] 解析命令行选项
来源：http://hz.gotoacloud.top/gtbrpaxyze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gtorzdosnj.html

[R80] 查看脚本执行耗时
来源：http://hz.guannengcc.top/gtmjqenltf.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtpvpvzywu.html

================================================================================
来源：http://hz.ydzc1.top/gtihtfivps.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtlzvhkmvp.html

================================================================================
来源：http://hz.shuidangran.top/gtppkuardy.html

[S01] C：Hello World
来源：http://hz.zhixingplan.top/gtwfgmxcdr.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtzhpobmqg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ywan-chungtsiang.top/gtttczpbae.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtnvfpoxye.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtftmajhzy.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gtskocggyc.html

int x; scanf("%d", &x);
来源：http://hz.meibo888.top/gturuymlue.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtltkbmuiw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258.top/gtoslijeqj.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtbplfmdup.html

strlen(s)
来源：http://hz.tanke756.top/gtkwvubokl.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtxpyovxdx.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gtnpnlkath.html

[S07] C：数组遍历求和
来源：http://hz.daria6918.cn/gtvpitejyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtohfbrxpf.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtoglrccra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtphsxumhq.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtzbkzikhx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cucudq.cn/gtgbrgcscr.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtmhntynig.html

int *p = &a;  *p = 5;
来源：http://hz.xziqi.cn/gtqdfxmgnk.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gttxnapnov.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fengsongda.top/gtxwxepmtx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.svipenyu.cn/gtvtxkrqcc.html

fclose(f);
来源：http://hz.sysykeji.top/gtjasgtzec.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtsmnqqyvs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.smart0.xyz/gtaqmvbscz.html

[S13] C：宏定义
来源：http://hz.ywan-chungtsiang.top/gtffswacup.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtclshejte.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtipjgjvil.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tianlin.xyz/gtofqggtgu.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtyoztaxpe.html

(double) a / b
来源：http://hz.sysykeji.top/gtfjhjaaft.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gttucsnjhc.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtgzlyatxj.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigfzy.top/gtjzogsytm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cucudq.cn/gtsdviuykz.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gttujalyzu.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtkattlayn.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gtrsxnsyyc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtvbxmrnvl.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtrrbksycc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtszdselhs.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtaaffstmg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigufen.top/gtnplxjebr.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gtcizvlail.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtxqrrhoit.html

[S23] C：随机数
来源：http://hz.daria6918.cn/gtvloczkfw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gthockddfk.html

[S24] C：获取本地时间
来源：http://hz.shangyingyoupin.top/gtnxhcqmdc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinyuanbaomall.cn/gtzycnqxza.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtylbdhpyv.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtjlgebteu.html

[S26] C：内存清零
来源：http://hz.jqgufenzy.top/gtjrfmtero.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtxpmbzsjo.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtcpharrgm.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtxpbhulju.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtsxvchdvn.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtwmtdpyyv.html

[S29] C：变参函数
来源：http://hz.sufxvd.cn/gtjxigbdrq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gtdlcdwsay.html

[S30] C：头文件保护
来源：http://hz.yj202588.top/gtvhigehxt.html

#ifndef X_H
来源：http://hz.chenjidiqi.icu/gtyoftkgpx.html

#define X_H
来源：http://hz.hywenlv.cn/gtzwxaeuaa.html

#endif
来源：http://hz.sufxvd.cn/gtwmtgpwnq.html

[S31] C++：Hello World
来源：http://hz.sufxvd.cn/gtuzqylsmz.html

#include <iostream>
来源：http://hz.tanke756.top/gtoailwchu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenlongwang.top/gtdjulbuhs.html

[S32] C++：字符串
来源：http://hz.zhengqikj.top/gtehwpdqcr.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gtdegxbikj.html

[S33] C++：vector 增删
来源：http://hz.hywenlv.cn/gtuqeptpki.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jlsjyb.cn/gtaebvykjs.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtxqvveual.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtrgquagpy.html

[S35] C++：map
来源：http://hz.tianlin.xyz/gtpmovwxkm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gthejhmuiu.html

[S36] C++：unordered_map
来源：http://hz.sufxvd.cn/gttcfrpwea.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtgkuavoba.html

[S37] C++：set
来源：http://hz.xinyue.icu/gteyxulumu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yangfankeji.com/gtavwuwwbi.html

[S38] C++：排序
来源：http://hz.xinyue.icu/gthoksrywh.html

std::sort(v.begin(), v.end());
来源：http://hz.jinyuanbaomall.cn/gteabrxbuv.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gttrwpuqfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.haohaochexian.top/gtmalzwhff.html

[S40] C++：查找元素
来源：http://hz.dianchejie.cn/gthgtdnkxx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigufen.top/gtmxpultci.html

[S41] C++：类与构造函数
来源：http://hz.hammf.cn/gtfmhsaoeh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtdvilatjd.html

[S42] C++：继承与虚函数
来源：http://hz.yj202588.top/gttcovzkrh.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gttgkvftnw.html

[S43] C++：智能指针
来源：http://hz.yvedp.cn/gttwokiswl.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtjkyqmwdk.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtgslhtmjq.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangtech.top/gtkwkobhir.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtsqllsdvh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnqzz.top/gtgbalufdw.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtdbeojkbj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenzaomai.com/gtalsiatad.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtnynkdnac.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtiyrhczpn.html

[S48] C++：逐行读文件
来源：http://hz.yvedp.cn/gtkweifgns.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.haohaochexian.top/gtzgfyrybo.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtaoaraxwp.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtkoqsqbsx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yongpay.top/gtsrtmpldz.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtnpinxaze.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gtwvpbksvb.html

[S51] C++：显式类型转换
来源：http://hz.jinqigufen.top/gtgtlxwnln.html

static_cast<double>(a) / b
来源：http://hz.xuetiantiany.cn/gtiatcmkbq.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtbkvubixn.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtahcnbveh.html

[S53] C++：移动语义
来源：http://hz.guannengcc.top/gtlfintmai.html

std::vector<int> w = std::move(v);
来源：http://hz.xylfe.cn/gthmbsdxir.html

[S54] C++：异常处理
来源：http://hz.jqgfzy.top/gtuqtvhvnc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daxiang520.top/gtrovecklr.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtbtsasqlh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zycfv.cn/gtixvmnmtu.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtkwduoahq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtlajcnoup.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gtxycwrmrh.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtsbsviicw.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtdlisphek.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtyjuaiwmd.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtizhdvkcq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtxofbmlzo.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gtrelrqotz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtaisdrprk.html

================================================================================
来源：http://hz.yj202588.top/gtvohkplau.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtlrprlusi.html

================================================================================
来源：http://hz.tianlin.xyz/gtrvxasyxk.html

[T01] Kotlin：Hello World
来源：http://hz.mhx1999.top/gtzqhavcnz.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtikjvmfac.html

[T02] Kotlin：变量
来源：http://hz.jinyuanbaomall.cn/gtswewxwcp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtjboordsb.html

[T03] Kotlin：字符串模板
来源：http://hz.feifeiyinyue.top/gtmmpbckwq.html

"值: $b"
来源：http://hz.ybcxt.top/gtjjgfucii.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gttpotocgd.html

val n: String? = null;  n?.length
来源：http://hz.jiagoushi.top/gtmylopjyx.html

[T05] Kotlin：when 表达式
来源：http://hz.hywenlv.cn/gtkniblnyw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtjcdgrqdh.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtemjyhykq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hongshengwenyu.top/gtlzgdusqe.html

[T07] Kotlin：集合过滤
来源：http://hz.redwolf501.top/gtfvyxvvnv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtfbosgumb.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtzwzgflom.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtgonzisbh.html

[T09] Kotlin：扩展函数
来源：http://hz.shangyingyoupin.top/gtqzmvljtw.html

fun String.exclaim() = this + "!"
来源：http://hz.cqqwz.cn/gthhivbfls.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtqfhbwnyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.0kj1m.cn/gtmgsavddy.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtshuyarpx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gtyvjvftmd.html

[T12] Kotlin：解构声明
来源：http://hz.wangdashe.top/gtoyrszrsx.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtyhacklmb.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gteqadvyzn.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gtsdgysegq.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gtyqptttgh.html

for (i in 1..10) println(i)
来源：http://hz.meibo888.top/gtxmvyaetb.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gthhtwpbyv.html

interface Shape { fun area(): Double }
来源：http://hz.hnxiangtu.top/gtewsrdufe.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtavyytcga.html

print("Hello")
来源：http://hz.316326.xyz/gtnbyjvqcy.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtlhffxzwt.html

var a = 1;  let b = 2
来源：http://hz.zycfv.cn/gtpltipzyd.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtduybhuvr.html

"值: \(b)"
来源：http://hz.hammf.cn/gtkagqvqif.html

[T19] Swift：可选绑定
来源：http://hz.aibaodan.cn/gtaqvlzyec.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtbqojvzye.html

[T20] Swift：数组操作
来源：http://hz.zhengqikj.top/gtddhjjqyw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtaksllvxz.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtsxqiuwah.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtjbchpbek.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtezcrtfko.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtytzjjjti.html

[T23] Swift：函数
来源：http://hz.svipenyu.cn/gtxuyuoyao.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenzaomai.com/gtgceujdzx.html

[T24] Swift：闭包
来源：http://hz.vqdsnc.cn/gtjbnujihk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cqqwz.cn/gtritlzsaq.html

[T25] Swift：结构体
来源：http://hz.ywan-chungtsiang.top/gtgxkjixjq.html

struct P { var x: Int }
来源：http://hz.shanyushiyangkeji.top/gtjxdqbnvb.html

[T26] Swift：类与重写
来源：http://hz.shuidangran.top/gtedebozsv.html

class A: Base { override func f() {} }
来源：http://hz.aibaodan.cn/gtwuoliywg.html

[T27] Swift：错误处理
来源：http://hz.yuanzhike.top/gtsycdfdct.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtofjrbipa.html

[T28] Swift：枚举
来源：http://hz.haohaochexian.top/gtiyynwthi.html

enum Color { case red, green }
来源：http://hz.ivvv.top/gtkbauqolw.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gttvidawym.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gtyauyhgtv.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtwrswvutb.html

protocol Shape { func area() -> Double }
来源：http://hz.guowangkeji.top/gtutjzltnk.html

[T31] Lua：Hello World
来源：http://hz.zhixingplan.top/gtegbupnzc.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtxeetsbrh.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gtubbgbzyh.html

local a = 1
来源：http://hz.yuanzhike.top/gtuldavgxo.html

[T33] Lua：表（数组）
来源：http://hz.hfpthk.cn/gtpbhcnlvt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtovdusmnd.html

[T34] Lua：遍历表
来源：http://hz.feifeiyinyue.top/gteioijojz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtkasumizj.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtvvdqoatg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.snrcjt.cn/gteqcwhsex.html

[T36] Lua：函数
来源：http://hz.hywenlv.cn/gtifevfrnd.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtddrrbuxc.html

[T37] Lua：字符串拼接
来源：http://hz.xuanzx.com/gtszwfgtgh.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtamdsqyxf.html

[T38] Lua：条件
来源：http://hz.chenjidiqi.icu/gtwnzksvgf.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gtggrliymh.html

[T39] Lua：模式匹配
来源：http://hz.zdqjudy.top/gtukltmrjv.html

string.find(s, "%d+")
来源：http://hz.jqgfzy.top/gtfvonjcxf.html

[T40] Lua：元表
来源：http://hz.zycfv.cn/gtpggcxwhn.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtgcveamml.html

[T41] Perl：Hello World
来源：http://hz.havefunace.top/gtnchtbtnr.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gturpqybrp.html

[T42] Perl：变量类型
来源：http://hz.cucudq.cn/gtjscutcpn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gtqcnaebbz.html

[T43] Perl：字符串插值
来源：http://hz.gaohongyu789.top/gttlaeoqux.html

"值: $a"
来源：http://hz.yongpay.top/gtpngebpvx.html

[T44] Perl：条件
来源：http://hz.nwbrower.top/gtwiumhktl.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtsuwkskfr.html

[T45] Perl：数组遍历
来源：http://hz.daxiang520.top/gtcaftztut.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gtluzzwlmx.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gtumgmtjma.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtaxgsbxoh.html

[T47] Perl：正则捕获
来源：http://hz.jyoumei.cn/gtiiuwnopa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sufxvd.cn/gtbwtxrbpa.html

[T48] Perl：正则替换
来源：http://hz.jinghuilouyu.cn/gtnvogldmm.html

$s =~ s/old/new/g;
来源：http://hz.yuxming.cn/gtvjfjbqwj.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtltfrgxkk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenlongwang.top/gtakktqfjc.html

[T50] Perl：逐行读文件
来源：http://hz.tanke756.top/gtzzrxcfyr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yongpay.top/gtwnuqrnyy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zdqjudy.top/gtpbzjrlsw.html

[T51] Scala：Hello World
来源：http://hz.jiagoushi.top/gtitiasbuf.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtylxqrios.html

[T52] Scala：变量
来源：http://hz.svipenyu.cn/gtqhurhjac.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gttbczhqhz.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangtech.top/gtmeqegmbo.html

s"值: $b"
来源：http://hz.c1oappe.top/gtvgpykftt.html

[T54] Scala：集合映射
来源：http://hz.jianghu66.top/gthtnmizft.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gtplwehivo.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtsgfjfjjd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sufxvd.cn/gtozemjtwn.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtwhnuhrxt.html

case class User(name: String, age: Int)
来源：http://hz.xuanzx.com/gtwdciynqu.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gtaafbivri.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhaomingkeji.xyz/gtglajnngd.html

[T58] Scala：函数定义
来源：http://hz.zhaomingkeji.xyz/gtmtdrymqm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aizwys.cn/gtyitxjzwb.html

[T59] Scala：循环
来源：http://hz.shzxlz.cn/gtwkyvykdc.html

for (i <- 1 to 10) println(i)
来源：http://hz.vqdsnc.cn/gtxvsibdxd.html

[T60] Scala：折叠
来源：http://hz.ppjwa.cn/gtkjxelqbv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhaomingkeji.xyz/gtjbqbnjnw.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfvbojeuj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtgrhvduvx.html

================================================================================
来源：http://hz.fengsongda.top/gtynkjefxh.html

[U01] Py：创建虚拟环境
来源：http://hz.sweek.top/gtreufsbzz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gtwkgadaso.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhijiandao.cn/gtvzvqhfyj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dashuyun.cn/gtwrhnsdqr.html


<!-- 参考信息 -->