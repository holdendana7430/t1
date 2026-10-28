代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.kuanghao11.cn/gtfsarbfjz.html

[R70] 时间戳与互转
来源：http://hz.haohaochexian.top/gtxtqyelhp.html

date +%s;  date -d @1700000000
来源：http://hz.dashuyun.cn/gtmogwchbq.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtgvtfqfzx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gtnnmyxypq.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtqroiqeoq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtskfxgsnf.html

[R73] 分割大日志
来源：http://hz.yuanzhike.top/gtciupwypt.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtxaylnwwr.html

[R74] 批量重命名
来源：http://hz.nanxinkj.top/gtrgoxhxsl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhixingplan.top/gtsumpuszq.html

[R75] 导出环境变量
来源：http://hz.zhiwuduotai.top/gtcffzvkhe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtquychaav.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtqhznxsuf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gththfsdag.html

[R77] 读取用户输入
来源：http://hz.ybcxt.top/gtblheatqp.html

read -rp "请输入: " ans
来源：http://hz.jqgufenzy.top/gtupturqmw.html

[R78] 交互式菜单
来源：http://hz.yuanzhike.top/gtsouazspi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ehwqpu.com/gtkuasfizu.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtldaojcqy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zdqjudy.top/gtucxztqcn.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gttnxalfup.html

time ./run.sh
来源：http://hz.hongshengwenyu.top/gtpjljqdgm.html

================================================================================
来源：http://hz.yj202588.top/gttxxodsgp.html

S. C / C++ 专题
来源：http://hz.fengsongda.top/gtmckrofbo.html

================================================================================
来源：http://hz.cashguo.top/gtygrapzir.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gtmqugsoyr.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtfsyxxfwb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gtndqizxsx.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gtjktzseib.html

int a = 10; printf("%d\n", a);
来源：http://hz.hfpthk.cn/gtrdxtnuhc.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gtphldppmb.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtberkdhoe.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtguwdtmte.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtqurqpgvs.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtpcmpmldj.html

strlen(s)
来源：http://hz.xziqi.cn/gtdoiftuiw.html

[S06] C：字符串比较
来源：http://hz.zhijiandao.cn/gtjrfzfidu.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gttmryskcu.html

[S07] C：数组遍历求和
来源：http://hz.zhongyouzk.top/gtwuwnkega.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gtoivwxvip.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtdpbglgch.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ppjwa.cn/gtevftheuw.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtvunwanqm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtdyjsmlgy.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gttehvuqnu.html

int *p = &a;  *p = 5;
来源：http://hz.wangdashe.top/gtemnctjrv.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtelvabyex.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guannengcc.top/gtuhslemlp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhoulong.xyz/gtdeaqqfro.html

fclose(f);
来源：http://hz.shuidangran.top/gtnwilzuqh.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtkaderpxy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtbvivkabr.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gthcatsnoi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtnpsbhbtk.html

[S14] C：枚举
来源：http://hz.yj202588.top/gtocyffdww.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gthlgkqnxg.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtrggkrnsg.html

(double) a / b
来源：http://hz.bjfxy.top/gtjdbnwvqz.html

[S16] C：位操作置位
来源：http://hz.tianlin.xyz/gtwikxjtet.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtkebgszxe.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gthsdmzjis.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtiimmkgeh.html

[S18] C：命令行参数
来源：http://hz.zhixingplan.top/gtqcrjmcpk.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtaitnhise.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtwglfkgdf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtupvlghdv.html

[S20] C：二分查找
来源：http://hz.birdmap.top/gtcfdoqsov.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtpkehksiq.html

[S21] C：字符类别判断
来源：http://hz.ydzc1.top/gtnisibpxo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtbcqvafrg.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtahyfbwgu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtxvpvssvn.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gtigdgouxh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtftbocvxu.html

[S24] C：获取本地时间
来源：http://hz.cheryme.top/gtmyjtakvg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtskdatvpz.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtyrrkeqck.html

memcpy(dst, src, n);
来源：http://hz.iojbl.cn/gtunlbnxzx.html

[S26] C：内存清零
来源：http://hz.chenlongwang.top/gtzrhnvaex.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gtiazphkbj.html

[S27] C：定义常量
来源：http://hz.birdmap.top/gtkvcdaklu.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtguuwtebm.html

[S28] C：静态变量
来源：http://hz.kuanghao11.cn/gttlmrryaz.html

static int counter = 0;
来源：http://hz.nanxuanxn.top/gtrigihmdy.html

[S29] C：变参函数
来源：http://hz.hfpthk.cn/gtzeszosxf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtutwatciv.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtggxgozdj.html

#ifndef X_H
来源：http://hz.hnqzz.top/gtiwexiqnb.html

#define X_H
来源：http://hz.jinqigufen.top/gtgqjnwxqa.html

#endif
来源：http://hz.ybcxt.top/gtlgynziim.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtrpgzohnf.html

#include <iostream>
来源：http://hz.chenjidiqi.icu/gtihksgjtx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtxctfoklx.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gteinlursa.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtoastikri.html

[S33] C++：vector 增删
来源：http://hz.smart0.xyz/gtwcjqrgql.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yvedp.cn/gtelmpkkzd.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtrsanmbad.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xylfe.cn/gtftjnpaic.html

[S35] C++：map
来源：http://hz.xinyue.icu/gtjhntjbli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtwjxhrgkh.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gttqappskw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtoouqiclw.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtvqxqssxq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtokkaeiug.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gtgzdmkhgk.html

std::sort(v.begin(), v.end());
来源：http://hz.sysykeji.top/gtzwnqzdnn.html

[S39] C++：自定义比较器排序
来源：http://hz.xylfe.cn/gtkirqbyyy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gttwbctmiy.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtnokobmat.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shuidangran.top/gtolzbibql.html

[S41] C++：类与构造函数
来源：http://hz.zhoulong.xyz/gtwsfgqudx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tian-w.cn/gtzkbfjcgt.html

[S42] C++：继承与虚函数
来源：http://hz.jiagoushi.top/gtnhrkzqwz.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtkhmeffjq.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtefzkbyir.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinghuilouyu.cn/gtkyaqobtq.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtweonhohr.html

void inc(int &x) { ++x; }
来源：http://hz.hnxiangtu.top/gtmdklrirx.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtrhnaglkm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtxxyafteu.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtvdnbehwv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.redwolf501.top/gtravligos.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinghuilouyu.cn/gtkbcfrska.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gtwbumezvk.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtqhpqndzt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtdceqwivu.html

while (std::getline(in, line)) { }
来源：http://hz.hnxiangtu.top/gtrdeebtaw.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtepazvqef.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtdytghsun.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gtomrmyanc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xylfe.cn/gtfyyvsvys.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtpmygxfjw.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtukhedjjb.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtluarhmwm.html

int size() const noexcept { return n_; }
来源：http://hz.ivvv.top/gtqorhehsm.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtkllossst.html

std::vector<int> w = std::move(v);
来源：http://hz.zhijiandao.cn/gtpnchavrj.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gtbeswhnno.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangkeji.top/gtjyomjfkt.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtgazcufdg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtnuqybcmz.html

[S56] C++：optional
来源：http://hz.yuanzhike.top/gtafiylptd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtthhkfdlg.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gtfpuxmkxu.html

constexpr int N = 10;
来源：http://hz.yuxming.cn/gtajjdzant.html

[S58] C++：命名空间
来源：http://hz.zhixingplan.top/gtjqzxvooa.html

namespace ns { int f() { return 1; } }
来源：http://hz.sufxvd.cn/gtsswruqrx.html

[S59] C++：静态断言
来源：http://hz.quarkkingdee.top/gtjquwgncr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtrpjcgxtc.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gtrflbryoa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtiqtustom.html

================================================================================
来源：http://hz.jianghu66.top/gtbemsqumn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgufenzy.top/gtvqtomake.html

================================================================================
来源：http://hz.jinqigufen.top/gtsrmzihcy.html

[T01] Kotlin：Hello World
来源：http://hz.yonumen.top/gtiaeevhit.html

println("Hello")
来源：http://hz.jiagoushi.top/gtighjivcp.html

[T02] Kotlin：变量
来源：http://hz.dashuyun.cn/gthkyfbkhk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtglaadktu.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtrjtapswu.html

"值: $b"
来源：http://hz.316326.xyz/gtnnnlvbpf.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gteuokeosv.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtpznayqqh.html

[T05] Kotlin：when 表达式
来源：http://hz.c1oappe.top/gtcgrgfogo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinyuanbaomall.cn/gttpztaybn.html

[T06] Kotlin：集合映射
来源：http://hz.haohaochexian.top/gtuqpugycs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhaomingkeji.xyz/gtridqmjli.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gtaknhcvxt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtbvpcbwpc.html

[T08] Kotlin：数据类
来源：http://hz.bjfxy.top/gtgolitbun.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgufenzy.top/gtzvegbyzu.html

[T09] Kotlin：扩展函数
来源：http://hz.316326.xyz/gtgtjskmae.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtfkauuofe.html

[T10] Kotlin：默认参数
来源：http://hz.jlsjyb.cn/gteqgvzzmi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shangyingyoupin.top/gtfzljcvpb.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gthziyipmy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gthsnexzbw.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigfzy.top/gtxoosxvmp.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtcbzxdluf.html

[T13] Kotlin：只读 Map
来源：http://hz.guowangkeji.top/gtjyzfghjw.html

val m = mapOf("a" to 1)
来源：http://hz.guowangkeji.top/gtiepfziva.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gtvxhaywpm.html

for (i in 1..10) println(i)
来源：http://hz.yongpay.top/gtsqguecqs.html

[T15] Kotlin：接口
来源：http://hz.shuidangran.top/gtyyyprcji.html

interface Shape { fun area(): Double }
来源：http://hz.hfpthk.cn/gtcqlmuczf.html

[T16] Swift：Hello World
来源：http://hz.sweek.top/gtootukepf.html

print("Hello")
来源：http://hz.shuidangran.top/gtvugjfzvh.html

[T17] Swift：变量与常量
来源：http://hz.jinyuanbaomall.cn/gtheyioypm.html

var a = 1;  let b = 2
来源：http://hz.yvedp.cn/gtzmhebmdk.html

[T18] Swift：字符串插值
来源：http://hz.daria6918.cn/gtpetbiopk.html

"值: \(b)"
来源：http://hz.jinyuanbaomall.cn/gtsshcttxr.html

[T19] Swift：可选绑定
来源：http://hz.fengsongda.top/gtqoelxzob.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtviacdllx.html

[T20] Swift：数组操作
来源：http://hz.zhengqikj.top/gtwmaipezs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuxming.cn/gtfstmgwyb.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gtdjsfbiyt.html

for x in a { print(x) }
来源：http://hz.jqgfzy.top/gtxfaiuchp.html

[T22] Swift：字典
来源：http://hz.0kj1m.cn/gtpldkkzif.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangtech.top/gtykdnpsgk.html

[T23] Swift：函数
来源：http://hz.guannengcc.top/gteygmievl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jyoumei.cn/gtjklfddym.html

[T24] Swift：闭包
来源：http://hz.yueranfly.top/gtfahvuuws.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ehwqpu.com/gthvpvdphs.html

[T25] Swift：结构体
来源：http://hz.gzhubu.top/gtgbuamycx.html

struct P { var x: Int }
来源：http://hz.yonumen.top/gtseshiyse.html

[T26] Swift：类与重写
来源：http://hz.chenjidiqi.icu/gtikyvbsfs.html

class A: Base { override func f() {} }
来源：http://hz.xuanzx.com/gtcoduxmqq.html

[T27] Swift：错误处理
来源：http://hz.ywan-chungtsiang.top/gtyfhqbzht.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gtvfuiqryx.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtdoqxhxxp.html

enum Color { case red, green }
来源：http://hz.zhijiandao.cn/gtpqynuogx.html

[T29] Swift：guard 提前返回
来源：http://hz.kuanghao11.cn/gtnwoakyos.html

guard let x = opt else { return }
来源：http://hz.jqgufenzy.top/gtzethhxmp.html

[T30] Swift：协议
来源：http://hz.jianghu66.top/gtikbayygu.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtlelpjqzp.html

[T31] Lua：Hello World
来源：http://hz.bjfxy.top/gtlpavxrgn.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtfuyviclb.html

[T32] Lua：局部变量
来源：http://hz.shangyingyoupin.top/gtpzckiyth.html

local a = 1
来源：http://hz.cashguo.top/gturfnzxbj.html

[T33] Lua：表（数组）
来源：http://hz.smart0.xyz/gthhvinqfd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydzc1.top/gtfwxoujda.html

[T34] Lua：遍历表
来源：http://hz.gogol.net.cn/gtspqnbvqs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigfzy.top/gtmbwitzcq.html

[T35] Lua：字典表
来源：http://hz.svipenyu.cn/gtuadipqku.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ybcxt.top/gtzajognqc.html

[T36] Lua：函数
来源：http://hz.chenlongwang.top/gtbchvhsra.html

function add(a, b) return a + b end
来源：http://hz.xylfe.cn/gtchaizohy.html

[T37] Lua：字符串拼接
来源：http://hz.chenlongwang.top/gtzflshbxi.html

"a" .. "b"
来源：http://hz.hongshengwenyu.top/gtytrbkxkr.html

[T38] Lua：条件
来源：http://hz.zhixingplan.top/gtubmctfhy.html

if x > 0 then print("正") end
来源：http://hz.yangfankeji.com/gtetvetxra.html

[T39] Lua：模式匹配
来源：http://hz.shzxlz.cn/gtgaracjhd.html

string.find(s, "%d+")
来源：http://hz.jqgufenzy.top/gtckvtffwi.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gthlvalnzw.html

setmetatable({}, { __index = base })
来源：http://hz.xuanzx.com/gtietjhbzo.html

[T41] Perl：Hello World
来源：http://hz.hnqzz.top/gtiincgpvt.html

print "Hello\n";
来源：http://hz.yj202588.top/gtollfrdwv.html

[T42] Perl：变量类型
来源：http://hz.hongshengwenyu.top/gtawsacjav.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aibaodan.cn/gtdtqxqtqi.html

[T43] Perl：字符串插值
来源：http://hz.tanke756.top/gtjgolckcy.html

"值: $a"
来源：http://hz.yongpay.top/gtnkzhtsex.html

[T44] Perl：条件
来源：http://hz.shangyingyoupin.top/gtrcualdnk.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gtidwgkoui.html

[T45] Perl：数组遍历
来源：http://hz.dashuyun.cn/gtasduehma.html

for my $x (@arr) { print $x; }
来源：http://hz.iojbl.cn/gtqkxmkrav.html

[T46] Perl：哈希操作
来源：http://hz.nanxinkj.top/gtpmgapoco.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtvurgpcii.html

[T47] Perl：正则捕获
来源：http://hz.jianghu66.top/gtrhkfcysd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtmnqdczvu.html

[T48] Perl：正则替换
来源：http://hz.chenzaomai.com/gteqmspeps.html

$s =~ s/old/new/g;
来源：http://hz.quarkkingdee.top/gtseuudjkr.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtoailjglo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.mhx1999.top/gtdynwqgvf.html

[T50] Perl：逐行读文件
来源：http://hz.jqgufenzy.top/gtszknobjb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gtrafoziue.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.svipenyu.cn/gtefaihqtt.html

[T51] Scala：Hello World
来源：http://hz.jiagoushi.top/gtompxelfg.html

println("Hello")
来源：http://hz.xuanzx.com/gtiurunsga.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtmjpvtpqg.html

val a = 1;  var b = 2
来源：http://hz.gaohongyu789.top/gtwbscepuh.html

[T53] Scala：字符串插值
来源：http://hz.ydzc1.top/gtlufkzseu.html

s"值: $b"
来源：http://hz.mhx1999.top/gtvfewcwal.html

[T54] Scala：集合映射
来源：http://hz.wangshuangyany.cn/gtushfudua.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gogol.net.cn/gtmjloyxti.html

[T55] Scala：集合过滤
来源：http://hz.pycfn.com/gtfnhgpjrx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.bjfxy.top/gttibzqdnw.html

[T56] Scala：样例类
来源：http://hz.pengpengdd.cyou/gtgjzvnynq.html

case class User(name: String, age: Int)
来源：http://hz.dashuyun.cn/gtevoohgun.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtiiorjgem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yvedp.cn/gtlqfngxym.html

[T58] Scala：函数定义
来源：http://hz.ydjk.org.cn/gtxfyviony.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gotoacloud.top/gtzyobrkpe.html

[T59] Scala：循环
来源：http://hz.yj20258888.top/gtpsxfotdq.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtsycnbsoq.html

[T60] Scala：折叠
来源：http://hz.pengpengdd.cyou/gttgtfbsnn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtrvrlpxeb.html

================================================================================
来源：http://hz.xziqi.cn/gtxsiwnazv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gtacoglifu.html

================================================================================
来源：http://hz.xinyue.icu/gteelkseqd.html

[U01] Py：创建虚拟环境
来源：http://hz.cdnleiting.top/gtdkmehszj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtbgbybdmz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnxiangtu.top/gttsorcamf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shzxlz.cn/gtzyvwirbn.html

[U03] Py：加载 .env 配置
来源：http://hz.guowangkeji.top/gthbiksont.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtqivnqxlq.html

[U04] Py：变量调试打印
来源：http://hz.sysykeji.top/gtwcmvnjhu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtijrcinpe.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtgpggpver.html

list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gthqgjogpq.html

[U06] Py：合并两个字典
来源：http://hz.jiagoushi.top/gtumcbfrxa.html

{**a, **b}
来源：http://hz.ivvv.top/gtmzmljnoq.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangkeji.top/gtahxtykcg.html

{v: k for k, v in d.items()}
来源：http://hz.jinyuanbaomall.cn/gtnnxwcjtb.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtjkxtvaso.html

[y for x in nested for y in x]
来源：http://hz.yvedp.cn/gtkzolzwjd.html

[U09] Py：字典取最大值的键
来源：http://hz.ivvv.top/gtlrgeaeyd.html

max(d, key=d.get)
来源：http://hz.shzxlz.cn/gtqlorhemz.html

[U10] Py：按值排序字典
来源：http://hz.andypj.xyz/gtvufiwrxi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.aibaodan.cn/gtditgiaem.html


<!-- 参考信息 -->